#SCALEUP

Server: The server is the foundational element of the infrastructure, responsible for hosting and running the software components that make up the application. In this case, we are splitting the components (web server, application server, and database) onto separate servers for scalability, fault tolerance, and isolation.

Load balancer (HAProxy): The load balancer is added to distribute traffic evenly across the multiple servers hosting the application components. This helps to ensure high availability and scalability by preventing any one server from becoming overloaded with traffic. By configuring the load balancer as a cluster, we can ensure that it is fault-tolerant and highly available, so that if one load balancer fails, the other can take over without service interruption.

Web Server: The web server is responsible for serving static content to users, such as HTML, CSS, and JavaScript files. By separating the web server onto its own server, we can scale it independently of the application server and database, which may have different performance characteristics and resource requirements.

Application Server: The application server is responsible for running the business logic of the application, processing requests from the web server and communicating with the database. By separating the application server onto its own server, we can scale it independently of the web server and database, which may have different performance characteristics and resource requirements.

Database: The database is responsible for storing and managing the data used by the application. By separating the database onto its own server, we can ensure that it has dedicated resources and is not impacted by the performance of the other application components. This also allows us to scale the database independently of the web server and application server, which may have different performance characteristics and resource requirements.