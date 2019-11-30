# 怎样恢复开发环境

可以使用 [hexo容器化开发环境](https://github.com/fanxingzju/docker-development-environment/tree/master/hexo),这样就不用每次重装hexo.  
接下来通过如下命令恢复开发环境.

```bash
git clone https://github.com/fanxingzju/hexo-blog.git
cd hexo-blog
# 克隆子仓库（这里指themes目录）的文件
git submodule update --init --recursive
npm install
# 重新生成静态文件
hexo generate
# 验证
hexo server
```
