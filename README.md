#           **Отчет Lab12**
##                *Report*
- `Ход работы`

- Были выплнены следующие команды
```
export GITHUB_USERNAME=Alex1505Gold
vimtutor ru
git clone https://github.com/${GITHUB_USERNAME}/lab07 lab12 #В лабораторной 11 не создавался новый репозиторий, поэтому был склонирован 7 репозитрий
cd lab12
git remote remove origin
git remote add origin https://github.com/${GITHUB_USERNAME}/lab12
vim README.md
:s/lab11/lab12/g
/file<CR>wChaving the path environment variable value **LOG_PATH**<ESC>
:wq
vim sources/demo.cpp
Yp3wct>cstdlib<ESC>
/while<CR>ostd::string log_path = std::getenv("LOG_PATH");<ESC>
/"log<CR>
cf"log_path<ESC>
k2dd2kpVj<
:wq
pushd $HUNTER_ROOT
git config --global hub.protocol https
git fork
git branch -u ${GITHUB_USERNAME}/master master
...
git release create -m"${HUNTER_VERSION}.1" ${HUNTER_VERSION}.1
git release show ${HUNTER_VERSION}.1
wget https://github.com/${GITHUB_USERNAME}/hunter/archive/${HUNTER_VERSION}.1.tar.gz
export MYHUNTER_SHA1=`openssl sha1 ${HUNTER_VERSION}.1.tar.gz | cut -d'=' -f2 | cut -c2-41`
echo $MYHUNTER_SHA1
rm -rf ${HUNTER_VERSION}.1.tar.gz
popd
echo $MYHUNTER_SHA1 | pbcopy
wim CMakeLists.txt
/SHA1<CR>
wc2w<C-V><ESC>
:wq
vim README.md
/lab11<CR>
e<C-A>
ne<C-A>
:wq
git add .
git commit -m"refactoring"
git push origin master
travis login --auto
travis enable

```
-  Результаты выполнения команд

![](https://github.com/Nikita7181/lab12/blob/master/Screenshots/1.png?raw=true) 
 
![](https://github.com/Nikita7181/lab12/blob/master/Screenshots/2.png?raw=true)

![](https://github.com/Nikita7181/lab12/blob/master/Screenshots/3.png?raw=true)

![](https://github.com/Nikita7181/lab12/blob/master/Screenshots/4.png?raw=true)

![](https://github.com/Nikita7181/lab12/blob/master/Screenshots/5.png?raw=true)

- После чего все было выгружено на Git hub

```
cd /home/nikita/Nikita7181/workspace/projects/lab12
git add .
git commit -m "Complete tasks"
git push origin master
```
