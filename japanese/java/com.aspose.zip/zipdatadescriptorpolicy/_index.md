---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "Data Descriptor の存在に関するオプション。"
type: docs
weight: 171
url: /ja/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Data Descriptor の存在に関するオプション。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [Always](#Always) | Data Descriptor はすべての zip エントリに常に存在します。 |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor はファイルデータを持つエントリにのみ存在し、ディレクトリには省略されます。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor はすべての zip エントリに常に存在します。

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor はファイルデータを持つエントリにのみ存在し、ディレクトリには省略されます。このオプションの使用は推奨されません。

暗号化されていないアーカイブにのみ適用できます。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
