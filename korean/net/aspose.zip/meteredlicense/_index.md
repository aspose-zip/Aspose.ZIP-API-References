---
title: Class MeteredLicense
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.MeteredLicense 수업. 측정 키를 설정하는 방법을 제공합니다.
type: docs
weight: 290
url: /ko/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

측정 키를 설정하는 방법을 제공합니다.

```csharp
public class MeteredLicense
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | 이 클래스의 새 인스턴스를 초기화합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | 측정된 공개 및 개인 키를 설정합니다. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | 소비 크레딧을 가져옵니다. |

### 비고

중요: 측정 라이센스를 사용하면 자동 압축 해제 zip 아카이브를 작성할 수 없습니다.

### 예

이 예에서는 측정된 공개 및 개인 키를 설정하려고 시도합니다.

```csharp
MeteredLicense matered = new MeteredLicense();
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

### 또한보십시오

* 네임스페이스 [Aspose.Zip](../../aspose.zip/)
* 집회 [Aspose.Zip](../../)


