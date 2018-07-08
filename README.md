en.pokmen.cn-2018
=============

博敏工业设备英文官网2018年版


域名绑定及nginx配置
-----

新建配置文件: ``sudo nano /etc/nginx/sites-available/pokmen.cn``

编辑配置文件及保存: 

    server {
        server_name en.pokmen.cn;
        index index.html;
        root /srv/en.pokmen.cn-2018/_site;
        error_page 404 /Error.html;
    }

建立链接: ``sudo ln -s /etc/nginx/sites-available/pokmen.cn /etc/nginx/sites-enabled/``

重启nginx: ``sudo service nginx restart``


下载及生成网站
-----

1. 下载网站源码: ``git clone git://github.com/zackwong/pokmen.cn-2018.git``

2. 进入源码根目录: ``cd pokmen.cn-2018``

3. 生成网站: ``jekyll build``


开发者
---------

* Zack Wong &lt;hzzzoo@126.com&gt;
