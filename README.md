### 部署步骤
每次部署的步骤，可按以下三步来进行。
``` bash
hexo clean
hexo generate
hexo deploy
```

###一些常用命令：
``` bash
hexo new "postName" #新建文章
hexo new page "pageName" #新建页面
hexo generate #生成静态页面至public目录
hexo server #开启预览访问端口（默认端口4000，'ctrl + c'关闭server）
hexo deploy #将.deploy目录部署到GitHub
hexo help  # 查看帮助
hexo version  #查看Hexo的版本
```


### 报错总结   

#### ERROR Deployer not found: git 或者 ERROR Deployer not found: github
* **解决方法** ： npm install hexo-deployer-git  --save

####如发生报错： ERROR Process failed: layout/.DS_Store, 那么进入主题里面layout和_partial目录下，使用删除命令：

``` bash
rm -rf .DS_Store
