# Nitendo 游戏折扣数据爬虫 

> :video_game: 任天堂游戏在各国家的最新折扣,Get Nitendo game discounts for spiders.

Jump小程序和Savecoins网站的游戏折扣信息

## 爬虫介绍
* jump
* savecoins

## 目录

* [环境安装](#环境安装)
* [启动运行](#启动运行)

## 环境安装
1. 下载安装Python3.5或以上版本
2. 安装Mysql数据库并执行[game.sql](game.sql)脚本初始化数据库表.
3. 在`DG/`目录下[pipelines.py](DG/pipelines.py)文件中修改数据库链接信息.
```python

    config = {
        'user': 'username', 
        'password': 'pwd', 
        'host': 'host',
        'database': 'db',
        'charset':'utf8mb4'
    }

```
3. 在项目根目录执行命令,安装依赖.
```bash
pip install -r requirements.txt
```

## 启动运行

执行 `run.sh`,启动爬虫.

```bash
chmod +x ./run.sh && ./run.sh
``` 

## Maintainers
[@yangb92](https://github.com/yangb92)

## License
© 2020 杨斌 :frog:
