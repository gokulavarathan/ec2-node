# EC2-node
ec2 deployment comments for node application

Node Hello World
Simple node.js app that servers 

Great for testing simple deployments on Cloud

Step 1: Install NodeJS and NPM using nvm
Install node version manager (nvm) by typing the following at the command line.

sudo su -

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash

Activate nvm by typing the following at the command line.

. ~/.nvm/nvm.sh

Use nvm to install the latest version of Node.js by typing the following at the command line.

nvm install node

Test that node and npm are installed and running correctly by typing the following at the terminal:

node -v

npm -v

Step 2: Install Git and clone repository from GitHub
To install git, run below commands in the terminal window:

sudo apt-get update -y

sudo apt-get install git -y

Just to verify if system has git installed or not, please run below command in terminal:

git version

This command will print the git version in the terminal.

Run below command to clone the code repository from Github:

git clone gitURL

Get inside the directory and Install Packages

cd nodejs-on-ec2

npm install

npm install pm2@latest -g

Start the application To start the application, run the below command in the terminal:

npm start


# insert the new value into the system config

echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p

# check that the new value was applied

cat /proc/sys/fs/inotify/max_user_watches

# config variable name (not runnable)

fs.inotify.max_user_watches=524288
