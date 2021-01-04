## Training Courses

**Visit : https://joycode-art.github.io/training-courses**

### build your own

#### install nodejs

```sh
sudo apt-get install nodejs
sudo apt-get install npm
```

upgrade:

```sh
sudo npm install npm -g
npm install –g n stable
```

modify repo:

```sh
npm get registry 
npm config set registry http://registry.npm.taobao.org/
# npm config set registry https://registry.npmjs.org/
```

#### install gitbook

```sh
npm install gitbook-cli -g
gitbook -V
```

#### install plugins

```sh
gitbook install
```

#### review book

```sh
gitbook serve
```

#### publish book to github pages

```sh
rm -rf docs
gitbook build
mv _book docs
git add ./docs
git commit -m "publish book"
git push
```

#### generate book

##### install ebook converter

- download Calibre: https://calibre-ebook.com/download
- install Calibre
- config Calibre


MACOS:

```sh
sudo ln -s ~/Applications/calibre.app/Contents/MacOS/ebook-convert /usr/bin
```

Or:

```sh
vi ~/.bash_profile

export EBOOK_PATH=/Applications/calibre.app/Contents/MacOS
export PATH=$PATH:$EBOOK_PATH 

source .bash_profile
```

##### generate pdf

```sh
gitbook pdf
```

#####  generate epub

```sh
gitbook epub
```

