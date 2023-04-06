---
title: TarArchive.SaveGzipped
second_title: .NET API 참조용 Aspose.ZIP
description: TarArchive 방법. gzip 압축을 사용하여 아카이브를 스트림에 저장합니다.
type: docs
weight: 130
url: /ko/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

gzip 압축을 사용하여 아카이브를 스트림에 저장합니다.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| output | Stream | 대상 스트림. |
| format | Nullable`1 | tar 헤더 형식을 정의합니다. Null 값은 가능한 경우 USStar로 처리됩니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *output* null입니다. |
| ArgumentException | *output* 쓸 수 없습니다. |

### 비고

*output*쓰기 가능해야 합니다.

### 예

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### 또한보십시오

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

gzip 압축을 사용하여 경로별로 아카이브를 파일에 저장합니다.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |
| format | Nullable`1 | tar 헤더 형식을 정의합니다. Null 값은 가능한 경우 USStar로 처리됩니다. |

### 예

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### 또한보십시오

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)


