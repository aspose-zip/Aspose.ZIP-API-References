---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ArchiveSaveOptions 속성. 기존 ZIP 아카이브 저장을 위한 암호화 설정을 가져오거나 설정합니다"
type: docs
weight: 60
url: /ko/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

기존 ZIP 아카이브 저장을 위한 암호화 설정을 가져오거나 설정합니다.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## 비고

암호화된 아카이브를 일반적으로 구성할 때 이 옵션을 사용하지 말고, 대신 [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/)를 사용하십시오.

`[`DataDescriptorPolicy`](../datadescriptorpolicy/)` 값이 ForAllFileEntries인 경우 호환되지 않습니다.

## 예제

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### 또 보기

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


