# node-httpc
Node CLI tool made to simulate curl like functions.Httpc currently only supports HTTP GET and POST requests only

# Installaton
1) Clone the repository. Make sure that node is installed on your machine.
2) Depending on the branch, the folder "node_modules" may or may not exist. If it does not exist, open a terminal in the folder, and use the command "npm install" to install node modules.
3) try "httpc help" to check if the application was properly installed

# Example Get Request (non verbose)
httpc get 'http://httpbin.org/get?course=networking&assignment=1'

# Example Get Request (verbose)
httpc get -v 'http://httpbin.org/get?course=networking&assignment=1'


# Post Request
httpc post -h "Content-Type: application/json" --d '{"Assignment": 1}' http://httpbin.org/post
