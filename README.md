# listenverwaltung

# Netzwerkkonfiguration mit einer statischen IP-Adresse im lokalen Subnetz
sudo nmcli -p connection show <br/>
sudo nmcli c mod "Wired connection 1" ipv4.addresses 192.168.24.187 ipv4.method manual

# Zwei lokale Benutzer
## „willi“ – Normaler Benutzer ohne Administratorrechte
sudo adduser willi <br/>
Passwort festlegen und bestätigen

## „fernzugriff“ – Benutzer für den Zugriff von außen mittels SSH mit sudo-Rechten
sudo adduser fernzugriff <br/>
Passwort festlegen und bestätigen <br/>
sudo visudo <br/>
Zu den User privilege specification "fernzugriff ALL=(ALL:ALL) ALL" hinzufügen
