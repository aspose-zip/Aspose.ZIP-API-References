---
title: Archive.DeleteEntry
second_title: .NET API 참조용 Aspose.ZIP
description: Archive 방법. 항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다.
type: docs
weight: 60
url: /ko/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| entry | ArchiveEntry | 항목 목록에서 제거할 항목입니다. |

### 반환 값

항목이 삭제된 아카이브.

### 예

마지막 항목을 제외한 모든 항목을 제거하는 방법은 다음과 같습니다.

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### 또한보십시오

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

항목 목록에서 항목을 index. 로 제거합니다.

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### 또한보십시오

* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)


