---
title: "ComHelper"
second_title: "Aspose.ZIP for Java API 참조"
description: "COM 클라이언트가 Aspose.Zip에 아카이브를 로드할 수 있는 메서드를 제공합니다."
type: docs
weight: 55
url: /ko/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

COM 클라이언트가 Aspose.Zip에 아카이브를 로드할 수 있는 메서드를 제공합니다.

ComHelper 클래스를 사용하여 파일이나 스트림에서 아카이브를 로드합니다. 특정 클래스는 새 아카이브를 만들기 위한 기본 생성자를 제공하며 파일이나 스트림에서 아카이브를 로드하기 위한 오버로드된 생성자도 제공합니다. .NET 애플리케이션에서 Aspose.Zip을 사용하는 경우 모든 아카이브 생성자를 직접 사용할 수 있지만, COM 애플리케이션에서 Aspose.Zip을 사용하는 경우 기본 아카이브 생성자만 사용할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ComHelper()](#ComHelper--) | 이 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | COM 애플리케이션이 스트림에서 bzip2 아카이브를 로드하도록 허용합니다. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | COM 애플리케이션이 파일에서 bzip2 아카이브를 로드하도록 허용합니다. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | COM 애플리케이션이 스트림에서 gzip 아카이브를 로드하도록 허용합니다. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | COM 애플리케이션이 파일에서 gzip 아카이브를 로드하도록 허용합니다. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | COM 애플리케이션이 스트림에서 rar 아카이브를 로드하도록 허용합니다. |
| [openRar(String fileName)](#openRar-java.lang.String-) | COM 애플리케이션이 파일에서 rar 아카이브를 로드하도록 허용합니다. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | COM 애플리케이션이 스트림에서 ZIP 아카이브를 로드하도록 허용합니다. |
| [openZip(String fileName)](#openZip-java.lang.String-) | COM 애플리케이션이 파일에서 ZIP 아카이브를 로드하도록 허용합니다. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


이 클래스의 새 인스턴스를 초기화합니다.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


COM 애플리케이션이 스트림에서 bzip2 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | .NET 스트림 객체로, 로드할 아카이브를 포함합니다. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


COM 애플리케이션이 파일에서 bzip2 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 로드할 아카이브의 파일 이름. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


COM 애플리케이션이 스트림에서 gzip 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | .NET 스트림 객체로, 로드할 아카이브를 포함합니다. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


COM 애플리케이션이 파일에서 gzip 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 로드할 아카이브의 파일 이름. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


COM 애플리케이션이 스트림에서 rar 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | .NET 스트림 객체로, 로드할 아카이브를 포함합니다. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


COM 애플리케이션이 파일에서 rar 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 로드할 아카이브의 파일 이름. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


COM 애플리케이션이 스트림에서 ZIP 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | .NET 스트림 객체로, 로드할 아카이브를 포함합니다. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


COM 애플리케이션이 파일에서 ZIP 아카이브를 로드하도록 허용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 로드할 아카이브의 파일 이름. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
