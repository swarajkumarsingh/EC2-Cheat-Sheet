# EC2 Cheatsheet
- Contains ec2 cheatsheet for most common scenarios like installing Nodejs, NPM, Docker, Golang, Grafana, Internet speed test, etc...


### Update applications
```
sudo apt update
```

### Git
```
sudo apt update
sudo apt install git
```

### Make
```
sudo apt update
sudo apt install make
ls /usr/bin/make
```

### Nodejs
```
sudo apt update
sudo apt install nodejs
node -v
```

### NPM
```
sudo apt update
sudo apt install npm
npm -v
```

### PM2
```
sudo npm install pm2 -g
pm2
```


### Docker
```
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
apt-cache policy docker-ce
sudo apt install docker-ce
sudo systemctl status docker
```


### Golang
```
sudo apt update
sudo apt install golang-go
golang version
```

### Django
```
sudo apt-get update
sudo apt install python3-pip -y
pip install django
```

### Grafana
```
sudo apt-get install -y apt-transport-https software-properties-common wget
sudo mkdir -p /etc/apt/keyrings/
wget -q -O - https://apt.grafana.com/gpg.key | gpg --dearmor | sudo tee /etc/apt/keyrings/grafana.gpg > /dev/null
echo "deb [signed-by=/etc/apt/keyrings/grafana.gpg] https://apt.grafana.com stable main" | sudo tee -a /etc/apt/sources.list.d/grafana.list
echo "deb [signed-by=/etc/apt/keyrings/grafana.gpg] https://apt.grafana.com beta main" | sudo tee -a /etc/apt/sources.list.d/grafana.list
sudo apt-get update
sudo apt-get install grafana
sudo systemctl start grafana-server
sudo systemctl status grafana-server
```

### Run .sh file
```
sudo sh <file_name.sh>
```

### Install htop
```
sudo apt update
sudo apt install htop
```

### Test internet speed
```
sudo apt update
apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 379CE192D401AB61
curl -s https://install.speedtest.net/app/cli/install.deb.sh | sudo bash
apt update
apt install speedtest-cli
speedtest-cli
```
