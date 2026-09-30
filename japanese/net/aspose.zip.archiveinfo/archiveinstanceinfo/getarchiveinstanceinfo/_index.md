---
title: "ArchiveInstanceInfo.GetArchiveInstanceInfo"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveInstanceInfo メソッド。アーカイブインスタンス情報を取得します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

アーカイブ インスタンス情報を取得します。

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | アーカイブファイルのファイル名です。 |

### 戻り値

フォーマットが検出されなかった場合は null となる、アーカイブインスタンスに関する情報。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *fileName* は null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *fileName* が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | *fileName* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *fileName* がシステムで定義された最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *fileName* のファイル名にコロン (:) が途中に含まれています。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | 指定されたファイルが見つかりませんでした。 |

### 関連項目

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

アーカイブ インスタンス情報を取得します。

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | アーカイブファイルのストリーム。 |

### 戻り値

フォーマットが検出されなかった場合は null となる、アーカイブインスタンスに関する情報。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *stream* は null です。 |
| ArgumentException | *stream* はシーク可能ではありません。 |

### 関連項目

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


