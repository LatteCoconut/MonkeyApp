# MonkeyApp
monkey app - 在Mac状态栏显示蓝队吗喽们的下班倒计时
![Alt](img/0.jpg)
<img src="img/0.gif" width="920">
### 实时倒计时
在状态栏显示下班倒计时

### 摸鱼百分比
在状态栏实时显示当前已上班时间百分比

### 摸鱼收入
在状态栏实时显示当天已获得的摸鱼收入，看着每秒增加的收入封起 IP 来更有动力！！！

# 怎样使用
## 1. 安装第三方模块
### rumps

```bash
pip3 install rumps
```

rumps 是一个 Python 模块，用于创建 Mac OS X 应用程序。它提供了一个简单的方式来创建带有菜单栏图标的应用程序，这些应用程序可以执行各种任务，比如显示通知、执行系统命令等。Rumps 特别适合快速开发小型的桌面应用程序，特别是那些需要在后台运行并提供菜单栏访问的应用程序。

## 2. 设置相关参数
在monkey.py中第17行修改你实际的上下班时间(必须)和你的日薪(非必须)：
```python
CONFIG = {
    'start_time': '08:20',  # 你的上班时间
    'end_time': '16:30',  # 你的下班时间
    'wage': 1000,  # 你的日薪，不为0时可以实时显示当天已摸多少元子
    'percent': True,  # 是否显示已摸鱼时间百分比，为False时不限时百分比
}
```

## 3. 开始运行
```bash
python3 monkey.py &
```
![alt](img/1.jpg)

开始运行后即可获得一个位于Mac状态栏的倒计时程序

<video width="320" height="240" controls>
  <source src="img/1.mp4" type="video/mp4">
</video>

## 4. 怎样退出
单击状态栏倒计时区域即可退出
![Alt](img/2.jpg)
