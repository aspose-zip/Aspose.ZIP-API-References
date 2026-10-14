---
title: "License"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "コンポーネントのライセンスを付与するメソッドを提供します。"
type: docs
weight: 79
url: /ja/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

コンポーネントのライセンスを付与するメソッドを提供します。


この例では、コンポーネントの jar ファイルが含まれるフォルダー内に MyLicense.lic という名前のライセンスファイルを探す試みが行われます：

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


コンポーネントにライセンスを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| licenseFile | java.io.File | ファイルパス名の表現 |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


コンポーネントにライセンスを適用します。

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
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| licenseName | java.lang.String | 完全なファイル名または短いファイル名、または埋め込みリソースの名前を指定できます。空文字列を使用すると評価モードに切り替わります。 |

