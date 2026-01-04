# piwall

Security services node for Raspberry Pi 4.

## Services
- AdGuard Home (DNS / ad / malware blocking)
- WireGuard VPN (wg-easy)
- Portainer (Docker management)

## Setup
```bash
sudo mkdir -p /opt/piwall
sudo chown -R $USER:$USER /opt/piwall

git clone https://github.com/ankitmshra/piwall.git /opt/piwall
cd /opt/piwall

cp .env.example .env

docker compose up -d
```