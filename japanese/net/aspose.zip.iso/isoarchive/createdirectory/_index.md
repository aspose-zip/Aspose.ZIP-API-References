---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoArchive メソッド。ディレクトリを ISO イメージに追加します"
type: docs
weight: 30
url: /ja/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

ISO イメージにディレクトリを追加します。

```csharp
public IsoEntry CreateDirectory(string name)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | ISO 内のディレクトリのパスです。 |

### 戻り値

ISO エントリが構成されました。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブは抽出用に開かれています。 |
| ArgumentNullException | `name` は null または空です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

### 関連項目

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


