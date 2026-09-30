---
title: "TarArchive.FromLZMA"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "TarArchive मेथड। प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से TarArchive बनाता है।"
type: docs
weight: 50
url: /hi/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से [`TarArchive`](../) बनाता है।

महत्वपूर्ण: LZMA आर्काइव इस मेथड के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

```csharp
public static TarArchive FromLZMA(Stream source)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| स्रोत | स्ट्रीम | आर्काइव का स्रोत। |

### रिटर्न वैल्यू

एक उदाहरण [`TarArchive`](../) का

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidDataException | आर्काइव भ्रष्ट है। |
| EndOfStreamException | जब स्ट्रीम का अंत पहुँच जाता है और अपेक्षित बाइट्स की संख्या पढ़ी नहीं जाती, तो यह अपवाद फेंका जाता है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| ArgumentNullException | *source* null है। |
| IOException | एक I/O त्रुटि हुई। |

## टिप्पणियाँ

LZMA निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है।

### संबंधित देखें

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से [`TarArchive`](../) बनाता है।

महत्वपूर्ण: LZMA आर्काइव इस मेथड के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

```csharp
public static TarArchive FromLZMA(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पथ। |

### रिटर्न वैल्यू

एक उदाहरण [`TarArchive`](../) का

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल अमान्य प्रारूप में है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| EndOfStreamException | जब स्ट्रीम का अंत पहुँच जाता है और अपेक्षित बाइट्स की संख्या पढ़ी नहीं जाती, तो यह अपवाद फेंका जाता है। |
| IOException | फ़ाइल खोलते समय एक I/O त्रुटि हुई। |
| InvalidDataException | आर्काइव भ्रष्ट है। |

## टिप्पणियाँ

LZMA निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है।

### संबंधित देखें

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


