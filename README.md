Not my work just trying to put it in English and make it more reachable/accessible for non Russian users

# InstagramTelegramBot
Telegram Bot monitoring Instagram accounts and send photos
Now bot parsing RSS-feed of websta.me, getting photos with titles and send it to subscribers

Commands:
```
1. /start - adding chat to 
2. /admin token - adding user as administrator (other users can't subscribe and not getting photos, it's private bot)
3. %username% - getting menu for subscribe / unsubscribe / getting photos of username
```

config_local.py template
```
BOT_API_TOKEN = '''your token for bot by telegram'''
BOT_ADMIN_PASSWORD = 'password / token for bot admin'
KEY = '''encryption key for db'''
```

# WIP How to install on Ubuntu 18.04
```
sudo apt install -y python3 python3-pip libsqlcipher-dev build-essential git
wget https://files.pythonhosted.org/packages/96/d9/40e4e515d3e17ed0adbbde1078e8518f8c4e3628496b56eb8f026a02b9e4/urllib3-1.21.1.tar.gz
tar zxvf urllib3-1.21.1.tar.gz
cd urllib3-1.21.1
python3 setup.py install
git clone https://github.com/bntjah/InstagramTelegramBot/
cd InstagramTelegramBot
pip3 install -r requirements.txt
```
