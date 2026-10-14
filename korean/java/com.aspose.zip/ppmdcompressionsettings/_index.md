---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브 내 PPMd 압축에 대한 설정."
type: docs
weight: 93
url: /ko/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

ZIP 아카이브 내 PPMd 압축에 대한 설정.

PPMd는 Dmitry Shkarin이 개발한 데이터 압축 알고리즘입니다. 이 알고리즘은 다중 순서 컨텍스트에서 예측 구문 매칭을 기반으로 합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | 새 인스턴스를 초기화합니다. [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) 클래스. |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | 기본 모델 순서와 서브 할당자 크기를 사용하여 새 인스턴스를 초기화합니다. [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | 모델의 순서를 가져옵니다. |
| [getSuballocatorSize()](#getSuballocatorSize--) | 서브 할당자 크기를 MB 단위로 가져옵니다. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


새 인스턴스를 초기화합니다. [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) 클래스.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

기본 모델 순서는 8이며, 서브 할당자 크기는 50MB입니다.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


모델의 순서를 가져옵니다.

**Returns:**
int - 모델의 순서
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


서브 할당자 크기를 MB 단위로 가져옵니다.

**Returns:**
int - 서브 할당자 크기(MB 단위)
