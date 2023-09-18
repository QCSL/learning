# vpn
1. [百度网盘链接提取码:96b2](https://wwrx.lanzoum.com/icTU70uuwe5c)
2. 从该网址下载安装包进行解压，把warp安装上
3. 打开手动2，输入ip：188.114.96.179:8319，替换ip，之后就可以进行翻墙

之后可以下载谷歌浏览器，注册一个谷歌邮箱账号，
[一个GPT网址](https://poe.com/ChatGPT)


# 安装虚拟机和ubuntu os系统
1. Windows环境下安装VirtualBox最新版本，找自己是什么电脑比如windows [ 安装VirtualBox链接](https://www.oracle.com/jp/virtualization/technologies/vm/downloads/virtualbox-downloads.html)
2. 下载 ubuntu20.04 ios 镜像文件 Desktop image [下载ubuntu20.04链接](https://releases.ubuntu.com/focal/)
3. 按照配置指南 安装ubuntu os （内存4GB以上，最好选择English 语言， 中文今后命令操作会很麻烦。 密码简单一点比较好比如1234， 最好不使用特殊字符）[参考blog](https://blog.csdn.net/qq_45373920/article/details/122409002)
4. 进入ubuntu系统在程序里 找到终端（terminal）打开,执行如下命令 `sudo apt update`和`sudo apt upgrade`
5. 然后安装 pyenv， python3 ，pip3，git，pandas，scikit-learn，matplotlib，jupyter， 等命令群
```
老师的方法：
###### git安装如下
      `sudo apt install git`

   ###### pip3 安装如下
      `sudo apt install python3-pip`

   ###### pyenv 安装方法看 手册 
      [参考pyenv安装手册]（https://github.com/pyenv/pyenv/wiki）

   ###### 然后在pyenv环境下安装python3
      比如执行如下命令
        `pyenv install --list`
      然后选你想安装的版本
        `pyenv install 3.9.1`
        `pyenv global 3.9.1`
        `pyenv rehash`

   ###### pandas，scikit-learn，matplotlib的话
      pip3 install pandas scikit-learn matplotlib

   ###### jupyter 安装看官网指南
      [参考jupyter官方安装说明]（https://jupyter.org/）
```

```
conda方法：
###### git安装如下
      `sudo apt install git`

######
`cd`#进去主目录
`mkdir anaconda`#创建anaconda文件夹
`cd anaconda`#进入anaconda文件夹
`wget https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/Anaconda3-5.3.1-Linux-x86_64.sh`#下载anaconda
`bash Anaconda3-5.3.1-Linux-x86_64.sh`然后一直点确定就行#类似解压文件
`conda update conda`#更新conda
`conda create -n python39 python=3.9`#创建python3.9，环境名字为python39
`source activate python39`#激活环境
`pip install install pandas scikit-learn matplotlib numpys jupyterlab`#安装各种包
`jupyterlab`打开jupyterlab
 
```
6. 打开之后建立新的文本 测试如下代码
```
       import matplotlib.pyplot as plt

       fig, ax = plt.subplots()

       fruits = ['apple', 'blueberry', 'cherry', 'orange']
       counts = [40, 100, 30, 55]
       bar_labels = ['red', 'blue', '_red', 'orange']
       bar_colors = ['tab:red', 'tab:blue', 'tab:red', 'tab:orange']

       ax.bar(fruits, counts, label=bar_labels, color=bar_colors)

       ax.set_ylabel('fruit supply')
       ax.set_title('Fruit supply by kind and color')
       ax.legend(title='Fruit color')

       plt.show()
```    
效果图如下
[Image and Code](https://matplotlib.org/stable/gallery/lines_bars_and_markers/bar_colors.html#sphx-glr-gallery-lines-bars-and-markers-bar-colors-py)



