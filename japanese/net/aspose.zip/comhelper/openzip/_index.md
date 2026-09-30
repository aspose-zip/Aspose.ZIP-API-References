---
title: "ComHelper.OpenZip"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ComHelper メソッド。COM アプリケーションがストリームから ZIP アーカイブをロードできるようにします。"
type: docs
weight: 50
url: /ja/net/aspose.zip/comhelper/openzip/
---
## OpenZip(Stream) {#openzip}

COM アプリケーションがストリームから ZIP アーカイブを読み込むことを許可します。

```csharp
public Archive OpenZip(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ロードするアーカイブを含む .NET ストリーム オブジェクトです。 |

### 戻り値

アーカイブを表す [`Archive`](../../archive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

### 関連項目

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenZip(string) {#openzip_1}

COM アプリケーションがファイルから ZIP アーカイブを読み込むことを許可します。

```csharp
public Archive OpenZip(string fileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | ロードするアーカイブのファイル名。 |

### 戻り値

アーカイブを表す [`Archive`](../../archive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ArgumentException | ファイル名が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| ArgumentNullException | *fileName* は `null` です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | *fileName* へのアクセスが拒否されました。 |

### 関連項目

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


