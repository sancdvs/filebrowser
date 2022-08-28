# filebrowser
Filebrowser 一键安装脚本  
来自：https://github.com/233boy/filebrowser

filebrowser.json说明：  
port: 9184, 监听的端口  
baseURL: 端口后显示为此+/files, 可留空  
address: ,  
log: stdout,  
database: /etc/filebrowser/database.db, 数据库的路径  
root: /, 默认管理的目录

当caddy采用proxy代理filebrowser时，baseURL、proxy的url目录（caddy网址斜杠后面的目录加proxy后的目录）需相同，或都为空，或单proxy的url目录为空，不然会进不去，一直3个圆圈的进度条

安装：wget -N --no-check-certificate https://raw.githubusercontent.com/sancdvs/filebrowser/master/filebrowser.sh && chmod +x filebrowser.sh && bash filebrowser.sh
