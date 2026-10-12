# Mission Reflection

This laboratory helped me understand why server security is important in cloud computing. I learned how a firewall controls network traffic and how proper port management can protect a server from unauthorized access.

First, a host-based firewall protects a server by controlling incoming and outgoing network connections directly on the server. Even if the physical network perimeter is breached, the firewall can still block traffic that is not allowed by its rules. This provides an additional layer of security through the principle of defense in depth.

Second, managing open network ports is important because every open port may provide an entry point for attackers. Allowing only the ports needed by an application reduces the server's attack surface and helps prevent unauthorized connections. In this activity, I allowed SSH on port 22 and web application traffic on TCP port 8080.

Third, leaving a database port such as MySQL port 3306 open to the public internet is dangerous because attackers may attempt to guess passwords, exploit vulnerabilities, or gain unauthorized access to sensitive information. In a real enterprise environment, database access should be restricted to trusted application servers or authorized networks instead of being publicly accessible.

Fourth, this mission changed my perspective on how easily a server can be compromised. I realized that deploying an application is not enough; the server must also be secured through firewall rules, careful port management, and regular security checks. A simple configuration mistake can expose services to unwanted connections.

Finally, completing eight missions has helped me build a more organized GitHub cloud computing portfolio. It contains my laboratory activities and documentation, showing my progress in learning cloud infrastructure, deployment, operations, and security. It also gives me a place to demonstrate the technical skills I have practiced and continue improving.

