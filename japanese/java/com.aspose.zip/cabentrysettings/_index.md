---
title: "CabEntrySettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "CAB エントリの書き込み方法を制御する設定。"
type: docs
weight: 47
url: /ja/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

CAB エントリの書き込み方法を制御する設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | 特定の圧縮プロファイルで設定を初期化します。 |
| [CabEntrySettings()](#CabEntrySettings--) | デフォルトの MSZip 圧縮で設定を初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | エントリに適用された圧縮設定を取得します。 |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


特定の圧縮プロファイルで設定を初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | 使用する圧縮設定。 |

以下のいずれかにできます: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


デフォルトの MSZip 圧縮で設定を初期化します。

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


エントリに適用された圧縮設定を取得します。

以下のいずれかにできます：

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
