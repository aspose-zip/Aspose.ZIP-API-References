---
title: "TarFormat"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "サポートされている形式の列挙です。"
type: docs
weight: 169
url: /ja/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

サポートされている形式の列挙です [TarArchive](../../com.aspose.zip/tararchive)。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [Gnu](#Gnu) | GNU tar は POSIX.1 の初期ドラフトに基づいています。 |
| [Pax](#Pax) | フォーマットは POSIX.1-2001 標準で定義されています。 |
| [UsTar](#UsTar) | フォーマットは v7 フォーマットからヘッダーブロックを拡張しています。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar は POSIX.1 の初期ドラフトに基づいています。このフォーマットは多くの Linux システムでデフォルトの tar フォーマットとして実装されています。

### Pax {#Pax}
```
public static final TarFormat Pax
```


フォーマットは POSIX.1-2001 標準で定義されています。

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


フォーマットは v7 フォーマットからヘッダーブロックを拡張しています。Windows 用の多くのユーティリティで広く使用され、サポートされています。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
