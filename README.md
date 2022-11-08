# hosts

Raw Url: https://raw.githubusercontent.com/uwang/myhosts/develop/home.txt   
CDN Url: https://gcore.jsdelivr.net/gh/uwang/myhosts@develop/home.txt   
CDN Url: https://fastly.jsdelivr.net/gh/uwang/myhosts@develop/home.txt  
CDN Url: https://cdn.staticaly.com/gh/uwang/myhosts/develop/home.txt (推荐) 

cdn.jsdelivr.net 被污染了，幸运的是，fastly.jsdelivr.net 还可以正常访问

刷新缓存：https://purge.jsdelivr.net/gh/uwang/myhosts@develop/home.txt

## Used

### Windows/MacOS

推荐使用 SwitchHosts https://github.com/oldj/SwitchHosts/releases

![image](https://user-images.githubusercontent.com/5615843/187586697-201b444c-1a3b-486a-867d-5fff9e63a4b2.png)

### Linux

```bash
# 删除
sudo sed -i '/# Uwang Hosts Start/,/# Uwang Hosts End/d' /etc/hosts
# 添加
curl -s -k -L https://cdn.staticaly.com/gh/uwang/myhosts/develop/home.txt | sudo tee -a /etc/hosts
```
