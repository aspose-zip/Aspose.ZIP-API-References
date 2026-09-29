---
title: "WimEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "wim イメージ内の単一ファイルまたはディレクトリを表します。"
type: docs
weight: 132
url: /ja/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

wim イメージ内の単一ファイルまたはディレクトリを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | ファイルまたはディレクトリの代替データストリームの名前を取得します。 |
| [getArchive()](#getArchive--) | エントリが属するアーカイブを取得します。 |
| [getChangeTime()](#getChangeTime--) | ファイルまたはディレクトリが最後に変更された時刻を取得します。 |
| [getCreationTime()](#getCreationTime--) | ファイルまたはディレクトリの作成時刻を取得します。 |
| [getFileAttributes()](#getFileAttributes--) | ファイルまたはディレクトリの属性を取得します。 |
| [getFullPath()](#getFullPath--) | イメージ内のエントリのフルパスを取得します。 |
| [getHardLink()](#getHardLink--) | ファイルまたはディレクトリのハードリンク ID を取得します。 |
| [getImage()](#getImage--) | エントリが属するイメージを取得します。 |
| [getLastAccessTime()](#getLastAccessTime--) | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [getLastWriteTime()](#getLastWriteTime--) | ファイルまたはディレクトリの更新時刻を取得します。 |
| [getModificationTime()](#getModificationTime--) | ファイルまたはディレクトリの更新時刻を取得します。 |
| [getName()](#getName--) | イメージ内のエントリの名前を取得します。 |
| [getParent()](#getParent--) | エントリが属する親ディレクトリを取得します。 |
| [getShortName()](#getShortName--) | イメージ内のエントリの短縮名を取得します。 |
| [hasHardLinks()](#hasHardLinks--) | ファイルまたはディレクトリが別名で知られているかどうかを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [toString()](#toString--) | インスタンスである [WimEntry](../../com.aspose.zip/wimentry) クラスの文字列表現を返します。 |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


ファイルまたはディレクトリの代替データストリームの名前を取得します。

**Returns:**
java.lang.String[] - ファイルまたはディレクトリの代替データストリームの名前
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


エントリが属するアーカイブを取得します。

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


ファイルまたはディレクトリが最後に変更された時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリが最後に変更された時刻
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


ファイルまたはディレクトリの作成時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリの作成時刻
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


ファイルまたはディレクトリの属性を取得します。

**Returns:**
int - ファイルまたはディレクトリの属性
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


イメージ内のエントリのフルパスを取得します。

**Returns:**
java.lang.String - イメージ内のエントリのフルパス
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


ファイルまたはディレクトリのハードリンク ID を取得します。

**Returns:**
long - ファイルまたはディレクトリのハードリンク ID
### getImage() {#getImage--}
```
public final WimImage getImage()
```


エントリが属するイメージを取得します。

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


ファイルまたはディレクトリの最終アクセス時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリの最終アクセス時刻
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


ファイルまたはディレクトリの更新時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリの更新時刻
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


ファイルまたはディレクトリの更新時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリの更新時刻
### getName() {#getName--}
```
public final String getName()
```


イメージ内のエントリの名前を取得します。

**Returns:**
java.lang.String - イメージ内のエントリの名前
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


エントリが属する親ディレクトリを取得します。

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


イメージ内のエントリの短縮名を取得します。

**Returns:**
java.lang.String - イメージ内のエントリの短縮名
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


ファイルまたはディレクトリが別名で知られているかどうかを取得します。

**Returns:**
boolean - ファイルまたはディレクトリが別名で知られているかどうか
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


エントリがディレクトリを表すかどうかを示す値を取得します。

**Returns:**
boolean - エントリがディレクトリを表すかどうかを示す値
### toString() {#toString--}
```
public String toString()
```


インスタンスである [WimEntry](../../com.aspose.zip/wimentry) クラスの文字列表現を返します。

**Returns:**
java.lang.String - このオブジェクトの文字列表現
