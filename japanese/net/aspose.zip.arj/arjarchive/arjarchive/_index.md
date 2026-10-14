---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArjArchive コンストラクタ。ArjArchive クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを作成します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

[`ArjArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを作成します。

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extractionSource | Stream | アーカイブのソースです。 |
| loadOptions | ArjLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *extractionSource* が null です。 |
| ArgumentException | &gt;*extractionSource* はシークをサポートしていません。 |
| InvalidDataException | アーカイブの署名が間違っています。 - または - ファイルが ARJ アーカイブではありません。 |
| EndOfStreamException | ヘッダー バイトまたは名前バイトがすべて読み取られる前にストリームの終端に達したときにスローされます。 |
| NotSupportedException | アーカイブが破損しています。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Extract`](../../arjentryplain/extract/) メソッドをご覧ください。

### 関連項目

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

[`ArjArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを作成します。

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | ArjLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| EndOfStreamException | ヘッダー バイトまたは名前バイトがすべて読み取られる前にストリームの終端に達したときにスローされます。 |
| InvalidDataException | ARJ のマジックナンバーが無効か、ヘッダーサイズが範囲外です。 |

## 備考

このコンストラクタはエントリを解凍しません。解凍については [`Extract`](../../arjentryplain/extract/) メソッドをご覧ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


