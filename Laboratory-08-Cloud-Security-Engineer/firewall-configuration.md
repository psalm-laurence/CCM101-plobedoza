# Firewall Configuration

## Allow SSH

I allowed SSH traffic so administrators can continue managing the server remotely.

```bash
sudo ufw allow ssh
```

## Configure Default Policies

I configured the firewall to block incoming connections by default while allowing outgoing traffic.

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Enable the Firewall

I activated UFW and checked its status.

```bash
sudo ufw enable
sudo ufw status verbose
```

## Allow the Web Application

I added a rule to allow TCP traffic on port 8080 for the Nginx web application.

```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Why SSH Must Be Allowed First

If I enabled UFW before allowing SSH, incoming SSH connections could be blocked, potentially preventing remote administrators from accessing the server.
