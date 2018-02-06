# wslc
Retrieve SQL data from server with [LiveCode](https://livecode.org/) and [websocketd](https://github.com/joewalnes/websocketd).

For security reason, most of the database servers does not allow remote connection and to be able to access a non exposed database servers I have to install LiveCode Server edition as a CGI processor or use a "middleware" code like PHP or Python.
With websocketd, I can run my executable livecode desktop application on the server without the hassle of server installation, and I like to keep my project as simple as possible without too many programming language. 
For simplicity I use SQLite as the database for this example project.

# How-to
* Create a new stack on LiveCode IDE and paste the code from sqldata.livecode to the stack script
* Save as standalone application
* [Download and install websocketd](https://github.com/joewalnes/websocketd/wiki/Download-and-install)
* Open command prompt and go to the standalone application folder created by LiveCode IDE.
