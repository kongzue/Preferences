# Preferences
Preferences是SharedPreferences的简易封装。

## 1.0说明：
每次手写SharedPreferences过于繁琐，因此封装了一个简易的属性记录读取类。
通过对属性的常见数据类型进行封装，使属性读取写入更方便，同时提供一些属性管理方法。

方法说明：
```
//读取属性为String类型
//参数：context上下文索引，path路径，preferencesName属性名
getPreferencesToString(context, path, preferencesName)
//类似的，提供读取为Boolean的方法：
getPreferencesToBoolean(context, path, preferencesName)
//提供读取为Int的方法：
getPreferencesToInt(context, path, preferencesName)

//写入属性方法是统一的
//参数：context上下文索引，path路径，preferencesName属性名，value根据属性数据类型定义
setPreferences(context, path, preferencesName, ?)

//提供清除（清空）所有属性的方法
cleanAll();
```
