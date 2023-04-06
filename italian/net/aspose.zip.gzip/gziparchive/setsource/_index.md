---
title: GzipArchive.SetSource
second_title: Riferimento API Aspose.ZIP per .NET
description: GzipArchive metodo. Imposta il contenuto da comprimere allinterno dellarchivio.
type: docs
weight: 70
url: /it/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | Il flusso di input per l'archivio. |

### Esempi

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | Il riferimento a un file da comprimere. |

### Esempi

Apri un archivio da uno stream ed estrailo in un file`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Percorso del file da comprimere. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Esempi

Apri un archivio dal file per percorso ed estrailo in a`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tarArchive | TarArchive | Archivio tar da comprimere. |

### Osservazioni

Utilizzare questo metodo per comporre un archivio comune tar.gz.

### Esempi

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Guarda anche

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)


