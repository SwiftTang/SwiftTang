### `pod install` 问题解决办法
> 在执行 ` pod install`时，如遇到 `Couldn't determine repo type for URL: ...` 问题
1. 通过终端执行
```
cd ~/.cocoapods/repos
git clone "https://github.com/CocoaPods/Specs" master --depth 1
```
2. 在Podfile中去掉：
      Removing # before #source 'https://github.com/CocoaPods/Specs.git'
3. Running ` pod install `
