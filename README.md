# labcsi
Lab materials for CSI WorkShop

https://console.bluemix.net



# Installation on Windows 10
Right-click the Windows PowerShell icon, and select Run as administrator
Run the following command:
Set-ExecutionPolicy Unrestricted; iex(New-Object Net.WebClient).DownloadString('http://ibm.biz/idt-win-installer')


# Go installation on Windows 10
- open a bash windows then run the following commands:
sudo apt-get update
sudo apt-get -y upgrade

wget https://dl.google.com/go/go1.11.4.linux-amd64.tar.gz
sudo tar -xvf go1.11.4.linux-amd64.tar.gz
sudo mv go /usr/local

export GOROOT=/usr/local/go
export GOPATH=$HOME/Projects/Proj1
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

vi ~/.profile

