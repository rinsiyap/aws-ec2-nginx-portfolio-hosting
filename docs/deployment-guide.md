\# AWS EC2 Portfolio Website Hosting



\## Project Overview



This project demonstrates the deployment of a static portfolio website on an AWS EC2 Ubuntu server using Nginx, DuckDNS, and Let's Encrypt HTTPS.



\## Architecture



\- \*\*AWS EC2:\*\* Hosts the Ubuntu server.

\- \*\*Ubuntu Linux:\*\* Provides the server operating system.

\- \*\*Nginx:\*\* Serves the static HTML, CSS, and JavaScript files.

\- \*\*DuckDNS:\*\* Maps a hostname to the EC2 public IP address.

\- \*\*Let's Encrypt / Certbot:\*\* Provides and manages the HTTPS certificate.

\- \*\*Security Groups:\*\* Control inbound network traffic.



\## Implementation



1\. Launched an Ubuntu EC2 instance.

2\. Installed and started Nginx.

3\. Uploaded the portfolio website files to the server.

4\. Configured the website document root and file permissions.

5\. Created an Nginx server block for the portfolio hostname.

6\. Configured DuckDNS to point to the EC2 public IP.

7\. Obtained and installed an HTTPS certificate using Certbot.

8\. Configured HTTP-to-HTTPS redirection.

9\. Tested website responses, Nginx configuration, and certificate renewal.



\## Verification



The following checks succeeded during testing:



\- Nginx configuration test: `sudo nginx -t`

\- Nginx service status: `sudo systemctl is-active nginx`

\- HTTPS response: `HTTP 200 OK`

\- HTTP redirection: `HTTP 301 Moved Permanently`

\- Certificate renewal simulation: `sudo certbot renew --dry-run`



\## Security Considerations



\- Allow SSH access only from a trusted IP address.

\- Allow HTTP and HTTPS traffic as required.

\- Never commit private keys, access tokens, passwords, or cloud credentials.

\- Review AWS resources and billing before and after project cleanup.



\## Cost Management



The website was hosted on an EC2 instance. The instance should be terminated when no longer required, after verifying that the source code and documentation are safely stored in GitHub. Other AWS resources may continue to incur charges.



\## Current Status



The deployment was tested successfully. The live website may become unavailable after the EC2 instance is terminated or its public IP changes.



\## Learning Outcomes



\- Linux server administration

\- AWS EC2 deployment

\- Nginx configuration and web hosting

\- DNS hostname configuration

\- HTTPS certificate installation

\- HTTP-to-HTTPS redirection

\- Basic server security and troubleshooting

\- Git and GitHub version control

