# git/ES6

## [选择题] 如果提示提交内容为空、不能提交，则最为合适的处理方式是：
#### [选项] 
* A.执行 git status 查看状态，再执行 git add 命令选择要提交的文件，然后提交
* B.执行 git commit --allow-empty ，允许空提交。
* C.执行 git commit -a ，提交所有改动。
* D.执行 git commit --amend 进行修补提交。

#### [答案] A

## [选择题] 我使用和其他人不一样的IDE软件，总是在目录下生成以 .xx 为后缀的临时文件。如何避免由于自己的误操作导致此类文件被添加到版本库中呢？
#### [选项] 
* A.执行 git clean -f 删除临时性文件。
* B.向版本库中添加一个 .gitignore 文件，其中包含一条内容为 *.xx 的记录。
* C.在文件 .git/info/exclude 中添加一条内容为 *.xx 的记录。
* D.更换另外一款IDE软件。

#### [答案] B

## [选择题] 所有改动的文件都已加入暂存区，若希望将其中的 other.py 文件下次再提交，如何操作？
#### [选项] 
* A.git reset -- other.py
* B.git checkout -- other.py
* C.git checkout HEAD other.py
* D.git reset --hard -- other.py

#### [答案] B

## [选择题] 关于删除分支XX，下列说法正确的是
#### [选项] 
* A.执行 git push origin :XX 来删除远程版本库的 XX 分支。
* B.执行 git branch -D XX 删除分支，总是能成功
* C.远程版本库删除的分支，在执行 git fetch 时本地分支自动删除
* D.本地删除的分支，执行 git push 时，远程分支亦自动删除

#### [答案] B

## [选择题] 以下程序的输出结果是：
```
function bar(x=y;y=2){
	return [x,y];
}
bar();
```
#### [选项] 
* A.[2,undefined]
* B.[undefined, 2]
* C.[2, 2]
* D.报错

#### [答案] C

## [选择题] 以下程序的输出结果是：
```
function move({x, y} = { x: 0, y: 0 }) {
  return [x, y];
}
	
move({x: 3, y: 8});
```
#### [选项] 
* A.[3, 8]
* B.[3, undefined]
* C.[undefined, 8]
* D.报错

#### [答案] A

## [选择题] 以下程序的输出结果是：
```
function foo() {
  export default 'bar';
}
foo()
```
#### [选项] 
* A.''
* B.undefined
* C.bar
* D.Error

#### [答案] C

## [选择题] 以下程序的输出结果是：
```
class B {}
let b = new B();

b.constructor === B.prototype.constructor
```
#### [选项] 
* A.true
* B.false
* D.Error

#### [答案] B


## [命令题] 你修改了一段代码，要怎么才能更新到远端；
#### [答案] git add ,commit -m ,push

## [命令题] 回退到上一版本，并且提交到远端；
#### [答案] git reset --hard commit_id ,commit

## [命令题] 用定义类的方法，来写一个加减法；
#### [答案] class A{
        constructor(x,y){
        this.x = x;
        this.y = y ;
        }
        add(){
            return `this.x + this.y`;
        }
        sub(){
            return `this.x - this.y`;
        }
}

# maven

# 试题名称
#### [作者] 管鹏波
#### [邮箱] guanpengbo@haomo-studio.com
#### [版本] v1.0.0
#### [标签]
* maven

## [选择题] pom.xml中project必须存在的标签
#### 标签
* maven

#### [选项]
* A.modelVersion
* B.url
* C.version
* D.groupId

#### [答案] D
* 

## [选择题] C直接依赖B，B直接依赖A，C->B  B->A，那么C和A的关系
#### 标签
* maven

#### [选项]
* A.直接关系
* B.间接关系
* C.没有关系
* D.依赖关系

#### [答案] B
* 

## [选择题] 如果直接依赖中包含有同一个坐标不同版本的资源依赖（先配置版本1，后配置版本2，版本2顺序靠后），那么jar包会如何引用。
#### 标签
* maven

#### [选项]
* A.产生冲突
* B.引用版本1
* C.引用版本2
* D.找不到依赖包

#### [答案] D
* 


## [选择题] Maven有哪些优点
#### 标签
* maven

#### [选项]
* A.简化了项目依赖管理
* B.易于上手
* C.配置比ant的灵活
* D.约定优于配置

#### [答案] A B D
* 

## [选择题] 属于编译命令的是
#### 标签
* maven

#### [选项]
* A.mvn compile
* B.mvn -v
* C.mvn package
* D.mvn install

#### [答案] A
* 


## [选择题] 下面有关maven和ant的描述，描述错误的是？
#### [标签]
* maven

#### [选项]
* A、Ant没有正式的约定如一个一般项目的目录结构，你必须明确的告诉Ant哪里去找源代码
* B、Maven拥有约定，因为你遵循了约定，它已经知道你的源代码在哪里
* C、maven和ant都有“生命周期”的概念，当你输入一个命令后，maven或者ant会执行一系列的有序的步骤，直到到达你指定的生命周期
* D、Ant构建文件默认命名为build.xml，Maven默认构建文件为pom.xml

#### [答案] C
* 


## [选择题] maven有三套生命周期，分别为：
#### 标签
* maven

#### [选项]
* A.clean周期
* B.默认周期
* C.site周期
* D.test周期

#### [答案]  A B C 
* 


## [选择题] maven有三套生命周期，分别为：
#### 标签
* maven

#### [选项]
* A.clean周期
* B.默认周期
* C.site周期
* D.test周期

#### [答案] A B C
* 

## [填空题] Maven是____组织中的一个开源项目。
#### [标签]
* maven

#### [答案] apache
* 



## [填空题] Maven项目的结构和内容在一个XML文件中声明，____项目对象模型（POM），这是整个Maven系统的基本单元。
#### [标签]
* maven

#### [答案]pom.xml
* 


## [填空题] Maven的依赖库查询顺序，首先会查询____。
#### [标签]
* maven

#### [答案] 本地仓库
* 


## [填空题] maven是不是跨平台的。____（是或者不是）
#### [标签]
* maven

#### [答案] 是
* 

## [填空题] maven不仅是构建工具，它还是____工具和项目管理工具，提供了中央仓库，能够帮我们自动下载构件。
#### [标签]
* maven

#### [答案] 依赖管理工具
* 

## [填空题] 为了解决的依赖的增多，版本不一致，版本冲突，依赖臃肿等问题，它通过一个____系统来精确地定位每一个构件（artifact）。
#### [标签]
* maven

#### [答案] 坐标
* 


## [填空题] maven采用____的策略（convention over configuration），虽然上手容易，但是一旦出了问题，难于调试。
#### [标签]
* maven

#### [答案] 约定优于配置
* 


## [命令题] （maven基本操作）maven编译项目命令____
#### [标签] mvn compile
* maven

#### [答案]
* 

## [命令题] （maven基本操作）maven构建项目命令____
#### [标签]
* maven

#### [答案] mvn generator
* 

## [命令题] （maven基本操作）maven打包和部署项目到本地资源库命令____
#### [标签]
* maven

#### [答案] mvn ackage
* 


## [命令题] （maven基本操作）maven单元测试命令____
#### [标签]
* maven

#### [答案] mvn test
* 

## [命令题] （maven基本操作）maven清理项目命令____
#### [标签]
* maven

#### [答案] mvn clean
* 

# java

# 试题名称
#### [作者] 管鹏波
#### [邮箱] guanpengbo@haomo-studio.com
#### [版本] v1.0.0
#### [标签]
* maven

## [选择题] 以下属于Java8新特性的是
#### 标签
* java8

#### [选项]
* A.Lambda表达式
* B.重复注解
* C.类的默认方法和静态方法
* D.更好的类型推断

#### [答案] A B C
* 

## [选择题] Lambda表达式不包含的部分
#### 标签
* java8

#### [选项]
* A.->符号
* B.=符号
* C.语句块
* D.逗号分隔的参数列表

#### [答案] B
* 

## [选择题] 接口中可以定义默认非抽象的方法，使用的关键字是
#### 标签
* java8

#### [选项]
* A.default关键字
* B.static关键字
* C.final关键字
* D.public关键字

#### [答案] A
* 


## [选择题] 以下关于JAVA语言异常处理描述正确的有？
#### 标签
* java

#### [选项]
* A.throw关键字可以在方法上声明该方法要抛出的异常。
* B.throws用于抛出异常对象。
* C.在try块中不可以抛出异常
* D.try是用于检测被包住的语句块是否出现异常，如果有异常，则抛出异常，并执行catch语句。

#### [答案] A B D
* 


## [选择题] 为了克服函数式接口的脆弱性并且能够明确声明接口作为函数式接口的意图，Java8增加了一种特殊的注解是
#### 标签
* java8

#### [选项]
* A.@FunctionalInterface
* B.@FunctionInterface
* C.@Functional
* D.@Interface

#### [答案] D
* 


## [选择题] 重复注解机制本身必须用____注解。
#### [标签]
* Java8

#### [选项]
* A、@Target
* B、@Retention
* C、@Repeatable
* D、@interface

#### [答案]  B
* 


## [选择题] Java8扩展了注解的上下文,以下可以添加注解的是
#### 标签
* java8

#### [选项]
* A.局部变量
* B.泛型类
* C.父类与接口的实现
* D.方法的异常

#### [答案]  C
* 


## [选择题] 下面哪些写法能在 java8 中编译执行（）
#### 标签
* java8

#### [选项]
* A.dir.listfiles((file f)->f.getName().endsWith(“.Java”));
* B.dir.listfiles((file f)=>f.getName().endsWith(“.Java”));
* C.dir.listfiles((_.getName().endsWith(“.Java”));
* D.dir.listfiles( f->f.getName().endsWith(“.Java”));

#### [答案] A
* 

## [填空题] 为了解决空指针异常，java8引入了____类
#### [标签]
* java8

#### [答案] optional
* 


## [填空题] java8的java.time包涵盖了所有处理日期，时间，日期/时间，时区，时刻（instants），过程（during）与时钟（____类）的操作。
#### [标签]
* java8

#### [答案] timeZone
* 


## [填空题] Java 8编译器在类型推断方面有很大的提升，在很多场景下编译器可以推导出某个参数的____，从而使得代码更为简洁。
#### [标签]
* java8

#### [答案] 类型
* 


## [填空题] ____指的是只有一个函数的接口，这样的接口可以隐式转换为Lambda表达式。
#### [标签]
* java8

#### [答案] 函数式接口
* 

## [填空题] Java8用默认方法与____这两个新概念来扩展接口的声明。
#### [标签]
* java8

#### [答案] lambda表达式
* 

## [填空题] Lambda可以引用类的成员变量与局部变量，为了效率更高，这些变量会被隐含的转为____
#### [标签]
* java8

#### [答案]参数
* 


## [填空题] java8构造器引用的语法（类Car）____
#### [标签]
* java8

#### [答案] constructor
* 

## [编码题] 将下面的代码修改成Lambda表达式（至少两种）
        List<String> names = Arrays.asList("zhao","qian","sun","li");
        Collections.sort(names, new Comparator<String>() {
            @Override
            public int compare(String o1, String o2) {
                return o1.compareTo(o2);
            }
        });
#### [答案] 1、names.stream().forEach(e->system.out.println("姓氏" +e);
2、

## [编码题] 将下面的代码修改成Lambda表达式
        new Thread(new Runnable() {
            @Override
            public void run() {
                System.out.println("线程1--test");
            }
        }).start();
#### [答案]  new Thread(()->System.out.println("线程1--test")).start();

## [编码题] 输出1995-06-01 01:12:24 -- 2014-07-10 02:12:15的时间差
#### [答案] 
zonedDateTime a = '1995-06-01';
zonedDateTime b = '2014-07-10';
System.out.println(b-a);

# NPM/Bower

## [选择题] npm作为前端包管理工具，下面描述错误的是
#### [标签]
* npm
* 工具

#### [选项]
* A、npm的主要功能就是管理node包，包括：安装、卸载、更新、查看、搜索等功能
* B、npm的包安装分为全局安装和本地安装
* C、npm是基于node包管理工具,安装node会同时安装npm
* D、npm安装的所有依赖都将记录在package.json的dependencies属性中

#### [答案] D
* 

## [选择题] 对于前端包管理工具npm的package.json描述错误的是
#### [标签]
* npm
* 工具

#### [选项]
* A、package.json可以通过npm init在项目初始化
* B、package.json里的对象属性包括:name、scripts、dependencies、devDependencies等
* C、package.json至少包括name和version两个属性
* D、package.json的scripts属性里记录了项目中的所有node包

#### [答案] D
* 

## [选择题] 对于使用npm install安装前端包的描述正确的是
#### [标签]
* npm
* 工具

#### [选项]
* A、npm install <packageName>可以使用npm -i <packageName>的缩写形式来代替
* B、npm install <packageName>默认可以将npm记录到package.json的dependencies中
* C、npm install <packageName>默认将安装包安装到全局环境下的node_modules
* D、npm install <packageName>默认可以将npm记录到package.json的devDependencies中

#### [答案] C
* 

## [选择题] 关于npm命令描述错误的是：
#### [标签]
* npm
* 工具

#### [选项]
* A、运行npm ls就可以查看当前目录安装了哪些package
* B、运行npm uninstall grunt-cli可以删除当前目录安装的grunt-cli的package
* C、运行npm install -g <packageName>可以将特定的包信息保存在项目目录下的package.json中
* D、运行npm update <packageName>可以升级特定的package


#### [答案] D
* 
## [选择题] npm描述错误的是：
#### [标签]
* npm
* 工具

#### [选项]
* A、npm install -g <packageName>将package安装在全局环境中，可以在任何目录下使用
* B、npm install --save <packageName>将package安装在目录环境下载node_modules文件下，并且将信息保存在dependencies中
* C、npm uninstall <packageName>可以将目录文件夹和全局中的package同时删除
* D、npm install --save-dev <packageName>将package安装在目录环境下载node_modules文件下，并且将信息保存在devDependencies中

#### [答案] C
* 

## [填空题] 使用npm安装jquery到目录文件夹下，并将安装的package信息保存到package.json中，使用的指令是___
#### [标签]
* npm
* 工具

#### [答案]
* npm install jquery

## [填空题] 使用npm管理前端中的package，我们可以使用___升级项目中已经安装的lodash

#### [标签]
* npm
* 工具

#### [答案] npm update lodash
* 

## [填空题] 使用npm安装前端打包工具gulp到项目文件目录中，并将安装的package信息保存到package.json的devDependencies中，使用的指令是___

#### [标签]
* npm
* 工具

#### [答案]
*  npm install -D gulp

## [填空题] 使用npm安装前端打包工具gulp到项目文件目录中，并将安装的gulp信息保存到package.json的devDependencies中，使用的指令是___

#### [标签]
* npm
* 工具

#### [答案]
* npm install -D gulp

## [填空题] 使用npm管理前端package，可以使用___查看已经安装的gulp的信息

#### [标签]
* npm
* 工具

#### [答案]
* npm view gulp

## [填空题] 使用npm管理前端package，可以使用___指令搜索webpack相关的包信息

#### [标签]
* npm
* 工具

#### [答案]
* npm search webpack

## [填空题] 使用npm管理前端package，在项目文件夹下使用___来初始化一个package.json;

#### [标签]
* npm
* 工具

#### [答案]
* npm init

## [填空题] 在我们的项目中,使用bower管理前端项目的package，使用___来下载jquery到本地目录下，并保存信息到bower.json；

#### [标签]
* bower
* 工具

#### [答案] bower install jquery

##  [填空题] 在我们的项目中,使用bower管理前端项目的package，使用___来下载gulp（构建工具）到本地目录下，并保存信息到bower.json；

#### [标签]
* bower
* 工具

#### [答案] bower install gulp

## [填空题] 从github上clone了一个前端项目；在使用bower管理项目中的依赖包时，我们可以使用___来下载刚clone的项目中的bower.json保存的package信息相关的前端包。

#### [标签]
* bower
* 工具

#### [答案] bower install <pkg>



