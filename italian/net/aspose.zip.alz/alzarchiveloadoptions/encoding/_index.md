---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà AlzArchiveLoadOptions. Ottiene o imposta la codifica per i nomi delle voci. Il valore predefinito è la pagina di codice Windows coreana 949 CP949"
type: docs
weight: 40
url: /it/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Ottiene o imposta la codifica per i nomi delle voci. L'impostazione predefinita è la pagina di codice Windows coreana 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Osservazioni

Gli archivi ALZ storicamente memorizzano i nomi dei file utilizzando la pagina di codice ANSI Windows coreana.

## Esempi

Nome della voce composto utilizzando la codifica specificata.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Vedi anche

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


