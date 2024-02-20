Basics of the Infrastructure

What is a Server?
A server is a computer or system that provides resources, data, services, or programs to other computers, known as clients, over a network. In the context of web infrastructure, servers are powerful computers that store, process, and deliver web pages to users.

What is the Role of the Domain Name?
The domain name serves as a human-readable address for a website. It is used to identify one or more IP addresses with a name that is easier to remember and use in web browsers. For example, the domain name `google.com` represents about a dozen IP addresses.

What Type of DNS Record `www` is in `www.foobar.com`
The `www` in `www.foobar.com` typically corresponds to a CNAME or A record in the Domain Name System (DNS). The CNAME record would point `www` to another domain name, indicating the actual host where the services are running, while an A record would point directly to the IP address of the server where the website is hosted.

What is the Role of the Web Server?
The web server's role is to accept requests from clients (web browsers) and send them the requested web pages, usually in the form of HTML documents along with additional content such as images, style sheets, and JavaScript. Servers like Apache and Nginx are examples of web servers.

What is the Role of the Application Server?
The application server is a framework that provides both facilities to create web applications and a server environment to run them. It acts as a set of components accessible to the software developer through an API defined by the platform itself. For web applications, it provides functionalities such as session management, database connectivity, and messaging, while also executing the logic of the applications.

What is the Role of the Database?
The database is a centralized collection of data that is stored and accessed electronically. Databases support the storage, retrieval, modification, and deletion of data. They play a crucial role in web applications for managing user information, preferences, and application data, ensuring data persistence across sessions.

What is the Server Using to Communicate with the Computer of the User Requesting the Website?
The server communicates with the user's computer using the Hypertext Transfer Protocol (HTTP) or its secure version, HTTPS. When a user requests a webpage, the user's browser sends an HTTP request to the server, which then responds with an HTTP response, including the requested page content.

Issues with the Infrastructure

Single Point of Failure (SPOF)
A single point of failure is a part of a system that, if it fails, will stop the entire system from working. This could be a single server, a database, or a network component. If this component goes down, the entire website or application becomes inaccessible.

Downtime When Maintenance Is Needed
When deploying new code or performing maintenance, the web server might need to be restarted, leading to downtime. This is an issue because it makes the website temporarily unavailable to users.

Cannot Scale If Too Much Incoming Traffic
If the infrastructure is set up on a single server or has limited resources, it might not be able to handle high volumes of traffic effectively. This can lead to slow response times or even a total outage if the server is overwhelmed.

Solutions
- Eliminating SPOF: Use redundant and distributed systems, such as load balancers and clusters of servers.
- Zero-Downtime Deployments: Implement blue-green deployments, rolling updates, or canary releases to update the system without taking it offline.
- Scalability: Use horizontal scaling (adding more machines) or vertical scaling (adding resources to existing machines) to handle increased loads. Additionally, implementing auto-scaling based on traffic can help manage unexpected spikes in demand.

Addressing these issues involves strategic planning and investment in infrastructure to ensure reliability, availability, and scalability.
