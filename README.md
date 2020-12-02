
# 通过Actions每天获取听歌记录展示在主页的README.md🎧 

### 成品样子 [sohyunQVQ](https://github.com/sohyunQVQ/sohyunQVQ)
<p align="center">
  <img src="https://github.com/sohyunQVQ/netease-music-show/blob/main/images/1.png" width="758">
</p>

### 准备

1. 克隆我原本的仓库 `git clone https://github.com/sohyunQVQ/sohyunQVQ`

2. 去拿到你的网易云UID(可以在https://music.163.com通过搜索用户进入拿到)

<p align="left">
  <img src="https://github.com/sohyunQVQ/netease-music-show/blob/main/images/2.png">
</p>

3. 修改`.github/workflows/job-work.yml`，将36行内的`136164194`修改成你的uid 

4. 修改仓库名以及remote的地址(或者你新建好自己的仓库 将原本的文件拉取过来) 并push到你的repo

### 

## 操作说明

- 使用的编码代码是由[wyy-action](https://github.com/t00t00-crypto/wyy-action) 编写
- Github Actions执行时间为标准时区 所以脚本的`0 8 * * *`是每天北京时间0点执行
- 可以通过对项目的`star`进行手动执行

## 可能出现的问题

- Action在执行python脚本时报错
  
  1.检查隐私权限是否听歌排行所有人可见
<p align="left">
  <img src="https://github.com/sohyunQVQ/netease-music-show/blob/main/images/3.jpg">
</p>
  2.打开自己的主页看是否有数据

  3.UID是否错误

- Action在push的过程出错

  1.README.md没有变动所以push失败 （正常情况）

  2.没有修改yaml内的git config