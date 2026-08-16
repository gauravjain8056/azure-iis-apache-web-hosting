# Azure Web Hosting – IIS & Apache

## Overview

Deployed and hosted a responsive HTML/CSS/JavaScript website on Microsoft Azure using both Apache on Ubuntu Linux and IIS on Windows Server.

## Technologies & Services

- Microsoft Azure
- Azure Virtual Machines
- Ubuntu 24.04 LTS
- Windows Server
- Apache HTTP Server
- Internet Information Services (IIS)
- HTML
- CSS
- JavaScript
- SSH
- Remote Desktop Protocol (RDP)

## Work Performed

### Apache on Ubuntu Linux

- Installed and configured Apache HTTP Server on an Ubuntu 24.04 LTS Azure VM.
- Deployed a static HTML/CSS/JavaScript website to `/var/www/html`.
- Configured Azure inbound HTTP access on port 80.
- Verified the website through the VM's public IP address.
- Troubleshot Linux file and directory permissions when website assets were not loading.
- Used `chmod` to provide appropriate read and directory traversal permissions.

### IIS on Windows Server

- Installed Internet Information Services (IIS) on a Windows Server Azure VM.
- Deployed the same HTML/CSS/JavaScript website to `C:\inetpub\wwwroot`.
- Configured Azure inbound HTTP access on port 80.
- Verified the website locally using `http://localhost`.
- Verified public access using the Azure VM's public IP address.
- Managed the IIS web server using Server Manager and IIS tools.

## Deployment Architecture

Microsoft Azure
- Ubuntu VM
  - Ubuntu 24.04 LTS
  - Apache
  - `/var/www/html`
  - HTTP :80
  - Hosted Website
- Windows VM
  - Windows Server
  - IIS
  - `C:\inetpub\wwwroot`
  - HTTP :80
  - Hosted Website

## Apache Deployment

Website files were placed in:

`/var/www/html`

Apache was installed using the Ubuntu package manager and managed as a system service.

Example commands used:

`sudo apt update`

`sudo apt install apache2 -y`

`sudo systemctl status apache2`

`sudo systemctl reload apache2`

## IIS Deployment

The website files were placed in:

`C:\inetpub\wwwroot`

IIS was installed through the Windows Server Add Roles and Features wizard and verified using both localhost and the Azure VM public IP.

## Key Learnings

- Hosting static websites on Linux and Windows servers
- Configuring and managing Apache HTTP Server
- Configuring and managing IIS
- Understanding Linux web server directory structures
- Understanding IIS web root configuration
- Working with HTTP port 80 and Azure network security rules
- Managing Linux file and directory permissions
- Deploying website files to cloud-based virtual machines
- Troubleshooting website asset and permission issues
- Comparing web hosting workflows between Linux and Windows

## Screenshots

Screenshots demonstrating Apache and IIS installation, configuration, deployment, troubleshooting, and public website access are included in the `screenshots` folder.
