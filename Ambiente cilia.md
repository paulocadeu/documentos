
## Flatpak
gestão de pacote e virtualização para o sistema operacional Linux.
```bash
sudo apt install flatpak
```
The Flatpak plugin for the Software app makes it possible to install apps without needing the command line. To install, run:
```bash
sudo apt install gnome-software-plugin-flatpak
```
Flathub is the best place to get Flatpak apps. To enable it, run:
```bash
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```
## Slack
```bash
flatpak install flathub com.slack.Slack
```
# Editores de Texto
## Sublime Text
```bash
flatpak install flathub com.sublimetext.three
```
## Visual Studio Code
```bash
flatpak install flathub com.visualstudio.code
```
## Postman
```bash
flatpak install flathub com.getpostman.Postman
```
## Firefox
```bash
flatpak install flathub org.mozilla.firefox
```

## Google Chrome
por flatpak
```bash
flatpak install flathub com.google.Chrome
```



nativo
```bash
wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
sudo apt-get update ; sudo apt-get install google-chrome-stable -y
```


## Rbenv

```bash
sudo apt install -y git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev libffi-dev nodejs postgresql-client libpq-dev postgresql postgresql-contrib git-flow redis wkhtmltopdf ghostscript imagemagick --no-install-recommends
```

```bash
sudo nano /etc/apt/sources.list
```
### Adicione:
>deb http://security.ubuntu.com/ubuntu bionic-security main

```bash
sudo apt update && apt-cache policy libssl1.0-dev
sudo apt install libssl1.0-dev -y
```

```bash
git clone git://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
```

```bash
git clone git://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## Ruby
```bash
echo "gem: --no-document" > ~/.gemrc
rbenv install -v 2.1.6
rbenv local 2.1.6
rbenv rehash
```
