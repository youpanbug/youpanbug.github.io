#使用"Nextcloud"搭建云盘

## Nextcloud一建安装:<https://github.com/nextcloud/nextcloud-snap>

建议安装Ubuntu系统,因为官方一键安装包用的是Snap,CentOS还不支持

    $ sudo apt-get update
    $ sudo apt-get install snap
    $ sudo apt-get install snapd
    $ sudo snap install nextcloud

(这时候你可以用服务器IP访问了.如果你想用域名访问,指向这个IP就可以,用域名访问的时候Nextcloud就会询问你是否绑定这个域名)

## 注意

(这时候可以正常使用云盘,不绑定域名也可正常使用)

## 启用SSL,使用HTTPS访问

    $ sudo nextcloud.enable-https lets-encrypt

(系统就会自动申请let's Encrypt证书并启用)

## 以后升级

    $ sudo snap refresh nextcloud