---
title: "SharArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SharArchive メソッド。提供された宛先ファイルにアーカイブを保存します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

提供された宛先ファイルにアーカイブを保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *destinationFileName* は長さ0の文字列であるか、空白文字のみを含むか、System.IO.Path.InvalidPathChars で定義された無効な文字が1つ以上含まれています。 |
| ArgumentNullException | *destinationFileName* が null です。 |
| PathTooLongException | 指定された *destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| DirectoryNotFoundException | 指定された *destinationFileName* は無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| UnauthorizedAccessException | *destinationFileName* が読み取り専用ファイルを指しており、アクセスが読み取りできません。 - または - パスがディレクトリを指しています。 - または - 呼び出し元に必要な権限がありません。 |
| NotSupportedException | *destinationFileName* の形式が無効です。 |
| FileNotFoundException | ファイルが見つかりません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 備考

アーカイブを読み込んだのと同じパスに保存することは可能です。ただし、この方法は一時ファイルへのコピーを使用するため推奨されません。

## 例

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### 関連項目

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

アーカイブを指定されたストリームに保存します。

```csharp
public void Save(Stream output)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *output* は null です。 |
| ArgumentException | *output* は書き込み可能ではありません。 - または - *output* は抽出元と同じストリームです。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 備考

*output* must be writable.

## 例

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### 関連項目

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


