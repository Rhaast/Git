
## Git上传步骤以及常用指令

* 1、建立一个本地文件夹，打开Git，通过cd 文件夹名的方式进入文件夹内部
* 2、在Github上新建一个存储仓库，打开并通过git clone + 克隆地址，将仓库克隆到本地。
* 3、把需要上传的文件拖拽到本地文件夹并在git里通过git status指令查看所添加的文件。
* 4、通过git add -A的指令将所有本地文件添加到云端（注：此时并未添加到上传到Github上），此后本地每新增一个文件都必须通过git add 文件名的方式添加到云端（删除的文件也是如此）。
* 5、通过git commit -m"需要描述的文字"指令添加对文件的描述。（注：单独为新增文件添加描述的方式为git commit -m"需要添加的描述"）。
* 6、最后通过git push origin master的指令，将需要上传的文件上传到Github主分支。
* 7、将Github上的更改同步到本地文件夹的方式则是通过git pull origin master的指令。（注：若是Github上的内容有所变更，最好是先同步到本地了再执行其他的操作，以免发生冲突）。
* 8、cd..指令用于返回文件路径的上一步。
* 9、在一台计算机上才安装git并建立新的工程提交文件时可能会出现"Please tell me who you are. Run" ，这个时候可以看看一下git环境是否配置：
  * ①.git init
  * ②.git config user.name "someone"
  * ③.git config user.email "someone@someplace.com"
  * ④.git add *
  * ⑤.git commit -m "some init msg"。
   
   特别注意2、3条的顺序。
* 10、其他相关指令链接http://www.cnblogs.com/springbarley/archive/2012/11/03/2752984.html
* 11、利用node.js+git安装atom插件：
  * ①.下载并安装node.js
  * ②.在git里使用命令行打开C:\Users\Easpada\.atom\packages>即插件所在的根目录。
  * ③.将插件在github上的源码git clone 到插件所在的根目录。
  * ④.打开插件路径C:\Users\Easpada\.atom\packages>linter并使用npm install指令对插件进行安装。
  * ⑤.安装成功后插件的目录下面会出现一个node_modules文件夹。
  * ⑥.通过C:\Users\Easpada\.atom\packages\linter>dir指令可查看当前插件的目录。

