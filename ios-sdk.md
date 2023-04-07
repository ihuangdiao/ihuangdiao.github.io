---
iOS SDK Full API Reference
---

# ThinkingAnalyticsSDK

## + startWithAppId:withUrl:

初始化方法

**Usage:**

 ```objective-c
 [ThinkingAnalyticsSDK startWithAppId:@"YOUR_APPID" 
                              withUrl:@"YOUR_SERVER_URL"];
 ```

| Argument | Type | Description |
| ------------- | ------------- | ----- |
| appId | NSString | APP ID |
| url | NSString | 接收端地址 |

**Returns:**

| Type | Description |
| ----- | ------------- |
| ThinkingAnalyticsSDK | SDK 实例 |

## - track:

自定义事件埋点

**Usage:**

 ```objective-c
 [[ThinkingAnalyticsSDK sharedInstance] track:@"some_event"];
 ```

| Argument | Type | Description |
| ------------- | ------------- | ----- |
| event | NSString | 事件名称 |

---
# TDConfig

## - initWithAppId:serverUrl:

初始化方法

**Usage:**

 ```objective-c
 TDConfig *config = [[TDConfig alloc] initWithAppid:APPID 
                                          serverUrl:SERVER_URL];
 [ThinkingAnalyticsSDK startWithConfig:config];
 ```

| Argument | Type | Description |
| ------------- | ------------- | ----- |
| appId | NSString | APP ID |
| serverUrl | NSString | 接收端地址 |

**Returns:**

| Type | Description |
| ----- | ------------- |
| ThinkingAnalyticsSDK | SDK 实例 |
