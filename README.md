

![1624762654518](./kyouka.jpg)

##### atr:[結月とば_](https://space.bilibili.com/8799104)

# 京华破防站[Kyouka-Button]🔨

[[EN](https://github.com/YYRDIO/Kyouka-button/blob/main/README-EN.md)/[日本语](https://github.com/YYRDIO/Kyouka-button/blob/main/README-JA.md)/中文]

------

我们拥有所有按钮站都没有的功能，那就是--------

#### **让主播破防**

------

### 本项目于2021年4月重启！

------



### 项目参与

​	通过fork项目使用git克隆项目

​	提交分支main

​	你需要更改的文件如下

​	[语音项目增加]：`setting\translate\01_voices.json`

​	[列表增加]：`setting\translate\category.json`

​	[音频存放路径]：`public\voices`

​	[图片存放路径]：`public\voices\img`

<br/>

  如果你需要测试，请保证你的环境里安装了nodejs和npm后
  在项目路径内输入`npm install`

  （国内地区如果下载速度过慢可使用cnpm，但使用方法`npm install -g cnpm` `cnpm install`）
  
  测试运行`npm run serve`

<br/>

​	`01_voices.json`解析如下

```json
{
    "name": "赢了", //可以填写音频文件名，但是不能出现重复值！！！
    "path": "赢了.mp3", //这里为音频文件名称，直接填写public\voices的音频文件即可(注意，是mp3格式哦)
    "date": "2020-02-15", //填写更新日期即可
    "translate": { //
      "zh-CN": "赢了，赢了，赢了！！！", //按钮文字，这里填写中文名称即可
      "en-US": "Kyouka Bible" //同上，填写按钮的英语名称！
    },
    "usePicture": { 
      "zh-CN": "", //这里是表情包的文件名称，填写public\voices\img的图片名称即可
      "en-US": ""  //同上
    },
    "category": "圣经", //该字段绑定category.json列表的name字段
    "mark": { //下面的三个分别填写视频名称'title'、所处时间段'time'、链接地址'url'
      "title": "【哭了】张京华被绿了？谁是泠鸢呢？【完全胜利ED】",
      "time": "",
      "url": "https://www.bilibili.com/video/BV1z7411J7c2"
    }
}
```

`category.json解析如下`

```json
{
    "name": "圣经", //标签名，不可重复
    "translate": {
      "zh-CN": "京 典 名 场 面",  //列表名称
      "en-US": "Kyouka famous scene"   //英语列表名称
    }
```

当然，如果你不会可以通过[这里](https://github.com/Timolop233/Kyouka-button/issues/17)提交你知道的怪话，我们会更新的。

------

### LICENSE
- 使用[voices-button-cli](https://github.com/blacktunes/voices-button-cli)创建的语音按钮
- 所用模板为[Hiiro按钮](https://github.com/blacktunes/hiiro-button)