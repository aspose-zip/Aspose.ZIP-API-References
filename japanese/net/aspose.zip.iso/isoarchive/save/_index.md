---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoArchive メソッド。指定されたパスに ISO イメージを保存します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

ISO イメージを指定されたパスに保存します。

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | ISO イメージが保存されるパス。 |
| saveOptions | IsoSaveOptions | ISO アーカイブを保存するためのオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブが編集モードでないときにスローされます。 |
| ArgumentNullException | *path* が null のときにスローされます。 |
| DirectoryNotFoundException | 指定されたパスが無効な場合（例: マッピングされていないドライブ上にある場合）にスローされます。 |
| IOException | ファイルがすでに開かれている場合にスローされます。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否された場合にスローされます。 |
| PathTooLongException | 指定された *path* がシステム定義の最大長を超える場合にスローされます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

次の例は、ISO アーカイブをファイルに保存する方法を示しています:

```csharp
// 新しい空の ISO アーカイブを作成する
using(IsoArchive isoArchive = new IsoArchive())
{
    // ISO アーカイブにファイルを追加する
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO アーカイブをファイルに保存する
    isoArchive.Save("new_archive.iso");
}
```

### 関連項目

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

ISO イメージを指定されたストリームに保存します。

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ISO イメージが保存されるストリームです。 |
| saveOptions | IsoSaveOptions | ISO アーカイブを保存するためのオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブが編集モードでないときにスローされます。 |
| ArgumentNullException | *stream* が null の場合にスローされます。 |
| ArgumentException | *stream* が書き込み可能でない場合にスローされます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| IOException | I/O エラーが発生しました。 |

## 例

次の例は、ISO アーカイブをメモリ ストリームに保存する方法を示しています:

```csharp

 // 新しい空の ISO アーカイブを作成する
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // ISO アーカイブにファイルを追加する
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // ISO アーカイブをメモリ ストリームに保存する
     isoArchive.Save(memoryStream);
 }
```

### 関連項目

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


