# wslc
Retrieve SQL data from server with [LiveCode](https://livecode.org/) and [websocketd](https://github.com/joewalnes/websocketd).

For security reason, most of the database servers does not allow remote connection and to be able to access a non exposed database servers I have to install LiveCode Server edition as a CGI processor or use a "middleware" code like PHP or Python.
With websocketd, I can run my executable livecode desktop application on the server without the hassle of server installation, and I like to keep my project as simple as possible without too many programming language.
For simplicity I use SQLite database for this example project.

# How-to
* Create a new stack on LiveCode IDE and paste the code from sqldata.livecode to the stack script
* Save as standalone application
* Navigate to the stand alone application folder and Create or download sqldata.html
* Download the sample database sqldata.db

  OR
  
* [Download prebuild binaries](https://github.com/samansjukur/wslc/releases/latest)
 
-------------------------------------------------------------------------------------------------------------------------------
* [Download and install websocketd](https://github.com/joewalnes/websocketd/wiki/Download-and-install)
* Open command prompt and go to application folder created with LiveCode or ./sqldata folder if download from prebuild binaries
* If you are using linux, make sure file sqldata have execute permission
* $ websocketd --port=8080 --staticdir=. ./sqldata -ui
* Open http://localhost:8080/sqldata.html with your browser
