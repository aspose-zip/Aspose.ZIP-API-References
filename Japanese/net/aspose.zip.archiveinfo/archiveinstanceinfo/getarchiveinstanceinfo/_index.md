---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveInstanceInfo 方法. アーカイブ インスタンス情報を取得します
type: docs
weight: 10
url: /ja/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

アーカイブ インスタンス情報を取得します。

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fileName | String | アーカイブ ファイルのファイル名。 |

### 戻り値

アーカイブ インスタンスに関する情報、またはフォーマットが検出されなかった場合は null。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *fileName*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*fileName*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*fileName*否定された。 |
| PathTooLongException | 指定された*fileName*システム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*fileName*文字列の途中にコロン (:) が含まれています。 |
| IOException | ファイルを開くときに入出力エラーが発生しました。 |

### 関連項目

* class [ArchiveInstanceInfo](../)
* 名前空間 [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* 組み立て [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

アーカイブ インスタンス情報を取得します。

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | アーカイブ ファイルのストリーム。 |

### 戻り値

アーカイブ インスタンスに関する情報、またはフォーマットが検出されなかった場合は null。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *stream*無効である。 |
| ArgumentException | *stream*はシークできません。 |

### 関連項目

* class [ArchiveInstanceInfo](../)
* 名前空間 [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* 組み立て [Aspose.Zip](../../../)


