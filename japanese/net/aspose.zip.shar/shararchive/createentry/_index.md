---
title: "SharArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SharArchive メソッド。アーカイブ内に単一のエントリを作成します"
type: docs
weight: 40
url: /ja/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

### 戻り値

Shar エントリのインスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *name* が null です。 |
| ArgumentException | *name* が空です。 |
| ArgumentNullException | *fileInfo* が null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 備考

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが破棄されるまでブロックされます。

## 例

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| sourcePath | String | 圧縮対象ファイルへのパス。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

### 戻り値

Shar エントリのインスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourcePath* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *sourcePath* が空、または空白のみ、または無効な文字が含まれています。 - または - *name* の一部であるファイル名が 100 文字を超えています。 |
| UnauthorizedAccessException | *sourcePath* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *sourcePath*、ファイル名、またはその両方がシステム定義の最大長を超えています。例えば、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 - または - *name* が shar に対して長すぎます。 |
| NotSupportedException | *sourcePath* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*sourcePath* パラメータで提供されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが破棄されるまでブロックされます。

## 例

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |

### 戻り値

Shar エントリのインスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *name* が null です。 |
| ArgumentNullException | *source* が null です。 |
| ArgumentException | *name* が空です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 例

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


