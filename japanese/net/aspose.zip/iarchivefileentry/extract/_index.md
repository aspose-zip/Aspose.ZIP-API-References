---
title: IArchiveFileEntry.Extract
second_title: Aspose.ZIP for .NET API リファレンス
description: IArchiveFileEntry 方法. 提供されたパスによってファイルシステムへのエントリを抽出します.
type: docs
weight: 30
url: /ja/net/aspose.zip/iarchivefileentry/extract/
---
## Extract(string) {#extract}

提供されたパスによってファイルシステムへのエントリを抽出します.

```csharp
public FileInfo Extract(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパス。ファイルが既に存在する場合は、上書きされます。 |

### 戻り値

FileInfo抽出されたデータを含むインスタンス。

### 関連項目

* interface [IArchiveFileEntry](../)
* 名前空間 [Aspose.Zip](../../iarchivefileentry/)
* 組み立て [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

提供されたストリームにエントリを抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 関連項目

* interface [IArchiveFileEntry](../)
* 名前空間 [Aspose.Zip](../../iarchivefileentry/)
* 組み立て [Aspose.Zip](../../../)


