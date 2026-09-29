---
title: "ComHelper"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "COM クライアントが Aspose.Zip にアーカイブをロードできるようにするメソッドを提供します。"
type: docs
weight: 55
url: /ja/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

COM クライアントが Aspose.Zip にアーカイブをロードできるようにするメソッドを提供します。

ComHelper クラスを使用して、ファイルまたはストリームからアーカイブをロードします。特定のクラスは、新しいアーカイブを作成するデフォルトコンストラクタを提供し、またファイルまたはストリームからアーカイブをロードするためのオーバーロードされたコンストラクタも提供します。.NET アプリケーションで Aspose.Zip を使用している場合、すべてのアーカイブコンストラクタを直接使用できますが、COM アプリケーションで Aspose.Zip を使用している場合は、デフォルトのアーカイブコンストラクタのみが利用可能です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ComHelper()](#ComHelper--) | このクラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | COM アプリケーションがストリームから bzip2 アーカイブをロードできるようにします。 |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | COM アプリケーションがファイルから bzip2 アーカイブをロードできるようにします。 |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | COM アプリケーションがストリームから gzip アーカイブを読み込むことを許可します。 |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | COM アプリケーションがファイルから gzip アーカイブを読み込むことを許可します。 |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | COM アプリケーションがストリームから rar アーカイブを読み込むことを許可します。 |
| [openRar(String fileName)](#openRar-java.lang.String-) | COM アプリケーションがファイルから rar アーカイブを読み込むことを許可します。 |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | COM アプリケーションがストリームから ZIP アーカイブを読み込むことを許可します。 |
| [openZip(String fileName)](#openZip-java.lang.String-) | COM アプリケーションがファイルから ZIP アーカイブを読み込むことを許可します。 |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


このクラスの新しいインスタンスを初期化します。

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


COM アプリケーションがストリームから bzip2 アーカイブをロードできるようにします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | .NET ストリーム オブジェクトで、読み込むアーカイブを含みます。 |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


COM アプリケーションがファイルから bzip2 アーカイブをロードできるようにします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | 読み込むアーカイブのファイル名。 |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


COM アプリケーションがストリームから gzip アーカイブを読み込むことを許可します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | .NET ストリーム オブジェクトで、読み込むアーカイブを含みます。 |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


COM アプリケーションがファイルから gzip アーカイブを読み込むことを許可します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | 読み込むアーカイブのファイル名。 |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


COM アプリケーションがストリームから rar アーカイブを読み込むことを許可します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | .NET ストリーム オブジェクトで、読み込むアーカイブを含みます。 |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


COM アプリケーションがファイルから rar アーカイブを読み込むことを許可します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | 読み込むアーカイブのファイル名。 |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


COM アプリケーションがストリームから ZIP アーカイブを読み込むことを許可します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | .NET ストリーム オブジェクトで、読み込むアーカイブを含みます。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


COM アプリケーションがファイルから ZIP アーカイブを読み込むことを許可します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | 読み込むアーカイブのファイル名。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
