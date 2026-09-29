---
title: "XarEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "xar アーカイブ内の単一エントリを表します。"
type: docs
weight: 140
url: /ja/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

xar アーカイブ内の単一エントリを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | ファイルまたはディレクトリの作成時刻を取得します。 |
| [getFullPath()](#getFullPath--) | アーカイブ内のエントリの完全パスを取得します。 |
| [getLastAccessTime()](#getLastAccessTime--) | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [getLastWriteTime()](#getLastWriteTime--) | ファイルまたはディレクトリの更新時刻を取得します。 |
| [getModificationTime()](#getModificationTime--) | ファイルまたはディレクトリの更新時刻を取得します。 |
| [getName()](#getName--) | アーカイブ内のエントリ名を取得します。 |
| [getParent()](#getParent--) | エントリが属する親ディレクトリを取得します。 |
| [isDirectory()](#isDirectory--) | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [toString()](#toString--) | インスタンスである [XarEntry](../../com.aspose.zip/xarentry) クラスの文字列表現を返します。 |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


ファイルまたはディレクトリの作成時刻を取得します。

**Returns:**
java.util.Date - ファイルまたはディレクトリの作成時刻
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


アーカイブ内のエントリの完全パスを取得します。

**Returns:**
java.lang.String - アーカイブ内のエントリの完全パス
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


アーカイブ内のエントリ名を取得します。

**Returns:**
java.lang.String - アーカイブ内のエントリの名前
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


エントリが属する親ディレクトリを取得します。

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
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


インスタンスである [XarEntry](../../com.aspose.zip/xarentry) クラスの文字列表現を返します。

**Returns:**
java.lang.String - このオブジェクトの文字列表現
