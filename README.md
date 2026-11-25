# Mr Tasty · App del local — distribución

Instalador de Windows de la app del local de Mr Tasty: mide los tiempos de atención en el
mostrador con la cámara del local y los envía al Admin.

**Descargar la última versión:** [Releases](../../releases/latest) → `MrTastyLocal-Setup-<versión>.exe`.

Cada versión se publica sola desde el repositorio del proyecto cuando un cambio en la app pasa
todos los tests. Este repositorio solo contiene los instaladores.

## Instalar en una PC nueva

1. Bajá `MrTastyLocal-Setup-<versión>.exe` del último release y ejecutalo (pide permisos de
   administrador: se instala para todos los usuarios de la PC).
2. Abrí **Mr Tasty Local**. La primera vez arranca el asistente: cámara, vínculo con el Admin,
   zonas y una prueba.

Requisitos: Windows 10 u 11 de 64 bits. Con placa de video Intel la detección anda mejor.

## Actualizaciones

La app se actualiza sola. Cada 30 minutos revisa si hay una versión nueva; si la hay, la baja,
espera a que no haya ningún cliente en curso, instala y vuelve a abrir la medición. El corte
dura alrededor de un minuto. El registro queda en `C:\ProgramData\MrTastyLocal\logs\updater.log`.

Cada instalador está firmado: la app rechaza cualquier actualización que no tenga la firma del
proyecto.

## Qué se guarda en la PC

La configuración, las zonas y la evidencia de auditoría quedan en `C:\ProgramData\MrTastyLocal`.
Actualizar o reinstalar no las borra. El video se procesa en la PC: no se graba ni se envía.
