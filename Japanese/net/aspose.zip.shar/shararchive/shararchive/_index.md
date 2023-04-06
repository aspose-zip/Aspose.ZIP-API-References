---
title: SharArchive.SharArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: SharArchive コンストラクタ. の新しいインスタンスを初期化しますSharArchiveclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

の新しいインスタンスを初期化します[`SharArchive`](../)class.

```csharp
public SharArchive()
```

### 例

次の例は、ファイルを圧縮する方法を示しています。

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### 関連項目

* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)


