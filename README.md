# hombridge-fhem
Autostart-Skript für Homebridge

INSTALLATION

Voraussetzungen für Homebridge:

GCC 4.8
gcc --version

Node.js 5.0.0
node -v


Homebridge Installieren:

sudo npm install -g homebridge

Shim von Justme-1968 installieren:

npm install -g https://github.com/justme-1968/homebridge-fhem.git

config.json in den Ordner /home/<user>/.homebrige kopieren

Homebridge mit dem Befehl

homebridge 

starten


Autostartskript:
sudo nano /etc/init.d/homebridge

dort den inhalt vom homebridge-file einfügen


sudo chmod 755 /etc/init.d/homebridge
sudo update-rc.d homebridge defaults

danach startet homebridge automatisch. Folgende Kommandos stehen zur Verfügung:
sudo /etc/init.d/homebridge start
sudo /etc/init.d/homebridge stop
sudo /etc/init.d/homebridge status
sudo /etc/init.d/homebridge restart

Logs:

tail -f /var/log/homebridge.log
tail -f /var/log/homebridge.err
