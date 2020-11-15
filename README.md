### 文章创建

* 创建文章

  ```bash
  hugo new post//index.md
  ```

* 启动hugo

  ```bash
  hugo server --theme=beautifulhugo --buildDrafts
  ```

* 生成静态文章

  ```bash
  hugo -d docs
  ```


### 更换电脑导致docs子项目无法提交

删除子模块，步骤如下：

1. `rm -rf 子模块目录` 删除子模块目录及源码

2. `vi .gitmodules` 删除项目目录下.gitmodules文件中子模块相关条目

3. `vi .git/config` 删除配置项中子模块相关条目

4. `rm -rf .git/modules/*` 删除模块下的子模块目录，每个子模块对应一个目录，注意只删除对应的子模块目录即可

5. git add .  

6. git commit -m '子库修改日志'

7. 执行完成后，再执行添加子模块命令即可，如果仍然报错，执行如下：

   ```
   git rm --cached 子模块名称
   ```

   完成删除后，提交到仓库即可

