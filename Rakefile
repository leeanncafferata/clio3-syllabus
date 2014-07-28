require "rake/clean"

desc "Preview the site with Jekyll"
task :preview do

  puts "Previewing the site locally with Jekyll."

  jekyllPid  = Process.spawn("jekyll serve --watch --baseurl")

  trap("INT") {
    [jekyllPid].each { |pid| Process.kill(9, pid) rescue Errno::ESRCH }
    exit 0
  }

  [jekyllPid].each { |pid| Process.wait(pid) }

end

:wa

desc "Build the production version of the site"
task :build do
  puts "\nBuilding the production version of the site ..."
  ok_failed system "jekyll build"
end

desc "Deploy the site via rsync"
task :rsync do
  puts "\nDeploying the site via rsync..."

  ssh_port       = "22"
  ssh_user       = "lincolnm@lincolnmullen.org"
  rsync_delete   = true
  rsync_options  = "--checksum --stats -avze"
  public_dir     = "public" 
  document_root  = "~/public_html/lincolnmullen.com/courses/clio3.2014"

  exclude = ""
  if File.exists?('./rsync-exclude')
    exclude = "--exclude-from '#{File.expand_path('./rsync-exclude')}'"
  end

  ok_failed system("rsync #{rsync_options} 'ssh -p #{ssh_port}' #{exclude} #{"--delete" unless rsync_delete == false} #{public_dir}/ #{ssh_user}:#{document_root}")
end

desc "Build and deploy the production version of the site"
task :deploy => [:build, :rsync]

def ok_failed(condition)
  if (condition)
    puts "OK"
  else
    puts "FAILED"
  end
end

CLOBBER.include('public/*')
