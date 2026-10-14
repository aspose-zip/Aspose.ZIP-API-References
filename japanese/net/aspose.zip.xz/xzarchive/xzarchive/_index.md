---
title: "XzArchive.XzArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XzArchive コンストラクタ。XzArchive クラスの新しいインスタンスを初期化し、xz 形式でアーカイブを作成します"
type: docs
weight: 10
url: /ja/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

[`XzArchive`](../) クラスの新しいインスタンスを初期化し、xz 形式でアーカイブを作成します。

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 設定 | XzArchiveSettings | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ。 |

### 関連項目

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(Stream, XzLoadOptions) {#constructor_1}

[`XzArchive`](../) クラスの新しいインスタンスを初期化し、解凍用に準備します。

```csharp
public XzArchive(Stream source, XzLoadOptions options = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソースです。 |
| オプション | XzLoadOptions | アーカイブを読み込む際のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *source* はシーク可能ではありません。 |
| ArgumentNullException | *source* が null です。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |
| InvalidDataException | データが無効または破損しています。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

### 関連項目

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(string, XzLoadOptions) {#constructor_2}

[`XzArchive`](../) クラスの新しいインスタンスを初期化し、解凍用に準備します。

```csharp
public XzArchive(string path, XzLoadOptions options = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブのソースへのパスです。 |
| オプション | XzLoadOptions | アーカイブを読み込む際のオプション。 |

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
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

### 関連項目

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


