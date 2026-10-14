---
title: "Lz4Archive.SetSource"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo Lz4Archive. Imposta il contenuto da comprimere all'interno dell'archivio"
type: docs
weight: 70
url: /it/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Stream | Lo stream di input per l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | L'archivio è pronto per l'estrazione. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | Il riferimento a un file da comprimere. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | L'archivio è pronto per l'estrazione. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

Apri un archivio da uno stream ed estrailo in un `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tarArchive | TarArchive | Archivio Tar da comprimere. |
| formato | TarFormat | Definisce il formato dell'intestazione tar. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | Questo archivio è pronto per l'estrazione. |

## Osservazioni

Utilizza questo metodo per comporre un archivio tar.lz4 congiunto.

## Esempi

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Vedi anche

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Percorso del file da comprimere. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| InvalidOperationException | Questo archivio è pronto per l'estrazione. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

Apri un archivio da file tramite percorso ed estrailo in un `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


