1. 通过终端执行
```
cd ~/.cocoapods/repos
git clone "https://github.com/CocoaPods/Specs" master --depth 1
```
2. 在Podfile中去掉：
      Removing # before #source 'https://github.com/CocoaPods/Specs.git'
3. Running ` pod install `
