---
title: "UueSaveOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "uuencoded ファイルを保存するためのオプション。"
type: docs
weight: 129
url: /ja/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

uuencoded ファイルを保存するためのオプション。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | ユーザーが提供したファイル名と改行でオプションを初期化します。 |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | ユーザーが提供したファイル名とデフォルトの改行でオプションを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFileName()](#getFileName--) | デコードされたデータを再作成する際に使用されるファイル名を取得します。 |
| [getNewLine()](#getNewLine--) | 各行を終了させる文字を取得します。通常は "\n" または "\r\n" です。 |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | ファイルの Unix パーミッションを取得します。 |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | ファイルの Unix パーミッションを設定します。 |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


ユーザーが提供したファイル名と改行でオプションを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | デコードされたデータを再作成する際に使用されるファイル名 |
| newLine | java.lang.String | 各行を終了させる文字 |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


ユーザーが提供したファイル名とデフォルトの改行でオプションを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | デコードされたデータを再作成する際に使用されるファイル名 |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


デコードされたデータを再作成する際に使用されるファイル名を取得します。

**Returns:**
java.lang.String - デコードされたデータを再作成する際に使用されるファイル名
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


各行を終了させる文字を取得します。通常は "\n" または "\r\n" です。

**Returns:**
java.lang.String - 各行を終了させる文字、通常は "\n" または "\r\n"。
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


ファイルの Unix パーミッションを取得します。

デフォルトは 644 です。

**Returns:**
java.lang.String - ファイルの Unix パーミッション
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


ファイルの Unix パーミッションを設定します。

デフォルトは 644 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | ファイルの Unix パーミッション |

