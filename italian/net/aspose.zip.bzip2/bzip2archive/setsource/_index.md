---
title: Bzip2Archive.SetSource
second_title: Riferimento API Aspose.ZIP per .NET
description: Bzip2Archive metodo. Imposta il contenuto da comprimere allinterno dellarchivio.
type: docs
weight: 60
url: /it/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | Il flusso di input per l'archivio. |

### Esempi

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | Il riferimento a un file da comprimere. |

### Esempi

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

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

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tarArchive | TarArchive | Archivio tar da comprimere. |
| format | TarFormat | Definisce il formato dell'intestazione tar. |

### Osservazioni

Utilizzare questo metodo per comporre un archivio comune tar.bz2.

### Esempi

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### Guarda anche

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cpioArchive | CpioArchive | Archivio Cpio da comprimere. |
| format | CpioFormat | Definisce il formato dell'intestazione cpio. |

### Osservazioni

Usa questo metodo per comporre un archivio cpio.bz2 congiunto.

### Esempi

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### Guarda anche

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)


