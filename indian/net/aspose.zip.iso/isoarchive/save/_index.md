---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "IsoArchive मेथड। ISO इमेज को निर्दिष्ट पथ पर सहेजता है।"
type: docs
weight: 70
url: /hi/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

ISO इमेज को निर्दिष्ट पाथ में सहेजता है।

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | पथ जहाँ ISO इमेज सहेजी जाएगी। |
| saveOptions | IsoSaveOptions | ISO आर्काइव को सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | जब आर्काइव संपादन मोड में नहीं होता तो फेंका जाता है। |
| ArgumentNullException | जब *path* शून्य हो तो फेंका जाता है। |
| DirectoryNotFoundException | जब निर्दिष्ट पथ अमान्य हो, जैसे कि अनमैप्ड ड्राइव पर हो, तो फेंका जाता है। |
| IOException | जब फ़ाइल पहले से खुली हो तो फेंका जाता है। |
| UnauthorizedAccessException | जब फ़ाइल *path* तक पहुँच अस्वीकृत हो तो फेंका जाता है। |
| PathTooLongException | जब निर्दिष्ट *path* सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हो तो फेंका जाता है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

निम्न उदाहरण दर्शाता है कि ISO आर्काइव को फ़ाइल में कैसे सहेजा जाए:

```csharp
// एक नया खाली ISO आर्काइव बनाएं
using(IsoArchive isoArchive = new IsoArchive())
{
    // ISO आर्काइव में फ़ाइलें जोड़ें
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO आर्काइव को फ़ाइल में सहेजें
    isoArchive.Save("new_archive.iso");
}
```

### संबंधित देखें

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

ISO इमेज को निर्दिष्ट स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | स्ट्रीम जहाँ ISO इमेज सहेजी जाएगी। |
| saveOptions | IsoSaveOptions | ISO आर्काइव को सहेजने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | जब आर्काइव संपादन मोड में नहीं होता तो फेंका जाता है। |
| ArgumentNullException | जब *stream* शून्य हो तो फेंका जाता है। |
| ArgumentException | जब *stream* लिखने योग्य नहीं होता है, तब फेंका जाता है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| IOException | एक I/O त्रुटि हुई। |

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि ISO संग्रह को मेमोरी स्ट्रीम में कैसे सहेजा जाए:

```csharp

 // एक नया खाली ISO आर्काइव बनाएं
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // ISO आर्काइव में फ़ाइलें जोड़ें
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // ISO संग्रह को मेमोरी स्ट्रीम में सहेजें
     isoArchive.Save(memoryStream);
 }
```

### संबंधित देखें

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


