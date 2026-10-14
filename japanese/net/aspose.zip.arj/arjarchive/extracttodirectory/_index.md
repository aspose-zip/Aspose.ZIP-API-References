---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArjArchive メソッド。すべてのエントリを指定されたディレクトリに抽出します。"
type: docs
weight: 60
url: /ja/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* が null の場合にスローされます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| InvalidDataException | ヘッダーまたはデータのチェックサムが一致しません。 - または - アーカイブが破損しています。 |
| NotImplementedException | エントリはメソッド 4 で圧縮されています。 |

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


