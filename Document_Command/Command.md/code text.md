,,,
#!/bin/bash
yes | sudo apt update
yes | sudo apt install apache2
echo "<h1>Server Details</h1><p>strong>Hostname:</strong>$(hostname)</p><p><strong>IP
Address:</strong> $(hostname- I |cut -d " " -f1)</p>" >/var/www/html/index.html/index
sudo systemctl restart apache2
yes | sudo mkdir /var/www/html/index/foo
yes | sudo mkdir  /var/www/html/bar

#Create /foo.html 
echo "<h1>Hello from /foo</h1><p> This is a sample hello message in /foo.html.</p> /var/www/html/index

yes | sudo apt update
yes | sudo apt install apache2
echo "<h1>Server Details</h1><p>strong>Hostname:</strong>$(hostname)</p><p><strong>IP
Address:</strong> $(hostname- I |cut -d " " -f1)</p>" >/var/www/html/index.html/index
sudo systemctl restart apache2




