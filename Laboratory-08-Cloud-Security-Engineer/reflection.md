# Reflection: The Cloud Security Engineer

In this laboratory activity, I learned how important it is to secure a server and control the network traffic that can access it. I used UFW, a host-based firewall, to manage incoming and outgoing connections on my Ubuntu environment. I also learned about the Principle of Least Privilege and the Default Deny policy, which help limit access to only what is needed.

A host-based firewall provides an additional layer of security even if the network's main security system is compromised. It can still control which connections are allowed directly on the server. Managing open ports is also important because every open port may provide another way for an attacker to access a system. By allowing only the ports needed by the application, we can reduce the server's attack surface and avoid unnecessary exposure.

Leaving a database port, such as port 3306 for MySQL, open to the public internet can be dangerous. Unauthorized users may attempt to connect to the database, especially if it has weak credentials or security settings. This could put important information at risk. Database access should be limited to trusted systems and users instead of allowing connections from everyone.

This activity changed my perspective on server security because I realized that running an application is not enough to keep it safe. Even a simple web server needs proper firewall rules and regular security checks. I also learned why it is important to allow SSH before enabling the firewall, since the wrong configuration may interrupt remote access.

Overall, completing this mission helped me understand the practical side of cloud security. Having eight completed missions in my GitHub portfolio also gives me a clearer record of what I have learned throughout the activities. It shows my progress in using cloud tools, managing containers, and applying basic security practices that I can continue improving as an IT student.