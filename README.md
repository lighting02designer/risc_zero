# sunucu güncelleme
sudo apt update
sudo apt upgrade -y


# nvmi yükleyelim
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash
source ~/.bashrc

# geçici dizin oluşturup içine giriyoruz
mkdir ~/p0tion-tmp
cd ~/p0tion-tmp

#  nvm v16.20 kurmak
nvm install 16.20
nvm use 16.20


# phase2cli yüklüyoruz
npm i @p0tion/phase2cli

screen -S risczero
npx phase2cli contribute
