---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "使用这些选项从压缩文件加载。"
type: docs
weight: 116
url: /zh/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

使用这些选项从压缩文件加载 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | 获取用于解密条目及条目名称的密码。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | 设置用于解密条目及条目名称的密码。 |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


获取用于解密条目及条目名称的密码。

您可以在归档提取时一次性提供解密密码。

```

``````

try (FileInputStream fs = new FileInputStream(\"encrypted_archive.7z\");
FileOutputStream extracted = new FileOutputStream(\"extracted.bin\")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel 7Z archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setCancellationFlag(cf);
         try (SevenZipArchive a = new SevenZipArchive("big.7z", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

取消通常会导致部分数据未被提取。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 用于取消提取操作的取消标志。 |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


设置用于解密条目及条目名称的密码。

您可以在归档提取时一次性提供解密密码。

```

``````

try (FileInputStream fs = new FileInputStream(\"encrypted_archive.7z\");
FileOutputStream extracted = new FileOutputStream(\"extracted.bin\")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

