---
title: "ArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveEntry イベント。生ストリームの一部が抽出されたときに発生します"
type: docs
weight: 100
url: /ja/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

生ストリームの一部が抽出されたときに発生します。

```csharp
public event EventHandler<ProgressCancelEventArgs> ExtractionProgressed;
```

## 備考

イベント送信者は [`ArchiveEntry`](../) インスタンスです。抽出をキャンセルすることが可能です。

## 例

このサンプルでは、処理済みサイズの割合をパーセンテージで計算するためにイベントハンドラが使用されています。

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

このサンプルでは、エントリの最初の数百 MB が抽出された後にキャンセルするためにイベントハンドラが使用されています。

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => { if (e.ProceededBytes > 100000000) e.Cancel = true; };
```

### 関連項目

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


