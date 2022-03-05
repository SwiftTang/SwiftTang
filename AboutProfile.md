#### Podfile
*Podfile是干什么的?*
*怎么用？*
下面以，Viperit为例，看如何添加库：

    source 'https://github.com/CocoaPods/Specs.git' 
    platform :ios, '12.0' 
    use_frameworks! 
    
    pod 'Viperit' 

##### 问题来了，怎么建这个文件，怎么添加这些内容呢？
完成如下步骤后，用XCODE打开项目文件即可使用。
1. 打开MAC应用程序(实用工具)： 终端
2. 进入项目文件夹，如：`cd ~\xcode\practice\Sample`
3. 使用 `POD init` 创建podfile文件 
4. 打开Podfile，添加项目及库信息

        \# Uncomment the next line to define a global platform for your project
        \# platform :ios, '9.0'
    
        \# 1. 添加.xcodeproj文件，如下：
        project 'VaporPractice.xcodeproj'
     
        target 'VaporPractice' do
       \# Comment the next line if you don't want to use dynamic frameworks
       use_frameworks!
 
       \# Pods for VaporPractice
    
        \# 2. 添加库文件
        source 'https://github.com/CocoaPods/Specs.git'
        platform :ios, '12.0'
        use_frameworks!
    
        pod 'Viperit'
        
        end
5. 在终端执行 `pop install` 加载库
