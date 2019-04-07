# vsCode安装使用教程和插件安装

### 1、下载地址

<https://code.visualstudio.com/Download>



### 2、若想改语言成中文

ctrl+shift+p

输入 Configure Display Language

设置 zh-cn 关闭软件重启



### 3、vsCode常用命令说明

![å¨è¿éæå¥å¾çæè¿°](https://img-blog.csdnimg.cn/20181125171832749.png)



### 4、前端常用插件

###### （1）自带的格式化：

- On Windows Shift + Alt + F
- On Mac Shift + Option + F
- On Ubuntu Ctrl + Shift + I

###### （2）eslint风格格式化：

下载插件

点击 VS Code 的 **文件 > 首选项 > 设置**，打开setting.json，添加：

```json
    "eslint.autoFixOnSave": true,
    "eslint.validate": [
      "javascript",
      "javascriptreact",
      {
        "language": "html",
        "autoFix": true
      },
      {
        "language": "vue",
        "autoFix": true
      }
     ],
```

eslint.autoFixOnSave 用来进行保存时自动格式化，但是默认只支持 javascript .js 文件。

eslint.validate 用来配置作用的文件类型。

然后在保存代码的时候，就会自动格式化为eslint风格（需要保存多次）。

###### （3）HTML格式化代码缩进

下载插件Vetur

点击 VS Code 的 **文件 > 首选项 > 设置**，打开setting.json，添加：

```json
    "vetur.format.defaultFormatterOptions": {
        "prettyhtml": {
          "printWidth": 160
        },
        "prettier": {
          "singleQuote": true,
          "proseWrap": "never",
          "printWidth": 130
        }
      },
```

###### （4）其他插件

![1554626574924](C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\1554626574924.png)



### 5、网页代码实时预览

安装Live Server插件