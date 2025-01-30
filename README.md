# power-shell

Task:

Date: 30-01-2025
task
#!/bin/bash
echo "enter url"
read -r url

git clone "$url"
cd docker-k8s

mvn clean package
webappspath="C:\Program Files\Apache Software Foundation\Tomcat 10.1\webapps"
cp target/*.war "$webappspath"
binpath="C:\Program Files\Apache Software Foundation\Tomcat 10.1\bin"
cd "$binpath"
./catalina.bat start


 2) give repository link "Remote Repo"
 3) Tomcat:8090 open
 4) target folder open there is helloword file is present
 5) Tomcat:8090//hello.snapshot it done!!!!!!!!!
