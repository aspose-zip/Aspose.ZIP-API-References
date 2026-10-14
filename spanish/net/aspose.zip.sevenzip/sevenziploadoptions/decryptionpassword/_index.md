---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad SevenZipLoadOptions. Obtiene o establece la contraseña para descifrar entradas y nombres de entradas"
type: docs
weight: 30
url: /es/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Obtiene o establece la contraseña para descifrar entradas y nombres de entrada.

```csharp
public string DecryptionPassword { get; set; }
```

## Ejemplos

Puede proporcionar la contraseña de descifrado una vez al extraer el archivo.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
        {
            using (var decompressed = archive.Entries[0].Open())
            {
                byte[] b = new byte[8192];
                int bytesRead;
                while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
                    extracted.Write(b, 0, bytesRead);
                
            }
        }
    }
}
```

### Ver también

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


