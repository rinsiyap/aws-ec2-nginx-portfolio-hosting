# \# AWS EC2 Portfolio Website Hosting

# 

# A static personal portfolio website deployed on an AWS EC2 Ubuntu server using Nginx, a DuckDNS hostname, and HTTPS with Let's Encrypt.

# 

# \## Project Overview

# 

# This project demonstrates practical skills in cloud infrastructure, Linux server administration, web hosting, DNS configuration, HTTPS setup, and troubleshooting.

# 

# \## Architecture

# 

# \*\*User → DNS (DuckDNS) → AWS EC2 Security Group → Ubuntu Server → Nginx → Portfolio Website\*\*

# 

# \- \*\*AWS EC2:\*\* Virtual server hosting the website.

# \- \*\*Ubuntu:\*\* Server operating system.

# \- \*\*Nginx:\*\* Web server serving the static website.

# \- \*\*DuckDNS:\*\* Hostname mapped to the EC2 public IP address.

# \- \*\*Let's Encrypt and Certbot:\*\* HTTPS certificate issuance and management.

# \- \*\*AWS Security Groups:\*\* Network access controls for SSH, HTTP, and HTTPS.

# 

# \## Technologies Used

# 

# \- AWS EC2

# \- Ubuntu Linux

# \- Nginx

# \- HTML5

# \- CSS3

# \- JavaScript

# \- DuckDNS

# \- Let's Encrypt

# \- Certbot

# \- Git and GitHub

# 

# \## Features

# 

# \- Responsive personal portfolio website

# \- Static website hosting on a cloud server

# \- Custom DNS hostname

# \- HTTPS certificate configuration

# \- HTTP-to-HTTPS redirection

# \- Nginx server block configuration

# \- Linux file permissions and service management

# 

# \## Deployment and Testing

# 

# The deployment steps and technical details are documented in \[`docs/deployment-guide.md`](docs/deployment-guide.md).

# 

# Successful checks during testing included:

# 

# \- `sudo nginx -t` — Nginx configuration validation

# \- `sudo systemctl is-active nginx` — service status

# \- `curl -I https://rinsiya-portfolio.duckdns.org` — HTTPS response returned `200 OK`

# \- `curl -I http://rinsiya-portfolio.duckdns.org` — HTTP redirected with `301 Moved Permanently`

# \- `sudo certbot renew --dry-run` — certificate renewal simulation succeeded

# 

# These results reflect the tests performed during deployment; they do not guarantee the website remains online.

# 

# \## Security Practices

# 

# \- Keep private keys and credentials out of version control.

# \- Restrict SSH access to trusted IP addresses.

# \- Use HTTPS for encrypted website traffic.

# \- Validate web server configuration before reloading services.

# \- Review cloud resources and billing after completing a lab.

# 

# \## Cost Management

# 

# The website ran on an EC2 instance. The instance will be terminated after the repository and documentation are verified. The live URL may stop working after termination. Other AWS resources can still incur charges, so check them separately.

# 

# \## Repository Structure

# 

# ```text

# aws-ec2-nginx-portfolio-hosting/

# ├── index.html

# ├── style.css

# ├── script.js

# ├── .gitignore

# ├── README.md

# └── docs/

# &#x20;   └── deployment-guide.md

# ```

# 

# \## Learning Outcomes

# 

# \- Cloud server provisioning

# \- Linux administration

# \- Nginx web hosting and configuration

# \- DNS and HTTPS configuration

# \- Troubleshooting and verification

# \- Git version control and GitHub documentation

# 

# \## Author

# 

# Rinsiya

# 

# This repository contains the website source code and technical documentation for a hands-on cloud hosting project.

