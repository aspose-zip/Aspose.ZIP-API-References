---
title: Bzip2Archive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2Archive 方法. 提供されたストリームにアーカイブを保存します
type: docs
weight: 50
url: /ja/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

提供されたストリームにアーカイブを保存します。

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| outputStream | Stream | 宛先ストリーム。 |
| saveOptions | Bzip2SaveOptions | bzip2 アーカイブを保存するためのオプション。指定しない場合、900 Kb のブロック サイズが使用されます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | アーカイブするデータのソースが提供されていません。 |
| ArgumentException | *outputStream*書き込み不可です。 |
| UnauthorizedAccessException | ファイル ソースが読み取り専用であるか、ディレクトリです。 |
| DirectoryNotFoundException | 指定されたファイル ソース パスは、マップされていないドライブ上にあるなど、無効です。 |
| IOException | ファイル ソースは既に開いています。 |

### 備考

*outputStream*書き込み可能でなければなりません。

### 例

圧縮データを http 応答ストリームに書き込みます。

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 関連項目

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

指定された宛先ファイルにアーカイブを保存します。

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |
| saveOptions | Bzip2SaveOptions | bzip2 アーカイブを保存するためのオプション。指定しない場合、900 Kb のブロック サイズが使用されます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *destinationFileName*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*destinationFileName*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*destinationFileName*否定された。 |
| PathTooLongException | 指定された*destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*destinationFileName*文字列の途中にコロン (:) が含まれています。 |

### 例

圧縮データをファイルに書き込みます。

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### 関連項目

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)


