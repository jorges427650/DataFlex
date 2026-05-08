# Estado de instalacion - FutbolWebApp

Fecha: 2026-05-08

## Carpeta base

- Trabajo del proyecto: `C:\Dev\Practicas`
- Programas/instaladores: `C:\Dev\Practicas\Programas`
- Scripts SQL: `C:\Dev\Practicas\SQL`
- Workspaces DataFlex: `C:\Dev\Practicas\Workspaces`

## Preparado

- MySQL Server 8.4.8 esta instalado y el servicio `MySQL80` esta arrancado.
- El servicio `MySQL80` realmente ejecuta MySQL Server 8.0.45 desde `C:\Program Files\MySQL\MySQL Server 8.0`.
- Usuario MySQL local para la practica: `root` / `Change_Password`.
- MySQL Workbench 8.0.47 CE esta instalado.
- DataFlex 2025 Studio 25.0.30.78 esta instalado en `C:\Dev\Practicas\Programas\DataFlex 25.0`.
- El servicio `DFWAS250` de DataFlex 25.0 Web Application Server esta arrancado y en automatico.
- MySQL Connector/ODBC 9.7 de 64 bits queda instalado y registrado:
  - `MySQL ODBC 9.7 Unicode Driver`
  - `MySQL ODBC 9.7 ANSI Driver`
- El instalador y ZIP del Connector/ODBC estan guardados en `C:\Dev\Practicas\Programas`.
- El script recibido se copio sin modificar a `C:\Dev\Practicas\SQL\futbolBD.sql`.
- La base de datos antigua `futbol` se elimino y se importo de nuevo desde `C:\Dev\Practicas\SQL\futbolBD.sql`.
- Verificacion de `futbol`: 12 tablas. Recuentos principales: entrenador 7, jugador 60, posicion 6, equipo 6, liga 2.
- Workspace DataFlex creado en `C:\Dev\Practicas\Workspaces\FutbolWebApp`.
- Proyecto Web Mobile `FutbolWebApp` creado y compilado en `C:\Dev\Practicas\Workspaces\FutbolWebApp\Programs\FutbolWebApp.exe`.
- Conexion MySQL configurada con `DFCONNID=Futbol` en `C:\Dev\Practicas\Workspaces\FutbolWebApp\Data\DFConnId.ini`.
- Las 12 tablas de MySQL quedaron traidas a DataFlex mediante `.int` y `.fd`; las 5 principales tambien tienen Data Dictionaries.
- Tablas embebidas disponibles en MySQL y apuntadas desde DataFlex: `CodeMast`, `CodeType` y `WebAppSession`.
- Vistas Select y Zoom creadas para `entrenador`, `jugador`, `posicion`, `equipo` y `liga`.
- Tiles creados en `Dashboard.wo` para las cinco tablas pedidas.
- Verificacion final: `FutbolWebApp.src` compila sin errores ni warnings.

## Pendiente

- Registrar/publicar la aplicacion en IIS/Web Application Server si se quiere abrir desde navegador; esa accion suele requerir permisos de administrador.
