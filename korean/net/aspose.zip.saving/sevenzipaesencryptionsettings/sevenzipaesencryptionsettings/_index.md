---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipAESEncryptionSettings 건설자. 의 새 인스턴스를 초기화합니다.SevenZipAESEncryptionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`SevenZipAESEncryptionSettings`](../) 클래스.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| password | String | 암호화 또는 암호 해독을 위한 암호입니다. |

### 예

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 또한보십시오

* class [SevenZipAESEncryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

의 새 인스턴스를 초기화합니다.[`SevenZipAESEncryptionSettings`](../) 외부 암호가 있는 클래스.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| cipher | SevenZipCipher | 맞춤형 AES 구현. |

### 예

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 또한보십시오

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* 집회 [Aspose.Zip](../../../)


