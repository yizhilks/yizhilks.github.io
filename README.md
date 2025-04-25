git bash here
首先获取秘钥
在git中输入ssh-keygen -t rsa -C "你的邮箱"
按2-3次空格直到图形输出，接着输入 clip < ~/.ssh/id_rsa.pub获取秘钥，并复制
打开github创建一个仓库，名称输入（你的github用户名.github.io）
勾选readme文件，并在设置中添加ssh秘钥
打开blog根目录文件——config.yml

  type: 'git'
  repository: 你的ssh地址
  branch: master
  打开git窗口
  git config --global user.email "你的github邮箱"
  git config --global user.name "你的github用户名"

hexo g生成网页
hexo d部署网页
