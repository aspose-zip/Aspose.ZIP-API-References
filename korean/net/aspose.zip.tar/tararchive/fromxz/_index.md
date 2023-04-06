---
title: TarArchive.FromXz
second_title: .NET API 참조용 Aspose.ZIP
description: TarArchive 방법. 제공된 xz 형식 아카이브를 추출하고 구성합니다.TarArchive 추출된 데이터에서.
type: docs
weight: 40
url: /ko/net/aspose.zip.tar/tararchive/fromxz/
---
## FromXz(Stream) {#fromxz}

제공된 xz 형식 아카이브를 추출하고 구성합니다.[`TarArchive`](../) 추출된 데이터에서.

중요: xz 아카이브는 이 방법 내에서 완전히 추출되며 해당 콘텐츠는 내부적으로 보관됩니다. 메모리 소모에 주의하세요.

```csharp
public static TarArchive FromXz(Stream source)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| source | Stream | 아카이브의 소스입니다. |

### 반환 값

인스턴스[`TarArchive`](../)

### 비고

Tar 아카이브는 임의의 레코드를 추출하는 기능을 제공하므로 후드 아래에서 탐색 가능한 스트림을 작동해야 합니다.

### 또한보십시오

* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)

---

## FromXz(string) {#fromxz_1}

제공된 xz 형식 아카이브를 추출하고 구성합니다.[`TarArchive`](../) 추출된 데이터에서.

중요: xz 아카이브는 이 방법 내에서 완전히 추출되며 해당 콘텐츠는 내부적으로 보관됩니다. 메모리 소모에 주의하세요.

```csharp
public static TarArchive FromXz(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 아카이브 파일의 경로입니다. |

### 반환 값

인스턴스[`TarArchive`](../)

### 비고

Tar 아카이브는 임의의 레코드를 추출하는 기능을 제공하므로 후드 아래에서 탐색 가능한 스트림을 작동해야 합니다.

### 또한보십시오

* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)


