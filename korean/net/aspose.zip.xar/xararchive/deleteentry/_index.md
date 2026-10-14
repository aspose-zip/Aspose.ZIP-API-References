---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarArchive 메서드. 항목 목록에서 특정 항목의 첫 번째 발생을 제거합니다"
type: docs
weight: 50
url: /ko/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

특정 항목의 첫 번째 발생을 항목 목록에서 제거합니다.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | XarEntry | 항목 목록에서 제거할 항목입니다. |

### 반환 값

Xar 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *entry*가 null입니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 열려 있지 않습니다. |

## 예제

다음은 마지막 항목을 제외한 모든 항목을 제거하는 방법입니다:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### 또 보기

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


