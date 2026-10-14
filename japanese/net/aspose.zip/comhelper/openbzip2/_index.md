---
title: "ComHelper.OpenBzip2"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ComHelper メソッド。COM アプリケーションがストリームから bzip2 アーカイブを読み込むことを可能にします。"
type: docs
weight: 20
url: /ja/net/aspose.zip/comhelper/openbzip2/
---
## OpenBzip2(Stream) {#openbzip2}

COM アプリケーションがストリームから bzip2 アーカイブをロードできるようにします。

```csharp
public Bzip2Archive OpenBzip2(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ロードするアーカイブを含む .NET ストリーム オブジェクトです。 |

### 戻り値

アーカイブを表す [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| InvalidDataException | 署名バイトが正しくありません。 |

### 関連項目

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenBzip2(string) {#openbzip2_1}

COM アプリケーションがファイルから bzip2 アーカイブをロードできるようにします。

```csharp
public Bzip2Archive OpenBzip2(string fileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | ロードするアーカイブのファイル名。 |

### 戻り値

アーカイブを表す [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ArgumentException | ファイル名が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| ArgumentNullException | *fileName* は `null` です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidDataException | 署名バイトが正しくありません。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | *fileName* へのアクセスが拒否されました。 |

### 関連項目

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


