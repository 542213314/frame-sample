# frame-sample
//2019-09-23
基于go-mega-master修改的web框架


修改点注意:
//关于模板添加
经修改,可在template文件夹下自定义多个文件夹进行模板分类
1.模板添加在template根目录下的自定义文件夹中，例：template/content/index.html。
2.目前模板只识别template目录下的一级文件夹.html文件


//2019-09-25
新增
1.静态资源目录配置
2.日志输出文件 生成目录 /run/

//2019-09-26
新增
1.文件监控
    可配置 config.yml 配置项 server.watch_path 后追加虚监控的目录或者文件
    执行方式: 1. go build 生成可执行文件 2. 运行可执行文件 ./server -auto=true  注:运行可执行文件后/run/目录下生成server.pid来记录进程
2.端口、日志、进程、监控文件路径可配置
    config.yml下
    server.port:       端口配置
    server.log:        日志配置
    server.pid:        进程配置
    server.watch_path: 端口配置
