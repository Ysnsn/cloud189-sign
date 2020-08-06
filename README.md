# 紧急通知

**6月23日(含)** 之前部署的老代码存在泄露账号密码的风险，已部署的童鞋赶紧处理一下！

泄露原因：```.github/workflows/run.yml``` 代码中有打印输出账号和密码，**只要登陆Github的用户，都可以访问你仓库的Actions中的build内容**！

目前我只知道这俩个仓库存在该风险！

```malaohu/Cloud189Checkin-Actions```
```peng4740/Cloud189Checkin-Actions```

处理方案：由于Github Action 还不支持删除 Workflows 以及 build结果！只能以下操作！

1）删除你的仓库（仓库 -> Settings -> Delete this repository），然后重新部署自动签到（只有这样才能清理掉build所有记录）！

2）赶紧修改天翼云盘的密码！


更多内容：[https://51.ruyo.net/16050.html](https://51.ruyo.net/16050.html)

有人说没事儿没人发现我部署的仓库！ Github仓库每个fork都有记录(点击右上角的fork数量), 任何人可看！小心被人利用！

部署的私有仓库，或者非21-23号部署的仓库应该没影响！


# Cloud189Checkin
天翼云盘每日签到一次，抽奖2次  
使用方法  
1.测试环境为python3.7.6,自行安装python3  
2.requirements.txt 是所需第三方模块，执行 `pip install -r requirements.txt` 安装模块  
3.可在脚本内直接填写账号密码  
4.Python 和需要模块都装好了直接在目录 cmd 运行所要运行的脚本。  

登录看的以下项目：
> [Cloud189](https://github.com/Dawnnnnnn/Cloud189)
> [cloud189](https://github.com/Aruelius/cloud189)

# Github Actions说明
## 一、Fork此仓库
![](http://tu.yaohuo.me/imgs/2020/06/f059fe73afb4ef5f.png)
## 二、设置账号密码
添加名为**USER**、**PWD**的变量  
值分别为**账号**、**密码**  
支持多账号，账号之间与密码之间用**半角逗号**分隔，账号于密码的个数要对应  
示例：**USER:123456,24678**，**PWD:cxkjntm,jntmcxk**
![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)

## 三、启用Action
1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
2 修改任意文件后提交一次  
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)

## 四、查看运行结果
Actions > Cloud189Checkin > build  
能看到如下图所示，表示成功  
![](http://tu.yaohuo.me/imgs/2020/06/b9e596c99f3835e0.png)

此后，将会在每天10:00和22:00各签到一次  
若有需求，可以在[.github/workflows/run.yml]中自行修改
