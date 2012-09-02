This is an improved version of the hello word Nginx module found at http://blog.zhuzhaoyuan.com/2009/08/creating-a-hello-world-nginx-module/
This module also accepts a value to the module directive and validates its value as well as prints it, instead of printing static "Hello World"

The sample configuration can look like 

    server {
            listen 8080;
        server_name localhost;

        location / {
                 hello 'Hello World';
        }
     }
