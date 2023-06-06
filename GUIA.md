# Crea tu propio EFI Hackintosh en Ventura para un procesador de 5ta Generación (Broadwell-U) [Versión en desarrollo]
[Primeros pasos]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#primeros-pasos
[Soporte de Hardware]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#soporte-de-hardware
[Creación de SSDTs]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#creación-de-ssdts
[Solucionando Problemas]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#solucionando-problemas
[Opiniones]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#opiniones


Esta guía está basada en mi propia experiencia intentando hacer que algunas versiones de MacOS arranquen y funcionen sobre procesadores Broadwell-U (Intels de 5ta Generación); Ahora, explicaré unos pasos/consejos a seguir:


---

Art. | Tabla de Contenido
---|:--:
1 | [Primeros Pasos]
1.1 | [Soporte de Hardware]
2 | [Creación de SSDTs]
3 | [Solucionando Problemas]
4 | [Opiniones]
---

**En mi caso, usaré como base mi laptop (Acer Aspire E5-572G/TravelMateP246-MG)**


![img](https://i.imgur.com/YKIPyaT.png)

---
## Primeros Pasos

<details>

### Soporte de Hardware
 
---
#### Sobre los procesadores/tarjetas gráficas integradas:

Cualquier procesador Broadwell-U (5ta Generación) está soportado hasta MacOS Monterey; en Ventura, dichos procesadores (y gráficas) han sido eliminados del soporte.
Pero, basandonos en la Guía de Dortania, podemos parchar falsamente nuestros PCs para intentar correr MacOS Ventura.

En ese caso, los procesadores con posible soporte (en este guía, al menos), serían los siguientes:
 
**DISPOSITIVOS SOPORTADOS**:
 
Línea del procesasor | Gráficos
--- | :--:
Serie Core i7 (U, HQ) | HD 5500/5600/6000, Iris 6100 e Iris Pro 6200
Serie Core i5 (U, H) | HD 5500/6000, Iris 6100 e Iris Pro 6200
Serie Core i3 (U) | HD 5500 e Iris 6100
---
 
 
**DISPOSITIVOS NO SOPORTADOS NATIVAMENTE**: 
 
Línea del procesasor | Gráficos
 --- | :--:
Serie Pentium (U) | HD 4100 (Por darle un nombre; Intel los llama solamente HD Graphics)
Serie Celeron (U) | HD 4100 (Por darle un nombre; Intel los llama solamente HD Graphics)
 
Los procesadores Pentium y Celeron no tienen un framebuffer real para MacOS. Si realmente quieres intentar usarlo, puedes intentar pacharlo como un Intel HD Graphics 4000 (de la 4ta Generación, Haswell).
 
---
  
#### About dedicated/external graphic cards:

Any Nvidia GPUs are dropped from MacOS BigSur, although some Nvidia graphics may be works on latest MacOS versions, the Low Power devices (and older architectures, like Fermi, Kepler and Maxwell) don't works.
  
#### About wireless/bluetooth cards:

#### About audio cards (internal and external):

**For Internal:** In this guide, we talking about [AppleALC's supported cards] and how config it in our Hackintosh EFI.

**For External:** Any USB Audio Card DAC what is compatible with MacOS or Windows may be work.

</details>

## Creación de SSDTs

<details>
</details>

## Solucionando Problemas

<details>
</details>

## Opiniones

<details>
</details>
