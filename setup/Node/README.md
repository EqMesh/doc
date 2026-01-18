# Node Setup

## basic install

apt update
apt upgrade
curl -fsSL https://tailscale.com/install.sh | sh


sudo tailscale up 
sudo tailscale down 

sudo tailscale up \
  --accept-dns=true \
  --advertise-routes=0.0.0.0/0,::/0,172.16.67.0/24 \
  --exit-node-allow-lan-access=true \
  --stateful-filtering=false

“Exit node + subnet routes require admin approval in the tailnet admin console.”

sudo tailscale serve reset
sudo tailscale serve /health /tmp/health.json


doublecheck serving works
curl -fsS https://<node-name>.ts.net/health

