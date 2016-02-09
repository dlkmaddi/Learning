B
B
B
C
C
C
C
C
# Learning
This is Learning Repository

package "httpd" do
 action :install
end
  


service "httpd" do
 action [ :enable, :start ]
end


cookbook_file "/var/www/html/index.html" do
 source "index.html"
 mode "0644"
end
