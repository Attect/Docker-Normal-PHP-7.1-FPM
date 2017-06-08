# Docker-Normal-PHP-7.1-FPM
基于官方的包含常用库的php7-fpm的 Dockerfile
> https://github.com/docker-library/php/tree/c48c629568bc166b58b271114d0b44ea6d5cfa09/7.1/fpm

## 说明
初入Docker发现官方image缺少许多常用库,为了自己项目能运行对其进行了一些补充.
基本解决了数据库以及验证码和图形处理方面的依赖.
但对Docker掌握不深,如果有更好的解决方案欢迎提出.

## 增加的依赖
1.  **libgd3**
1.  **libjpeg-dev**
1.  **libpng-dev**
1.  **libwebp-dev**
1.  **libfreetype6-dev**

## 增加的编译配置
1. **--with-pdo-myql**
1. **--with-mysqli**
1. **--with-gd**
1. **--with-freetype-dir=/usr**
1. **--enable-gd-native-ttf**
1. **--enable-gd-jis-conv-ttf**