---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: AesEcryptionSettings 건설자. 의 새 인스턴스를 초기화합니다.AesEcryptionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`AesEcryptionSettings`](../) 클래스.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| password | String | 암호화 또는 암호 해독을 위한 암호입니다. |
| method | EncryptionMethod | 암호의 블록 크기를 나타내는 알고리즘 옵션입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| NotSupportedException | *method* 다음 중 하나가 아닙니다.AES128 ,AES192 , 또는AES256. |

### 예

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### 또한보십시오

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../aesecryptionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

의 새 인스턴스를 초기화합니다.[`AesEcryptionSettings`](../)비밀번호가 없는 클래스.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| method | EncryptionMethod | 암호의 블록 크기를 나타내는 알고리즘 옵션입니다. |

### 또한보십시오

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../aesecryptionsettings/)
* 집회 [Aspose.Zip](../../../)


