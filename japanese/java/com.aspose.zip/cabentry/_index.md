---
title: "CabEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "cab アーカイブ内の単一ファイルを表します。"
type: docs
weight: 46
url: /ja/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

cab アーカイブ内の単一ファイルを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | エントリを提供されたストリームに抽出します。 |
| [extract(String path)](#extract-java.lang.String-) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [getLength()](#getLength--) | エントリの長さ（バイト単位）を取得します。 |
| [getModificationTime()](#getModificationTime--) | 最終更新日時を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [open()](#open--) | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| [toString()](#toString--) | インスタンスの文字列表現を返します（[CabEntry](../../com.aspose.zip/cabentry) クラス）。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


エントリを提供されたストリームに抽出します。

CAB アーカイブのエントリを抽出します。

```

``````

try (CabArchive archive = new CabArchive(\"archive.cab\")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | java.lang.String | 宛先ファイルへのパスです。ファイルが既に存在する場合は上書きされます。 |

**Returns:**
java.io.File - 組み立てられたファイルの情報
### getLength() {#getLength--}
```
public final Long getLength()
```


エントリの長さ（バイト単位）を取得します。

**Returns:**
java.lang.Long - エントリのバイト単位の長さ
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


最終更新日時を取得します。

**Returns:**
java.util.Date - 最終更新日時。
### getName() {#getName--}
```
public final String getName()
```


アーカイブ内のエントリ名を取得します。

**Returns:**
java.lang.String - アーカイブ内のエントリの名前
### open() {#open--}
```
public final InputStream open()
```


エントリを抽出用に開き、エントリの内容を含むストリームを提供します。

使用方法:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
