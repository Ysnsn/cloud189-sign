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
添加名为**USER**、**PWD**、**SCKEY**(可选)的变量  
值分别为**账号**、**密码**、**Server酱的KEY**  
多账号时账号密码一行一个一一对应  
示例：  
**USER**
```
123456
24678
```
**PWD**
```
cxkjntm
jntmcxk
```
**SCKEY**  
KEY获取方法详见官网：https://sc.ftqq.com
```
xxxxxxxx
```
![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)
![](http://tu.yaohuo.me/imgs/2020/06/af2013b1ef5d8430.png)
![](http://tu.yaohuo.me/imgs/2020/06/09c22adcec7b5d81.png)


## 三、启用Action
1 点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
2 修改任意文件后提交一次  
![](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)

## 四、查看运行结果
Actions > Cloud189Checkin > build  
能看到如下图所示，表示成功  
![](http://tu.yaohuo.me/imgs/2020/06/b9e596c99f3835e0.png)

此后，将会在每天10:00-10:45之间和22:00-22:45之间各需求，可以在[.github/workflows/run.yml]中自行修改

## 可能遇到的问题
- 1. 验证码错误  
首先考虑是不是密码错误  
其次查看是否已经关闭设备锁  
- 2. 暂无


