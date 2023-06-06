# Crea tu propio EFI Hackintosh en Ventura para un procesador de 5ta Generación (Broadwell-U) [Versión en desarrollo]
[Primeros pasos]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#primeros-pasos
[Soporte de Hardware]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#soporte-de-hardware
[Creación del EFI]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#creación-del-efi
[Solucionando Problemas]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#solucionando-problemas
[Opiniones]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md#opiniones


Esta guía está basada en mi propia experiencia intentando hacer que algunas versiones de MacOS arranquen y funcionen sobre procesadores Broadwell-U (Intels de 5ta Generación); Ahora, explicaré unos pasos/consejos a seguir:


---

Art. | Tabla de Contenido
---|:--:
1 | [Primeros Pasos]
1.1 | [Soporte de Hardware]
2 | [Creación del EFI]
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
  
#### Sobre las GPUs Discretas/Dedicadas:

Cualquier GPU de Nvidia está eliminada del soporte desde MacOS BigSur, aunque algunas gráficas de Nvidia podrían funcionar en versiones posteriores (desde BigSur); Las gráficas de bajo consumo (y de arquitecturas viejas como Fermi, Kepler y Maxwell) directamente no funcionan.
  
#### Sobre tarjetas Wi-Fi/Bluetooth:

#### Sobre tarjetas de audio (internas y externas):

**Para tarjetas internas:** En esta guía, hablaremos sobre las [tarjetas de audio soportadas por AppleALC] y cómo configurarlas en tu EFI Hackintosh.

**Para tarjetas externas:** Cuelquier tarjeta de audio DAC USB que sea compatible con Windows o MacOS podría funcionar.

</details>

## Creación del EFI

<details>
</details>

## Solucionando Problemas

<details>
</details>

## Opiniones

<details>
</details>
