这个md文件我将带你一步一步修改此网站
如想获取完整的源代码，请加我QQ 2776980336
第一步安装git和node.js
安装完成后打开amd终端，输入node -v和npm -v。如果没报错，则安装成功
访问hexo博客官网，并新建文件夹命名为hexo，右键鼠标，点击git bash here，以此输入hexo下5行代码（一般不会报错）
你就会看到你的网站的地址，好的，你已经拥有了一个个人博客，请安装sublime，你可以使用md语法进行编辑或使用HTML或使用主题包


你已经编辑完成了，接下来我将带你配置服务器，你可以使用gitee（较为推荐）
下面我将带你使用github进行上传
首先获取秘钥
在git中输入ssh-keygen -t rsa -C "你的邮箱"
按2-3次空格直到图形输出，接着输入 clip < ~/.ssh/id_rsa.pub获取秘钥，并复制
打开github创建一个仓库，名称输入（你的github用户名.github.io）
勾选readme文件，并在设置中添加ssh秘钥
打开blog根目录文件——config.yml
在最后输入
  type: 'git'
  repository: 你的ssh地址
  branch: master
  打开git窗口，输入
  git config --global user.email "你的github邮箱"
  git config --global user.name "你的github用户名"
接着输入
hexo g生成网页
hexo d部署网页

你可以在设置里面看到你的网站地址，供大家访问
过程中会遇到超多报错，欢迎私信我
