# 来源
https://ssr.tools/700
https://www.moerats.com/archives/571/
https://www.j000e.com/Nextcloud/cloud-drive-direct-sharelink.html
# 下载
wget --no-check-certificate -qO /usr/local/bin/gdlink 'https://www.moerats.com/usr/shell/gdlink.sh' && chmod a+x /usr/local/bin/gdlink
# 使用
```
#Work with share link/使用分享链接方式
gdlink 'https://drive.google.com/open?id=0B8SvBXZ3I5QMcUduTMJEanRkMzQ'

#Work with file id/使用文件ID方式
gdlink '0B8SvBXZ3I5QMcUduTMJEanRkMzQ'

#download with share link/使用分享链接方式直接使用wget下载链接
##可将其中./download改成自己需要的文件名或文件绝对路径
gdlink 'https://drive.google.com/open?id=0B8SvBXZ3I5QMcUduTMJEanRkMzQ' |xargs -n1 wget -c -O ./download
```