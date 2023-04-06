---
title: XarDirectoryEntry.ExtractToDirectory
second_title: Riferimento API Aspose.ZIP per .NET
description: XarDirectoryEntry metodo. Estrae tutti i file nella directory corrente nella directory fornita.
type: docs
weight: 50
url: /it/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Estrae tutti i file nella directory corrente nella directory fornita.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | String | Il percorso della directory in cui inserire i file estratti. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | percorso è nullo |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per accedere alla directory esistente. |
| NotSupportedException | Se la directory non esiste, il percorso contiene un carattere di due punti (:) che non fa parte di un'etichetta di unità ("C:\"). |
| ArgumentException | path è una stringa di lunghezza zero, contiene solo spazi vuoti o contiene uno o più caratteri non validi. È possibile eseguire query per caratteri non validi utilizzando il metodo System.IO.Path.GetInvalidPathChars. -oppure- path è preceduto o contiene solo un carattere due punti (:). |
| IOException | La directory specificata da path è un file. - oppure - Il nome della rete non è noto. |

### Osservazioni

Se la directory non esiste, verrà creata.

### Esempi

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.Directories.First().ExtractToDirectory("C:\\extracted");
}
```

### Guarda anche

* class [XarDirectoryEntry](../)
* spazio dei nomi [Aspose.Zip.Xar](../../xardirectoryentry/)
* assemblea [Aspose.Zip](../../../)


