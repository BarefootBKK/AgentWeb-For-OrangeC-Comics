# AgentWeb-For-ComicApp-

本项目封装了AgentWeb，以满足[【漫画APP】](https://blog.csdn.net/HBK_MySummerCT/article/details/89057970)项目的使用需要，也可以在源码上自定义所需功能。

## 使用方法

### Step 1

在Gradle中添加项目依赖

```
implementation 'com.just.agentweb:agentweb:4.0.2'
```

### Step 2

复制本项目的 ```AWCoreController.java``` 文件到你的安卓项目中

## 使用示例

```
// 初始化
AWCoreController awCoreController = 
                        new AWCoreController(Activity或Fragment, new AWCoreController.OnAgentDataLoadingListener() {
                            @Override
                            public void onWebLoading(String html) {
                                // html加载中的目标网页源码
                            }
                        });
// 加载URL
awCoreController.loadUrl(url);
```


## 感谢

- [AgentWeb](https://github.com/Justson/AgentWeb)
