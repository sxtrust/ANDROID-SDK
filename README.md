# 山西信托AndroidSDK

## 1、获取SDK
### a)在项目的build.gradle中添加
```
allprojects {
  repositories {
    ...
    maven {
      url 'https://raw.githubusercontent.com/sxtrust/ANDROID-SDK/master'
    }
  }
}
```
### b)在Module的build.gradle中添加
```
implementation 'com.sxxt:sdk:0.1.8-SNAPSHOT'
```

## 2、使用
```java
SXTrustSDK.getInstance()
```

### a)初始化SDK
```java
/**
* @param isDev 是否为开发模式
*/
init(boolean isDev);
```

### b)唤起
```java
/**
* @param context
* @param loginChannel 登录渠道 *必须
* @param productCode  产品编号 *非必须，不传默认全部
*/
startInvest(Context context, String loginChannel, String productCode);
```
