---
title: "TarArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。アーカイブ内に単一のエントリを作成します"
type: docs
weight: 110
url: /ja/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| fileInfo | FileSystemInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |

### 戻り値

Tar エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| PathTooLongException | *name* は IEEE 1003.1-1998 標準に基づく tar の制限を超えて長すぎます。 |
| ArgumentException | *name* の一部であるファイル名が 100 文字を超えています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## 例

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

### 戻り値

Tar エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| PathTooLongException | *name* は IEEE 1003.1-1998 標準に基づく tar の制限を超えて長すぎます。 |
| ArgumentException | *name* の一部であるファイル名が 100 文字を超えています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

*fileInfo* can refer to DirectoryInfo if the entry is directory.

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが破棄されるまでブロックされます。

## 例

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 圧縮対象ファイルへのパス。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

### 戻り値

Tar エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみを含むか、無効な文字を含んでいます。-または- *name* の一部であるファイル名が 100 文字を超えています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。-または- *name* は IEEE 1003.1-1998 標準に基づく tar の制限を超えて長すぎます。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*path* パラメータで指定されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが破棄されるまでブロックされます。

## 例

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


