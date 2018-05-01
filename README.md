# install-ssl-lets-encrypt

sudo git clone https://github.com/rehmatworks/serverpilot-letsencrypt.git && cd serverpilot-letsencrypt && sudo mv sple.sh /usr/local/bin/rwssl && sudo chmod +x /usr/local/bin/rwssl && (crontab -l ; echo "@monthly \"sudo service nginx-sp stop && yes | letsencrypt --standalone renew &>/dev/null && service nginx-sp start && service nginx-sp reload\"")| crontab - && service cron reload

sudo -s

rwssl
