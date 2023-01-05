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
## Node check commands 
#### Check if your containers are working 
```
docker ps -a
```
#### Restart node
```
docker restart exorde-cli
```
####  Checking Logs.
```
docker logs --follow  exorde-cli
```
#### The official website of the project read a lot of useful is : https://taiko.xyz/docs/alpha-1-testnet/start-here
#### Request ETH from Ethereum A1: https://l1faucet.a1.taiko.xyz/.
#### Request ETH from Taiko A1: https://l2faucet.a1.taiko.xyz/.
#### Deployed on L1: https://l1explorer.a1.taiko.xyz/address/0x3612E284D763f42f5E4CB72B1602b23DAEC3cA60
#### Deployed on L2: https://l2explorer.a1.taiko.xyz/address/0x0000777700000000000000000000000000000002
