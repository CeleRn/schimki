Сайт для сервисного центра по адресу schimki.ru
Бекэнд реализован на Odoo. 

Фронтэнд - приложение c SSR.
На фронтэенде используются:
- TypeScript
- React.js
- Redux
- Redux-saga
- Material UI
- CSS-in-JS

SSR реализован на koa.js

Общие правила установки:
```
mkdir ~/projects/schimki/log
mkdir ~/projects/schimki/log/nginx
mkdir ~/projects/schimki/log/odoo
mkdir ~/projects/schimki/log/koa
mkdir ~/projects/schimki/cache
```


Установка Бэкэнда:

```
sudo apt-get install build-essential autoconf libtool pkg-config python-opengl python-pil python-pyrex idle-python2.7 qt4-dev-tools qt4-designer libqtgui4 libqtcore4 libqt4-xml libqt4-test libqt4-script libqt4-network libqt4-dbus python-qt4 python-qt4-gl libgle3 python-dev libssl-dev libsasl2-dev libldap2-dev

git clone --branch 14.0 --single-branch --depth 1 git@github.com:odoo/odoo.git backend/odoo_server

virtualenv --python=python3 ~/projects/schimki/backend/venv
. ~/projects/schimki/backend/venv/bin/activate
pip install -r ./backend/odoo_server/requirements.txt
```

Установка Фронтэнда
```
cd ~/projects/schimki/frontend

```