### FORK FROM 甬哥 未做任何更改
系统如果没有curl
方法一
```
apt-get install curl
```
如安装curl程序可能会出现命令无效，请继续往下看
方法一：
出现安装错误，看了很多资料，都是建议建议先做
```
apt-get update
```
但是执行了，还是不行，试试先安装如下命令
```
apt-get install sudo
```
执行了这个之后在执行安装curl就能正常安装了
方法二：
还有一个方法就是先执行
```
dpkg –configure -a
```
然后在执行
```
apt-get install curl
```
就可以正常安装了
特么提醒：
运用以上方法如果提示依赖包没有安装，可以用如下命令安装
```
sudo apt-get install -f
```
另附命令

ubuntu/debian 系统安装方法: 
```
apt-get update -y && apt-get install curl -y
```
centos 系统安装方法: 
```
yum update -y && yum install curl -y
```
### x-ui修改版一键脚本（xray内核）

### 支持纯IPV4、纯IPV6的VPS直接安装，主流linux系统均支持

### 相关说明及注意点请查看[博客说明](https://ygkkk.blogspot.com/2023/05/reality-xui-chatgpt.html)、[更新日志及配置](https://ygkkk.blogspot.com/2022/02/x-ui-yg.html)
### 一键脚本：
```
bash <(wget -qO- https://gitlab.com/rwkgyg/x-ui-yg/raw/main/install.sh 2> /dev/null)
```
或
```
bash <(curl -Ls https://gitlab.com/rwkgyg/x-ui-yg/raw/main/install.sh)
```

![ce8002bc4949ddb34786a749ce58b81](https://user-images.githubusercontent.com/121604513/236723333-fb657028-b985-4157-afd1-c92843764d1d.png)

### 脚本源码备份[Gitlab地址](https://gitlab.com/rwkgyg/x-ui-yg)
### 参考项目[vaxilu](https://github.com/vaxilu/x-ui)，[FranzKafkaYu](https://github.com/FranzKafkaYu/x-ui)，[MHSanaei](https://github.com/MHSanaei/3x-ui)，[qist](https://github.com/qist/xray-ui)

