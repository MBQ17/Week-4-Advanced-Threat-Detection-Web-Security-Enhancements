The project documented internship file focuses on Layered Security (Defense in Depth), which is the practice of combining multiple security controls to protect a system. 
This approach ensures that if one security layer fails, others are in place to stop an attacker. In project, this is achieved by merging system-level hardening with application-level security.
At the System Level, I utilized Fail2Ban on a Linux environment. Fail2Ban monitors system logs (like SSH login attempts) and automatically updates firewall rules to "ban" or block IP addresses 
that show malicious behavior, such as repeated failed password attempts. This prevents brute-force attacks from even reaching your application.
At the Application Level, the project uses Node.js and Express.js to build a secure API. Key security headers are implemented using the Helmet middleware, which helps prevent common web 
vulnerabilities like Cross-Site Scripting (XSS) and Clickjacking. Additionally, Rate Limiting is applied to ensure that no single user can overwhelm the server with too many requests, 
which protects the service from Denial of Service (DoS) attacks. Finally, API Key Authentication ensures that only authorized users with a specific secret key can access sensitive data, completing 
a robust security framework that protects the server from the outside in.
