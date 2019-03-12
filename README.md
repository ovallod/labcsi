# labcsi
Lab materials for CSI WorkShop

https://console.bluemix.net



# Installation on Windows 10
Right-click the Windows PowerShell icon, and select Run as administrator

Run the following command:

Set-ExecutionPolicy Unrestricted; iex(New-Object Net.WebClient).DownloadString('http://ibm.biz/idt-win-installer')


# install Golang on Windows 10 bash
- open a bash windows then run the following commands:

sudo apt-get update

sudo apt-get -y upgrade

wget https://dl.google.com/go/go1.11.4.linux-amd64.tar.gz

sudo tar -xvf go1.11.4.linux-amd64.tar.gz

sudo mv go /usr/local

mkdir $HOME/gosrc

export GOROOT=/usr/local/go

export GOPATH=$HOME/gosrc

export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

vi ~/.profile

sudo apt install gcc

#	Install NodeJS

Run the following commands in a bash PowerShell window:

curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -

sudo apt-get install -y nodejs

sudo apt install npm

#	Install Hyperledger fabric packages

cd $GOPATH 

mkdir src;cd src; mkdir github.com; cd github.com; mkdir hyperledger;cd hyperledger

git clone https://github.com/hyperledger/fabric.git

cd fabric

git checkout tags/v1.2.1


