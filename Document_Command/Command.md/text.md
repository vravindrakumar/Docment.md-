
#!/bin/bash
yes | sudo apt update
yes |  sudo apt install apache2
echo "<h1>Server Details</h1><p>strong>Hostname:</strong>$(hostname)</p><p><strong>IP
Address:</strong> $(hostname- I |cut -d " " -f1)</p>" >/var/www/html/index.html/index
sudo systemctl restart apache2

$tail - 3000 /var/log/cloud-init-output.log