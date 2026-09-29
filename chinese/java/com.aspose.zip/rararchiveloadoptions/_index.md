---
title: "RarArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "使用这些选项从压缩文件加载。"
type: docs
weight: 101
url: /zh/java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

用于从压缩文件加载 [RarArchive](../../com.aspose.zip/rararchive) 的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | 获取用于解密条目及条目名称的密码。 |
| [getDictionaryStorageMode()](#getDictionaryStorageMode--) | 获取 RAR 解压缩字典的存储方式。 |
| [getTemporaryDirectory()](#getTemporaryDirectory--) | 获取用于临时字典文件的目录。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | 设置用于解密条目及条目名称的密码。 |
| [setDictionaryStorageMode(RarDictionaryStorageMode value)](#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-) | 设置 RAR 解压缩字典的存储方式。 |
| [setTemporaryDirectory(String value)](#setTemporaryDirectory-java.lang.String-) | 设置用于临时字典文件的目录。 |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


获取用于解密条目及条目名称的密码。

您可以在归档提取时一次性提供解密密码。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### getDictionaryStorageMode() {#getDictionaryStorageMode--}
```
public final RarDictionaryStorageMode getDictionaryStorageMode()
```


Gets how the RAR decompression dictionary is stored.

**Returns:**
[RarDictionaryStorageMode](../../com.aspose.zip/rardictionarystoragemode) - the dictionary storage mode
### getTemporaryDirectory() {#getTemporaryDirectory--}
```
public final String getTemporaryDirectory()
```


Gets the directory used for temporary dictionary files.

**Returns:**
java.lang.String - the temporary directory; the system temporary directory is used by default
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel RAR archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (RarArchive a = new RarArchive("big.rar", options)) {
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

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

### setDictionaryStorageMode(RarDictionaryStorageMode value) {#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-}
```
public final void setDictionaryStorageMode(RarDictionaryStorageMode value)
```


Sets how the RAR decompression dictionary is stored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RarDictionaryStorageMode](../../com.aspose.zip/rardictionarystoragemode) | the dictionary storage mode |

### setTemporaryDirectory(String value) {#setTemporaryDirectory-java.lang.String-}
```
public final void setTemporaryDirectory(String value)
```


Sets the directory used for temporary dictionary files. A null or empty value selects the system temporary directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the temporary directory |

