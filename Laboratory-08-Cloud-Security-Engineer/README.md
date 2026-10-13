# Laboratory 08: The Cloud Security Engineer

## Mission Overview

This mission focuses on securing a server using a host-based firewall. I configured UFW to control incoming and outgoing traffic and allowed only the necessary connections for SSH and the web application.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Configure UFW with a Default Deny incoming policy.
- Allow SSH and TCP traffic on port 8080.
- Document and verify firewall rules.

## Commands Executed

```bash
docker run -d -p 8080:80 --name secure-web-app nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

- Running and testing an Nginx Docker container.
- Configuring a host-based firewall with UFW.
- Applying a Default Deny incoming policy.
- Allowing specific network ports.
- Checking firewall status and documenting security configurations.