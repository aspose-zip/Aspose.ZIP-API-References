---
title: "XarArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarArchive メソッド。指定された宛先ファイルにアーカイブを保存します。"
type: docs
weight: 80
url: /ja/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

アーカイブを指定された宛先ファイルに保存します。

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| saveOptions | XarSaveOptions | xar アーカイブを保存するためのオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationFileName* が null です。 |
| InvalidOperationException | xar アーカイブを変更できません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | *destinationFileName* が読み取り専用のファイルを指定しています。-or- *destinationFileName* がディレクトリを指定しています。-or- 呼び出し元に必要な権限がありません。 |

### 関連項目

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

アーカイブを指定されたストリームに保存します。

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| saveOptions | XarSaveOptions | xar アーカイブを保存するためのオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *output* は null です。 |
| ArgumentException | *output* は書き込み可能/読み取り可能ではないか、シークできません。 |
| InvalidOperationException | xar アーカイブを変更できません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

### 関連項目

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


