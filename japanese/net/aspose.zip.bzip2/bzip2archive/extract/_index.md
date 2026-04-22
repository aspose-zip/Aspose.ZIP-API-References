---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2Archive 方法. 提供されたストリームにアーカイブを抽出します
type: docs
weight: 30
url: /ja/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

提供されたストリームにアーカイブを抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *destination*書き込みをサポートしていません。 |

### 例

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)


