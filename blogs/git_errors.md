# 1.今天 当我  执行  git add  somefile 的时候，出现 如下 错误：
```
If no other git process is currently running, this probably means a
git process crashed in this repository earlier. Make sure no other git
process is running and remove the file manually to continue.
```
# 解决方法：
```
rm -f ./.git/index.lock
```
# 2. 编译ICS时 出现 如下错误：
```
build/core/java.mk:20: *** dalvik/dexgen: Invalid LOCAL_SDK_VERSION '4' Choices are: current .  Stop.
```
# 解决方法：
```
rm -rf prebuilt ; repo sync prebuilt
```

 and more...
