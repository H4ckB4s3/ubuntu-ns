# Handshake (HNS) Nameserver Setup for Ubuntu

This guide configures your Ubuntu system to resolve `.` (root) and Handshake top-level domains (TLDs) by adding the official HNS nameservers.

## One-liner (Quick Setup)

Run this command as root (or with `sudo`):

```bash
sudo bash -c 'cat > /etc/resolv.conf << EOF
nameserver 82.68.70.162
nameserver 82.68.70.163
nameserver 8.8.8.8
EOF'
