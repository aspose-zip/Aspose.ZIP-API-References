---
title: TarArchive.FromZ
second_title: Aspose.ZIP for .NET API リファレンス
description: TarArchive 方法. 提供された Z 形式のアーカイブを抽出し構成しますTarArchive抽出されたデータから.
type: docs
weight: 50
url: /ja/net/aspose.zip.tar/tararchive/fromz/
---
## FromZ(Stream) {#fromz}

提供された Z 形式のアーカイブを抽出し、構成します[`TarArchive`](../)抽出されたデータから.

重要: Z アーカイブはこのメソッド内で完全に抽出され、その内容は内部に保持されます。メモリ消費に注意.

```csharp
public static TarArchive FromZ(Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソース。 |

### 戻り値

のインスタンス[`TarArchive`](../)

### 備考

Tar アーカイブは、任意のレコードを抽出する機能を提供するため、フードの下でシーク可能なストリームを操作する必要があります。

### 関連項目

* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## FromZ(string) {#fromz_1}

提供された Z 形式のアーカイブを抽出し、構成します[`TarArchive`](../)抽出されたデータから.

重要: Z アーカイブはこのメソッド内で完全に抽出され、その内容は内部に保持されます。メモリ消費に注意.

```csharp
public static TarArchive FromZ(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |

### 戻り値

のインスタンス[`TarArchive`](../)

### 備考

Tar アーカイブは、任意のレコードを抽出する機能を提供するため、フードの下でシーク可能なストリームを操作する必要があります。

### 関連項目

* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)


