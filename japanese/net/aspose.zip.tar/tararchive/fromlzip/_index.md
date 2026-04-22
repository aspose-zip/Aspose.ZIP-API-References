---
title: TarArchive.FromLZip
second_title: Aspose.ZIP for .NET API リファレンス
description: TarArchive 方法. 提供された lzip アーカイブを抽出して構成しますTarArchive抽出されたデータから.
type: docs
weight: 30
url: /ja/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

提供された lzip アーカイブを抽出して構成します[`TarArchive`](../)抽出されたデータから.

重要: lzip アーカイブはこのメソッド内で完全に抽出され、その内容は内部に保持されます。メモリ消費に注意.

```csharp
public static TarArchive FromLZip(Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソース。 |

### 戻り値

のインスタンス[`TarArchive`](../)

### 備考

Lzip 抽出ストリームは、圧縮アルゴリズムの性質上、シークできません。 tar アーカイブは任意のレコードを抽出する機能を提供するため、内部でシーク可能なストリームを操作する必要があります。

### 関連項目

* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

提供された lzip アーカイブを抽出して構成します[`TarArchive`](../)抽出されたデータから.

重要: lzip アーカイブはこのメソッド内で完全に抽出され、その内容は内部に保持されます。メモリ消費に注意.

```csharp
public static TarArchive FromLZip(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |

### 戻り値

のインスタンス[`TarArchive`](../)

### 備考

Lzip 抽出ストリームは、圧縮アルゴリズムの性質上、シークできません。 tar アーカイブは任意のレコードを抽出する機能を提供するため、内部でシーク可能なストリームを操作する必要があります。

### 関連項目

* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)


