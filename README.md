# listenverwaltung

# Netzwerkkonfiguration mit einer statischen IP-Adresse im lokalen Subnetz
sudo nmcli -p connection show
sudo nmcli c mod "Wired connection 1" ipv4.addresses 192.168.24.187 ipv4.method manual
