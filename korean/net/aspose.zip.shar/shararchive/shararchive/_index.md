---
title: SharArchive.SharArchive
second_title: .NET API 참조용 Aspose.ZIP
description: SharArchive 건설자. 의 새 인스턴스를 초기화합니다.SharArchive 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

의 새 인스턴스를 초기화합니다.[`SharArchive`](../) 클래스.

```csharp
public SharArchive()
```

### 예

다음 예제는 파일을 압축하는 방법을 보여줍니다.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### 또한보십시오

* class [SharArchive](../)
* 네임스페이스 [Aspose.Zip.Shar](../../shararchive/)
* 집회 [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### 또한보십시오

* class [SharArchive](../)
* 네임스페이스 [Aspose.Zip.Shar](../../shararchive/)
* 집회 [Aspose.Zip](../../../)


