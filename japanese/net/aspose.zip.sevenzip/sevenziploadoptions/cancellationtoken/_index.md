---
title: "SevenZipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipLoadOptions プロパティ。抽出操作をキャンセルするために使用されるキャンセルトークンを取得または設定します。"
type: docs
weight: 20
url: /ja/net/aspose.zip.sevenzip/sevenziploadoptions/cancellationtoken/
---
## SevenZipLoadOptions.CancellationToken property

抽出操作をキャンセルするために使用されるキャンセルトークンを取得または設定します。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 備考

このプロパティは .NET Framework 4.0 以降で使用できます。

## 例

一定時間後に 7Z アーカイブの抽出をキャンセルします。

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new SevenZipArchive("big.7z", new SevenZipLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Entries[0].Extract("data.bin");
        }
        catch(OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

`Task` と併用する

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new SevenZipLoadOptions() { CancellationToken = cts.Token };
    using (var a = new SevenZipArchive("big.7z", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(Task antecedent)
{
     if (antecedent.IsCanceled)
     {
         Console.WriteLine("Extraction was cancelled after 60 seconds");
     }

     cts.Dispose();
});
```

キャンセルにより、主に一部のデータが抽出されないことがあります。

### 関連項目

* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


