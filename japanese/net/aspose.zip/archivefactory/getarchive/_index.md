---
title: "ArchiveFactory.GetArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveFactory メソッド。指定されたパスで指定されたアーカイブの種類に従って、アーカイブ形式を検出し、適切な IArchive オブジェクトを作成します。"
type: docs
weight: 20
url: /ja/net/aspose.zip/archivefactory/getarchive/
---
## GetArchive(string) {#getarchive_2}

指定されたパスで指定されたアーカイブの種類に従って、アーカイブ形式を検出し、適切な [`IArchive`](../../iarchive/) オブジェクトを作成します。

```csharp
public static IArchive GetArchive(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 解析対象のアーカイブへのパスです。 |

### 戻り値

アーカイブを表す [`IArchive`](../../iarchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* は `null` です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | *path* で指定されたファイルが見つかりませんでした。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | *path* がディレクトリを指定しました。-or- 呼び出し元に必要な権限がありません。 |

### 関連項目

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream) {#getarchive}

指定されたストリームで指定されたアーカイブの種類に従って、アーカイブ形式を検出し、適切な [`IArchive`](../../iarchive/) オブジェクトを作成します。

```csharp
public static IArchive GetArchive(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | アーカイブデータを含むストリームです。シーク可能である必要があります。 |

### 戻り値

アーカイブを表す [`IArchive`](../../iarchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *stream* はシーク可能ではありません。 |
| ArgumentNullException | *stream* は null です。 |

### 関連項目

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream, string) {#getarchive_1}

指定されたストリームで指定された暗号化アーカイブの種類に従って、アーカイブ形式を検出し、適切な [`IArchive`](../../iarchive/) オブジェクトを作成します。

```csharp
public static IArchive GetArchive(Stream stream, string password)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | アーカイブデータを含むストリームです。シーク可能である必要があります。 |
| password | String | 暗号化されたアーカイブを復号化するためのパスワードです。 |

### 戻り値

アーカイブを表す [`IArchive`](../../iarchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *stream* はシーク可能ではありません。 |
| ArgumentNullException | *stream* は null です。 |

### 関連項目

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


