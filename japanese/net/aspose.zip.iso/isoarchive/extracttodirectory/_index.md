---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoArchive メソッド。指定されたディレクトリにすべてのエントリを抽出します"
type: docs
weight: 60
url: /ja/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

すべてのエントリを指定されたディレクトリに抽出します。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | String | エントリを抽出するディレクトリです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブが編集モードの場合にスローされます。 |
| ArgumentNullException | *destinationDirectory* が null の場合にスローされます。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


