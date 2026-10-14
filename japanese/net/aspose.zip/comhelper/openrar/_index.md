---
title: "ComHelper.OpenRar"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ComHelper メソッド。COM アプリケーションがストリームから rar アーカイブを読み込むことを可能にします。"
type: docs
weight: 40
url: /ja/net/aspose.zip/comhelper/openrar/
---
## OpenRar(Stream) {#openrar}

COM アプリケーションがストリームから rar アーカイブを読み込むことを許可します。

```csharp
public RarArchive OpenRar(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ロードするアーカイブを含む .NET ストリーム オブジェクトです。 |

### 戻り値

アーカイブを表す [`RarArchive`](../../../aspose.zip.rar/rararchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

### 関連項目

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenRar(string) {#openrar_1}

COM アプリケーションがファイルから rar アーカイブを読み込むことを許可します。

```csharp
public RarArchive OpenRar(string fileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | ロードするアーカイブのファイル名。 |

### 戻り値

アーカイブを表す [`RarArchive`](../../../aspose.zip.rar/rararchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | ファイル名が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| ArgumentNullException | *fileName* は `null` です。 |
| 例外 | 実行時エラーが発生したときにスローされます。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | *fileName* へのアクセスが拒否されました。 |

### 関連項目

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


