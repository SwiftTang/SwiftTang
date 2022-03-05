👋 Hi, I’m @SwiftTang
### 专注于用Swift解决问题
- 目前正在学习算法，已上架APP - 灿灿，就是希望用算法来提高投资能力的APP
- 欢迎大家使用和建议，谢谢。
未来我将在GITHUB,就我在学习过程中所面临的问题，以及我的解决办法，以最简洁明了方式分享出来，希望对您有用。


### 基础
#### Podfile
Podfile是干什么的，怎么用？
看Viperit的示例：

    source 'https://github.com/CocoaPods/Specs.git' 
    platform :ios, '12.0' 
    use_frameworks! 
    
    pod 'Viperit' 

##### 问题来了，怎么建这个文件，怎么添加这些内容呢？
完成如下步骤后，用XCODE打开项目文件即可使用。
1. 打开MAC应用程序： 终端
2. 进入项目文件夹，如：
    cd ~\xcode\practice\Sample
3. 使用POD init创建podfile文件 
    pod init
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
 4. 在终端执行pop install加载库
    
    pod install
