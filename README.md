# Modpack-Servers (Configuración del Launcher)

Este repositorio contiene la lista blanca (whitelist) oficial de modpacks y servidores, así como los archivos individuales y configuraciones de cada uno de ellos para **MiLauncher**.

## Estructura del Repositorio

* **Rama `main` (Esta rama)**: Contiene información básica y documentación sobre cómo administrar los modpacks del launcher.
* **Rama `whitelist`**: Contiene el archivo central `whitelist.json` con la definición de todos los modpacks oficiales.
* **Rama de cada modpack (Ej: `zombie-apocalipsis`, `vanilla-plus`)**: Contiene los archivos correspondientes a cada modpack (configuraciones, mods individuales, imágenes promocionales y fondos).

---

## Cómo Añadir un Nuevo Modpack

1. **Definir el Modpack en la Whitelist**:
   Cambia a la rama `whitelist` y edita el archivo `whitelist.json` para agregar un nuevo objeto con los detalles del modpack (ID, versión, descripción, cargador de mods y rama asociada).

2. **Crear la rama del Modpack**:
   Crea una nueva rama cuyo nombre coincida con el campo `branch` definido en el `whitelist.json`.

3. **Subir los Archivos**:
   En la nueva rama del modpack, sube los siguientes archivos:
   - `config-modpack.json`: Ajustes y argumentos de inicio por defecto del cliente.
   - `custom_icon.png`: Icono personalizado visible en la lista.
   - `background-modpack.png` / `background-modpack.jpg`: Fondo promocional de la cabecera.
   - `mods/`: Directorio que contiene todos los archivos `.jar` de los mods.
