[Guía de Ventura]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md
[Problemas de incompatibilidad con Metal]: https://github.com/dortania/OpenCore-Legacy-Patcher/issues/1076
[OpenCore Legacy Patcher]: https://github.com/dortania/OpenCore-Legacy-Patcher
[itlwm]: https://github.com/OpenIntelWireless/itlwm/releases/download/v2.2.0/itlwm_v2.2.0_stable.kext.zip
[HeliPort]: https://github.com/OpenIntelWireless/HeliPort


# Crea tu propio EFI Hackintosh en Sonoma para un procesador de 5ta Generación (Broadwell-U) [Versión en desarrollo]

Resumen: Seguir la [Guía de Ventura], pues, de momento MacOS Sonoma está en Beta; las diferencias palpables serán añadidas abajo.

### Sobre el Hardware:

Apple ha eliminado con la salida de MacOS 14 (Sonoma) aún más hardware, siendo oficialmente compatibles procesadores Coffee Lake (8va generación de Intel) y superiores.

Acabando así por completo el soporte para procesadores y gráficas Skylake X y Kaby Lake (7ma Generación).

En cuanto a lo que nos compete (Hackintosh), todos los procesadores Skylake e inferiores están completamente eliminados del soporte oficial de MacOS, por lo cual, sería recomendable no actualizar a versiones superiores a MacOS 12.x.x (Monterey); pero si en todo caso queremos probar esta primera Beta, los consejos y pasos a seguir son los siguientes:

1. Cambiar SMBIOS: La recomendación sería usar una de las siguientes (para laptop):

SMBIOS | Hardware
--- | :--:

MacBookPro15,1 | Coffee Lake, UHD 630
MacBookPro15,2 | Coffee Lake, Iris Plus 655    
MacBookPro15,3 | Coffee Lake, UHD 630  
MacBookPro15,4 | Coffee Lake, Iris Plus 645   
MacBookPro16,1 | Coffee Lake, UHD 630
MacBookPro16,2 | Ice Lake, Iris Plus G4/G7     
MacBookPro16,3 | Coffee Lake, Iris Plus 645  
MacBookPro16,4 | Coffee Lake, UHD 630

---


**Con cualquiera de éstas lo más seguro es que el sistema inicie**


2. Olvidarse de la aceleración 3D (por ahora): Para aquellos que tenemos hardware más antiguo, [OpenCore Legacy Patcher] será nuestra solución en cuanto al problema de las GPUs; pero, hasta que no estén resueltos los [Problemas de incompatibilidad con Metal]; tendremos que prescindir, sí o sí de la acelereación 3D y acostumbrarnos a usar los drivers genéricos **VESA**; en este caso, agregando a nuestro boot-args: **-igfxvesa**.


3. Acostumbrarse a usar HeliPort (por ahora): Con toda la eliminación de Hardware, Apple ha quitado soporte a las tarjetas de red de Broadcom de forma definitiva; en cambio, con las de Intel, aún podemos tener Wi-Fi vía [itlwm] junto con [HeliPort].


4. Solucionar problemas de audio: Como buena versión beta que se respete, nos dejará la tarjeta de audio sin funcionar, por más que se muestre activa; si vienes de Ventura y ya la habías hecho funcionar perfectamente; sólo añade en boot-args: **-lilubetaall** y **-alcbeta** en tu config.plist para Sonoma.
