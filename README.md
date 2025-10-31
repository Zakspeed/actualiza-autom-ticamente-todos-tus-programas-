# actualiza-autom-ticamente-todos-tus-programas-

Este comando actualiza **todos los programas** instalados en tu sistema usando **Windows Package Manager (winget)**. Aquí te explico cada parámetro:
```
winget upgrade --all --include-unknown --silent --disable-interactivity --accept-package-agreements --accept-source-agreements
```
## Desglose del comando:

- **`winget upgrade`** - Comando para actualizar paquetes
- **`--all`** - Actualiza TODOS los programas que tengan actualizaciones disponibles
- **`--include-unknown`** - Incluye programas cuya versión actual no puede determinarse con certeza
- **`--silent`** - Instalación silenciosa (sin ventanas ni diálogos)
- **`--disable-interactivity`** - Desactiva cualquier solicitud de confirmación del usuario
- **`--accept-package-agreements`** - Acepta automáticamente los acuerdos de licencia de los paquetes
- **`--accept-source-agreements`** - Acepta automáticamente los acuerdos de las fuentes (repositorios)

## En resumen:

El script actualiza **automáticamente** todos tus programas sin pedir confirmación, sin mostrar ventanas y aceptando todas las licencias automáticamente. Es útil para:

✅ Mantener el sistema actualizado sin intervención manual
✅ Automatizar actualizaciones (por ejemplo, en un script programado)
✅ Actualizar múltiples programas de una sola vez

## ⚠️ Consideración:

Este comando acepta **todas** las licencias automáticamente sin que las leas. Si prefieres revisar qué se va a actualizar antes, usa:
```batch
winget upgrade --all
```
(Sin los parámetros de aceptación automática)
