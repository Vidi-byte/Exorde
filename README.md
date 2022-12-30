# Exorde
#### Install packages download git 
```
apt update
apt install git
apt install apt-transport-https ca-certificates software-properties-common curl
```
#### Install the dock, start it and check it 
```
curl -f -s -S -L https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
apt update
sudo apt install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y
sudo systemctl status docker
```
## Run the container with YOUR ERC 20 address below is an example ( 0x69b9b1D16feD43... replace with your ERC 20) 
```
docker run -d --restart unless-stopped --pull always --name exorde-cli exordelabs/exorde-cli -m 0x69b9b1D16feD43Dc89188441030DcD6a70Cd8642 -l 2
```
#### After a while, your EPC 20 should appear in the checker for up to 24 hours.
#### Link to the check: https://explorer.exorde.network/leaderboard
