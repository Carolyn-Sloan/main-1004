# ⏰ 自动获取订阅链接

## 🚀 每三天更新一次

- clash订阅链接：`
- CDN加速链接：`

- v2ray订阅链接：



## Fork之后需要修改的一些地方

### 基本设置
1. 首先是右上角头像下拉，点击Settings->Developer settings->Generate new Token
![](https://raw.githubusercontent.com/vveg26/ImageHosting/master/BlogImg/202209071853387.png)
![](https://raw.githubusercontent.com/vveg26/ImageHosting/master/BlogImg/202209071851304.jpg)
2. 生成一个可以读写仓库的新token,复制Token
3. 点击仓库->Setting->Actions->new repostoiry secrets
![](https://raw.githubusercontent.com/vveg26/ImageHosting/master/BlogImg/202209071854965.png)

4. name写TOKEN secrets写刚刚复制的Token
![](https://raw.githubusercontent.com/vveg26/ImageHosting/master/BlogImg/202209071855328.png)
### workflow中的设置
首先的首先，先去Action中开启

1. 首先第一个“更新项目”需要你的项目有Starts和Forks，不然就会报错，不过报错也不影响
2. 更改workflow中的各个yaml中的配置文件,找到下方代码，更改为自己的用户名和邮箱
        ```
        git config --global user.name "vveg26" 
        git config --global user.email vveg26@gmail.com ```
3. 之后重新运行一遍三个action，就可以成功了      
        
### 更改时间       
自己去搜cron表达式，去修改时间
