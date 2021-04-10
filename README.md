# MyReversiApp

## 設定

### Django

##### Pythonのインストール
Python 3.9.2  
https://www.python.org/downloads/

##### Djangoのインストール
```
$ pip install django
```

##### serverプロジェクトの作成
```
$ cd (略)\MyReversiApp
$ django-admin startproject server
```

##### MyReversiServerアプリの作成
```
$ cd server
$ django-admin startapp MyReversiServer
```

### Vue.js

##### Vue.jsのインストール
vue CLI v4.5.12  
https://jp.vuejs.org/v2/guide/installation.html

##### clientプロジェクトの作成
```
$ cd (略)\MyReversiApp
$ vue create client
 <options>
  Please pick a preset: Manually select features
  Check the features needed for your project: Choose Vue version, Babel, Router, Vuex, Linter
  Choose a version of Vue.js that you want to start the project with 2.x
  Use history mode for router? (Requires proper server setup for index fallback in production) No
  Pick a linter / formatter config: Basic
  Pick additional lint features: Lint on save
  Where do you prefer placing config for Babel, ESLint, etc.? In dedicated config files
  Save this as a preset for future projects? No
```

#### パッケージの追加
```
$ cd client
$ vue add vuetify
 <options>
  Choose a preset: Default (recommended)
$ npm install --save axios sweetalert2 vue-session
```

## 実行

### server(Django)
```
$ cd (略)\MyReversiApp\server
$ python manage.py runserver
```
http://127.0.0.1:8000/

### client(Vue.js)
```
$ cd (略)\MyReversiApp\client
$ npm run serve
```
http://localhost:8080/
