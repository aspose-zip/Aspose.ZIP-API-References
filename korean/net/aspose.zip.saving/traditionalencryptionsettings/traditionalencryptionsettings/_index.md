---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: TraditionalEncryptionSettings 건설자. 의 새 인스턴스를 초기화합니다.TraditionalEncryptionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`TraditionalEncryptionSettings`](../) 클래스.

```csharp
public TraditionalEncryptionSettings(string password)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| password | String | 암호화용 비밀번호입니다. |

### 예

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [TraditionalEncryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

의 새 인스턴스를 초기화합니다.[`TraditionalEncryptionSettings`](../) 사용자 정의 인코딩이 있는 클래스.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| password | String | 암호화용 비밀번호입니다. |
| encoding | Encoding | 비밀번호 문자 인코딩. |

### 비고

이 생성자의 사용은 권장되지 않습니다. 인코딩을 설정하면 표준과 모순되고 호환되지 않는 아카이브가 생성될 수 있습니다.

### 예

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [TraditionalEncryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

의 새 인스턴스를 초기화합니다.[`TraditionalEncryptionSettings`](../)비밀번호가 없는 클래스.

```csharp
public TraditionalEncryptionSettings()
```

### 또한보십시오

* class [TraditionalEncryptionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 집회 [Aspose.Zip](../../../)


