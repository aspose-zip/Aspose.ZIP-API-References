---
title: "Bzip2Archive.ExtractToDirectory"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo Bzip2Archive. Estrae il contenuto dell'archivio nella directory fornita"
type: docs
weight: 40
url: /it/net/aspose.zip.bzip2/bzip2archive/extracttodirectory/
---
## Bzip2Archive.ExtractToDirectory method

Estrae il contenuto dell'archivio nella directory fornita.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | String | Il percorso della directory in cui posizionare i file estratti. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationDirectory* è null. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file devono essere inferiori a 260 caratteri. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere alla directory esistente. |
| NotSupportedException | Se la directory non esiste, il percorso contiene un carattere due punti (:) che non fa parte di un'etichetta di unità (\"C:\\\") |
| ArgumentException | *destinationDirectory* è una stringa di lunghezza zero, contiene solo spazi bianchi o contiene uno o più caratteri non validi. È possibile verificare i caratteri non validi utilizzando il metodo System.IO.Path.GetInvalidPathChars. -or- il percorso è prefissato da, o contiene, solo un carattere due punti (:). |
| IOException | La directory specificata dal percorso è un file. -or- Il nome di rete non è noto. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

Se la directory non esiste, verrà creata.

### Vedi anche

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


