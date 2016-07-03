# sbhackathon2
#必要なもんいれる
sudo apt-get install -y nodejs npm

sudo npm cache clean

sudo npm install n -g

sudo n stable

sudo ln -sf /usr/local/bin/node /usr/bin/node

#最初にいれたのややこいから消す
sudo apt-get purge -y nodejs npm

#ディレクトリ作って移動
mkdir devwebsocket

cd devwebsocket/

#cloneする
git clone git://github.com/gasugasu/sbhackathon2.git

#npm install する
npm install

#起動する。
npm start

#確認方法
~~http://hostname:3001/chatbox.htmlにアクセスし、話しかける。~~
~~おうむ返ししたら成功。~~
以下のURLにアクセスし、相互の発話を受信できたらOK
http://hostname:3001/chatbox.html?userid=0002&ID=87ce0a699af03dbba6212b65649952ab
http://hostname:3001/chatbox.html?userid=0003&ID=87ce0a699af03dbba6212b65649952ab

#備考
routes/module/mod_socket.jsをネット見ながら適当に書いただけ。

