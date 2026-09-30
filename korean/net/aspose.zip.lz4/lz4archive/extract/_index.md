---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Lz4Archive 메서드. 경로에 따라 아카이브를 파일로 추출합니다"
type: docs
weight: 30
url: /ko/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

경로를 지정하여 파일로 아카이브를 추출합니다.

```csharp
public FileInfo Extract(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

### 반환 값

추출된 파일의 정보.

### 예외

| 예외 | 조건 |
| --- | --- |
| EndOfStreamException | 소스 스트림이 너무 짧습니다. |
| InvalidDataException | 디코딩 중 잘못된 바이트가 발견되었습니다. |
| NotSupportedException | 이 LZ4 버전은 지원되지 않습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| InvalidOperationException | 아카이브가 조합을 위해 준비되었습니다. |

### 또 보기

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

제공된 스트림으로 아카이브를 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 대상 | 스트림 | 대상 스트림. 쓰기 가능해야 합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | *destination* 은(는) 쓰기를 지원하지 않습니다. |
| EndOfStreamException | 소스 스트림이 너무 짧습니다. |
| InvalidDataException | 디코딩 중 잘못된 바이트가 발견되었습니다. |
| NotSupportedException | 이 LZ4 버전은 지원되지 않습니다. |
| InvalidOperationException | 아카이브가 조합을 위해 준비되었습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### 또 보기

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


