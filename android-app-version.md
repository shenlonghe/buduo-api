## 安卓APP版本检测
【token不需要】

```
GET /1/android-app-version
```

#### 结果示例1(有新版):
```
{
  "status": "SUCCESS",
  "error_message": "",
  "results": [
    {
      "version": "1.0.1",
      "apk_url": "https://pic.buduobushao.com/apps/buduobushao-1.0.1.apk"
    }
  ]
}
```

#### 结果示例2（无新版）:
```
{
  "status": "SUCCESS",
  "error_message": "",
  "results": []
}
```
