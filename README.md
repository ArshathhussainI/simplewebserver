# EX01 Developing a Simple Webserver
## Date:20-11-2024

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.


### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
''' from http.server import HTTPServer,BaseHTTPRequestHandler

content='''

LAPTOP CONFIGURATION
System configuration	Description
Processor	i5
Primary Memory	Ram 16 GB
Secondary Memory	512 GB
0.S	Windows 11
Graphic	nvidia
</body>
'''
class MyServer(BaseHTTPRequestHandler): def do_GET(self): print("Get request received...") self.send_response(200) self.send_header("content-type", "text/html")
self.end_headers() self.wfile.write(content.encode())

print("This is my webserver") server_address =('',8000) httpd = HTTPServer(server_address,MyServer) httpd.serve_forever() '''

## OUTPUT:

![380017945-18a9c0f7-2f55-4b59-9c71-e762b01473de](https://github.com/user-attachments/assets/a84ab4e4-79e9-46d4-be62-1afb8bd419ad)


## RESULT:
The program for implementing simple webserver is executed successfully.
