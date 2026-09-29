---
title: "License"
second_title: "Aspose.ZIP for Java API 参考"
description: "提供对组件授权的方法。"
type: docs
weight: 79
url: /zh/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

提供对组件授权的方法。


在本示例中，将尝试在包含组件 jar 文件的文件夹中查找名为 MyLicense.lic 的许可证文件：

```

``````

License license = new License();
license.setLicense("MyLicense.lic");
 
```


## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initializes a new instance of the [License](../../com.aspose.zip/license) class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licenses the component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenses the component. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licenses the component. |
### License() {#License--}
```
public License()
```


Initializes a new instance of the [License](../../com.aspose.zip/license) class.


In this example, an attempt will be made to find a license file named MyLicense.lic in the folder that contains the component jar file:

```

``````

     License license = new License();
     license.setLicense("MyLicense.lic");
 
```



### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


为组件授权。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| licenseFile | java.io.File | 文件路径名的表示形式 |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


为组件授权。

```

``````

License license = new License();
license.setLicense(myStream);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A stream that contains the license. |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licenses the component.

Library tries to find the license in the following locations:

1. Explicit path.

2. The folder that contains the Aspose component JAR file.

3. The folder that contains the client's calling JAR file.


In this example, an attempt will be made to find a license file named MyLicense.lic in locations listed above:

```

``````

     License license = new License();
     license.setLicense("MyLicense.lic");
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| licenseName | java.lang.String | 可以是完整或简短的文件名，或嵌入资源的名称。使用空字符串可切换到评估模式。 |

