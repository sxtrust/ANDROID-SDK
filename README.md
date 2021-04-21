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
implementation 'com.sxxt:sdk:1.0.0'
```

## 2、使用
```java
SXTrustSDK.getInstance()
```

### a)初始化SDK
```java
init();

/**
* @param isDev 是否为开发模式
*/
init(boolean isDev);
```

### b)唤起
```java
/**
* @param context
* @param channel      渠道  *必须
* @param productCode  产品编号  *非必须，不传默认全部
*/
startInvest(Context context, String channel, String productCode);
```
### c)其他
#### 1)setDev(boolean isDev);//设置开发模式

