#SIMPLE WEB STACK

User accesses www.foobar.com:
When a user wants to access the website, they enter www.foobar.com into their web browser.

DNS Lookup:
The domain name system (DNS) resolves the domain name www.foobar.com to the IP address of the server hosting the website. This is done through a DNS lookup.

Web Server:
The request is forwarded to a web server. The web server is responsible for processing the user's request and returning the appropriate response. It could be running Apache, Nginx or any other web server software.

Application Server:
If the web server needs to run any code, such as a database query or an API call, it forwards the request to an application server. The application server is responsible for running the code and returning the result back to the web server.

Database Server:
If the application server needs to access a database, it forwards the request to a database server. The database server is responsible for storing and retrieving data.

Issues That Can Affect A Simple Web Stack:

1. SPOF;

Single Point Of Failure (SPOF), is a part of the system that, if it fails the whole entire system stops from working.

The above infrastructure has no redundancy that can help in avoiding SPOFs, hence, any single failure in any part of the system will cause all the system to stop.

2. Downtime when maintenance needed (like deploying new code web server needs to be restarted);

The Infrastructure above, downtime will occur because we only have one server and one database, that is used to make the deployment and maintenance hence no way users will access the website in that period.

3. Cannot scale if too much incoming traffic;

The above infrastructure cannot scale if there’s too much incoming traffic because no second server in the system to share loads and the system will be overloaded.

The link to the diagram is https://imgur.com/a/NHnU7Ak