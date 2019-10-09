# Sledge Deployment

(fall 2019)

Eventually I hope to make Sledge deployment as automated as possible but until
that happens this repo contains deployment information for now.

## Server Information

Instance type: `t3.medium`

IP: `3.132.24.73` (IPv4 only)

DNS: `judge.hackru.org`

## Checklist

 * Setup ec2 instance, use Debian 9 image

 * Port blocking will be done on AWS only (no iptables), only SSH, HTTP and
   HTTPS allowed (incoming)

 * Instance RAM is 4GB, but to be safe I want to add another 4GB swap backed by
   seperate EBS storage

 * Node v12 and npm should be built from source

 * Redirect everything to HTTPS, and get certificates (certbot/Let's Encrypt)

 * Nginx config files
