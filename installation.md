You will need to install node, as well as npm. Most latest ubuntu distributions come with node and npm pre-installed.

```shell
node --version
npm --version
# if not installed install using apt
sudo apt update && \
    sudo apt install node && \
    sudo apt install npm
```

For React to work, you will need at least node 14. My Ubuntu server had 10.x so I needed to follow below process

```shell
# Install Curl
sudo apt-get install -y curl
# Download node
curl -fsSL https://deb.nodesource.com/setup_23.x -o nodesource_setup.sh
# Prepare setup
sudo -E bash nodesource_setup.sh
# Install node
sudo apt-get install -y nodejs
```