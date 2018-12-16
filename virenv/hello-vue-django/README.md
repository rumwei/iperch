# hello-vue + Django

This is a boilerplate project for using vuejs with Django.

### 中文详细教程
[Django + Vue 单页面应用的开发环境搭建步骤](http://www.jianshu.com/p/fe74907e16b9)

### Features
* Django backend in `./backend`
* vuejs (v2) frontend in `./frontend`
* Hot-reload with vue-loader
* eslint linter integration
* Makefile to make your life easy


### Development environment setup

These steps will install all required dependencies including development ones, run migrations and start dev server.

```bash
make dev
make migrate
make run
```

### Deployment

These steps will install productio dependencies and build vuejs application to `static/dist` folder.

```bash
make prod
make build
```

### Be aware

For the sake of simplicity Django config is contained within it's own backend app. In real world setting you would
probably want to remove `backend` from `INSTALLED_APPS`, create a new app and move `backend.views` to it.

You probably want to create python virtual environment as well. Default python instance available will be used.
