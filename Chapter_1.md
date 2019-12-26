# 第一章 开发环境
- ## 安装 [jdk](https://www.oracle.com/technetwork/java/javase/downloads/index.html)（8或以上版本）
- ## 安装 [IntelliJ IDEA](https://www.jetbrains.com/idea/download/#section=windows) （community版本可以免费使用）
- ## 下载 [fabric-mod-example](https://github.com/FabricMC/fabric-example-mod/) 到本地
- ## 修改 gradle.properties 文件
  1. ### mod_version = 1.0.0（版本号）
  2. ### maven_group = com.github.haodong1101 (包名)
  3. ### archives_base_name = demo (模组名)
  4. ### 通过[这个网站](https://modmuss50.me/fabric.html?&version=1.14.4)修改 minecraft_version、yarn_mappings、loader_version、fabric_version 的参数信息
       ![image](./Resource/image/1.png)
- ## 修改 项目文件
   1. ### 修改文件路径名为自己的包名（src\main\java\net\fabricmc\example -> src\main\java\com\github\haodong1101）
   2. ### 修改模组主文件名为自己的模组名（ExampleMod.java -> DemoMod.java）
   3. ### 修改资源文件路径名（src\main\resources\assets\modid -> src\main\resources\assets\demo）
- ## 修改 src\main\resources\fabric.mod.json 文件
   1. ### "id" 模组ID
   2. ### "name"   模组名
   3. ### "description"   描述
   4. ### "icon"  模组图标
   5. ### "entrypoints":"main"  模组主文件地址
   6. ### "depends":"minecraft"  minecraft版本
       ![image](./Resource/image/2.png)
- ## 构建Gradle项目
   1. ### 进入项目根目录，选择资源管理器的菜单：文件-> 打开Windows PowerShell
   2. ### 命令行中输入 
            .\gradle idea
    1. ### 等待命令完成 （中国大陆由于众所周知的原因，此命令可能较慢或者失败，请多次尝试，或使用代理）