---
title: CpioArchive.DeleteEntry
second_title: .NET API 참조용 Aspose.ZIP
description: CpioArchive 방법. 항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| entry | CpioEntry | 항목 목록에서 제거할 항목입니다. |

### 반환 값

Cpio 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *entry* null입니다. |

### 예

마지막 항목을 제외한 모든 항목을 제거하는 방법은 다음과 같습니다.

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### 또한보십시오

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

항목 목록에서 항목을 index. 로 제거합니다.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| entryIndex | Int32 | 제거할 항목의 0부터 시작하는 인덱스입니다. |

### 반환 값

항목이 삭제된 아카이브.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* 0보다 작음.-또는-*entryIndex* 같거나 크다`항목` 세다. |

### 예

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### 또한보십시오

* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)


