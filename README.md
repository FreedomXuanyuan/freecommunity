# 自由bbs论坛项目
## springboot项目
### 项目上传第一周
### 类似 https://elasticsearch.cn/ 中文社区
### spring模块 https://spring.io/guides
#### git命令 git add . #将文件放入暂存
#### git命令 git status #查看当前状态
#### git命令 git commit -m "add readme" #添加新的分支添加备注
#### git命令 git commit --amend --no-edit #追加更改不需要修改目录
###### git bush 上传代码
#### 上传代码时出现 ”Could not create directory '/c/Users/\351\“的问题时需要配置环境变量。系统环境变量中修改HOME环境变量（没有的就自己添加），修改成c:\Users\<username>，其中<username>整体替换成你当前用户所对应的名字。
#### 然后重新启动开发环境或者git bash 重新push代码
## 使用的组件或者工具
##### https://v3.bootcss.com/ bootstrap
[GitHub API 用户授权 OAuth](https://docs.github.com/en/developers/apps/building-oauth-apps/creating-an-oauth-app)

[绘图工具 visual paradigm](https://www.visual-paradigm.com/cn/)

## 快捷键
使用shift+Enter直接创建新的一行
ctrl+e 快速切换标签页

## 解决accesstoken 安全令牌的相关问题  
"message": "Must specify access token via Authorization header. ”
Request request = new Request.Builder()
.url("https://api.github.com/user")
.header("Authorization","token "+accessToken)
.build();
