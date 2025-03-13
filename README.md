## 使用Xposed

参考`app/src/main/java/com/android/hp/Entry.java`

不要修改`app/src/main/assets/xposed_init`
不要修改全类名 `com.android.hp.Entry#init` 这是入口函数

```
// 参数`Bundle params`目前没有任何含义空值
public static void init(Context appContext, Bundle params)
```

## 如何使用native?

在`app/src/main/assets/native_init`添加你的SO, 使用方法参考Lsposed

## 编译请使用Release

```
./gradlew :app:assembleRelease
```
