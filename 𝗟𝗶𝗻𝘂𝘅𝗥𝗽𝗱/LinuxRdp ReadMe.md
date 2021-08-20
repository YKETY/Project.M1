#--Cuda Install--
- wget https://developer.download.nvidia.com/compute/cuda/11.4.1/local_installers/cuda-repo-debian10-11-4-local_11.4.1-470.57.02-1_amd64.deb
- sudo dpkg -i cuda-repo-debian10-11-4-local_11.4.1-470.57.02-1_amd64.deb
- sudo apt-key add /var/cuda-repo-debian10-11-4-local/7fa2af80.pub
- sudo add-apt-repository contrib
- sudo apt-get update
- sudo apt-get -y install cuda

#--Miner install--
- mkdir rdp
- cd rdp
- wget https://phoenixminer.info/downloads/PhoenixMiner_5.6d_Linux.tar.gz
- tar -xf PhoenixMiner_5.6d_Linux.tar.gz
- cd PhoenixMiner_5.6d_Linux
- apt install nano
- nano start_miner.sh

#--Edit Your Wallet Details--
- ./PhoenixMiner -pool ssl://us1-etc.ethermine.org:5555 -pool2 ssl://eu1-etc.ethermine.org:5555 -wal <your_wallet>.<your worker_id>

#--Install gnome--
- cd rdp/PhoenixMiner_5.6d_Linux
- sudo apt-get install ubuntu-gnome-desktop
- ./start_miner.sh
