---
title: Class SelfExtractorOptions
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Saving.SelfExtractorOptions 수업. 자동 압축 풀기 실행 가능 아카이브 생성 옵션.
type: docs
weight: 500
url: /ko/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

자동 압축 풀기 실행 가능 아카이브 생성 옵션.

```csharp
public class SelfExtractorOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | 추출 시 추출기 창을 닫아야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | 추출기 창의 제목을 가져오거나 설정합니다. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | 아카이브 추출이 완료된 후 실행할 프로그램을 가져오거나 설정합니다. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | 추출기 응용 프로그램의 기본 창에 대한 제목 아이콘의 경로를 가져오거나 설정합니다. |

### 비고

자동 압축 풀기 아카이브는 측정된 라이선스로 구성할 수 없습니다.[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### 예

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### 또한보십시오

* 네임스페이스 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 집회 [Aspose.Zip](../../)


