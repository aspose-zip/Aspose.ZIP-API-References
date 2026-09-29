---
title: "License"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Menyediakan metode untuk melisensikan komponen."
type: docs
weight: 79
url: /id/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Menyediakan metode untuk melisensikan komponen.


Dalam contoh ini, akan dicoba menemukan file lisensi bernama MyLicense.lic di folder yang berisi file jar komponen:

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


Memberi lisensi pada komponen.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| licenseFile | java.io.File | representasi jalur nama file |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


Memberi lisensi pada komponen.

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| licenseName | java.lang.String | Dapat berupa nama file lengkap atau pendek, atau nama sumber daya yang disematkan. Gunakan string kosong untuk beralih ke mode evaluasi. |

