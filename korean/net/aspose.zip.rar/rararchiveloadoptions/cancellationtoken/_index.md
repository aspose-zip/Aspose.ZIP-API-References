---
title: "RarArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "RarArchiveLoadOptions 속성. 추출 작업을 취소하는 데 사용되는 취소 토큰을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.zip.rar/rararchiveloadoptions/cancellationtoken/
---
## RarArchiveLoadOptions.CancellationToken property

추출 작업을 취소하는 데 사용되는 취소 토큰을 가져오거나 설정합니다.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 비고

이 속성은 .NET Framework 4.0 이상에서 존재합니다.

## 예제

특정 시간 후에 RAR 아카이브 추출을 취소합니다.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new RarArchive("big.rar", new RarArchiveLoadOptions() { CancellationToken = cts.Token }))
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

`Task`와 함께 사용하기

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new RarArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new RarArchive("big.rar", loadOptions))
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

취소는 대부분 일부 데이터가 추출되지 않는 결과를 초래합니다.

### 또 보기

* class [RarArchiveLoadOptions](../)
* namespace [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


