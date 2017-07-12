# tomcat-as-service-linux
This repo to show how to start up tomcat as service under linux distro

tomcat-script Redhat Distrubtion

# Setup 
if you havn't tomcat user 
sudo groupadd tomcat
sudo useradd -s /sbin/nologin -g tomcat -d /path/to/tomcat-server

sudo vim /etc/init.d/tomcat
copy script into tomcat file or download script from repo then copy to /etc/init.d
sudo chmod +x /etc/init.d/tomcat
sudo chkconfig tomcat on


# NOTE

Before running the script make sure it has permissions to execute and you run it with root permissions.

Set execution permissions with chmod +x tomcat.sh and execute it with root permissions with sudo .

# Example usage and output

For starting service
sudo service tomcat start

For stop service
sudo service tomcat stop

For restart service
sudo service tomcat restart

# License

The MIT License (MIT)

Copyright (c) 2017 Omar Eisa

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
