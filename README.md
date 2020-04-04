# filebrowser
Filebrowser 一键安装脚本  
来自：https://github.com/233boy/filebrowser

filebrowser.json说明：  
port: 9184, 监听的端口  
baseURL: 端口后显示为此+/files, 可留空  
address: ,  
log: stdout,  
database: /etc/filebrowser/database.db, 数据库的路径  
root: /usr/local/caddy/www/file, 可管理的目录

当caddy采用proxy时，baseURL、proxy的url目录需相同，或都为空，不然会进不去，一直3个圆圈的进度条

每次安装都会重置配置文件，但不会重置数据库，安装2.0.15以后的版本存在刷新后打不开
