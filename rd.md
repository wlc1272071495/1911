



1.  安装ruby(sass基于Ruby语言开发而成，因此安装sass前需要安装Ruby)
    1.1  安装教程详见官网  https://www.sass.hk/install/
    1.2  测试ruby 是否安装成功    ruby -v
    1.3  安装sass  命令    gem install 路径(拖拽对应的 sass-3.4.22.gem)文件即可
    1.4  测试sass 是否安装成功  sass -v
    

2.  监听sass 
    手动找到项目文件 在 改项目根目录中 按住shift + 鼠标右键 会出现 "在此处打开powerShell(命令行)窗口"
    手动输入命令监听 

    2.1   单文件监听
    命令:   sass --watch sass所在的文件夹/监听的sass文件 : 输出的文件夹/输出的文件名
    eg:    sass --watch sass/nav.scss:css/nav.css   (按ctrl + C 停止监听)

     2.1   文件夹监听
    命令:   sass --watch sass所在的文件夹 : 输出的文件夹
    eg:    sass --watch sass:css



3.  sass 的四种输出模式

    <!-- 嵌套 -->
    sass --watch sass:css   --style nested  
    <!-- expanded  展开的 -->
    sass --watch sass:css   --style expanded  
    <!-- compact  紧凑的 -->
    sass --watch sass:css   --style compact  
    <!-- compressed  压缩 -->
    sass --watch sass:css   --style compressed  


     
     


3.  
    sass 的六个特性
    1. 定义变量   $deep-color :red;
    2. 嵌套css /  嵌套属性

        嵌套css
        .wrap{
            .left{
                
            }
            .right{

            }
        }

        border: {
            width:1px;
            style:solid;
            color:red;
        }
    
    3.  &  >  +  ~

    4.  混合器
    @minxin center{
        text-align:center;
        line-height:24px;
    }

    @include center;


    5.  函数
    @function name($arg1,$arg2){

        @return 
    }

    name();

    6. 选择器的继承

    .test{
        background-color:#f00;
    }

    .box{
        @extend .test;
    }

    7. 导入sass文件
    @import "url";


