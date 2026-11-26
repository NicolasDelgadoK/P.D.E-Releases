# P.D.E

**P.D.E** es una aplicación de escritorio para Windows para establecimientos de ocio nocturno. Se instala en el computador del negocio y funciona **sin internet**: configuras tus mesas, categorías y productos, registras el consumo de cada mesa y haces el cierre de caja con el dinero por medio de pago y los productos vendidos.

Este repositorio solo contiene los instaladores y el archivo `version.json` con el que la aplicación busca actualizaciones. No tiene código.

## Descargar

Descarga siempre la última versión desde [Releases](../../releases/latest): el archivo se llama `PDE-Setup-<versión>.exe`.

Requisitos: Windows 10 o superior (64 bits). No necesitas instalar Java ni permisos de administrador.

## Instalar y activar

1. Ejecuta el instalador con doble clic. Al terminar queda un ícono de **P.D.E** en el escritorio y en el menú Inicio.
2. Abre P.D.E. La primera vez aparece la pantalla de activación con el **ID de este equipo**.
3. Pulsa **Copiar** y envíale ese ID a tu proveedor después de pagar.
4. Pega la clave de licencia que te envíe y pulsa **Activar**.

La licencia sirve solo para el computador cuyo ID enviaste. Si cambias de computador o reinstalas Windows, el ID cambia: envía el nuevo ID y te darán una clave nueva.

## Aviso de Windows ("Windows protegió su PC")

Al abrir el instalador por primera vez, Windows puede mostrar una pantalla azul que dice **"Windows protegió su PC"**. Es normal: ocurre con programas nuevos que no tienen certificado de firma de código (esos certificados tienen costo). El instalador no es un virus.

Para continuar:

1. Haz clic en **"Más información"**.
2. Haz clic en el botón **"Ejecutar de todas formas"**.
3. Sigue el instalador.

## Tus datos

Todo lo que registras se guarda en tu computador, en la carpeta `%APPDATA%\PDE\`:

- `pde.db`: la base de datos (mesas, productos, ventas y cierres).
- `fotos\`: las fotos de los productos.
- `licencia.lic`: tu licencia.
- `backups\`: copias que la aplicación hace antes de actualizar.

Instalar una versión nueva o desinstalar la aplicación **no borra** esta carpeta.

**Haz copias de seguridad con frecuencia.** En P.D.E, entra a **Historial y respaldo → Crear copia de seguridad** y guarda el archivo en una memoria USB.

Para restaurar una copia: cierra P.D.E, abre `%APPDATA%\PDE\`, reemplaza `pde.db` por la copia (renómbrala como `pde.db`) y abre P.D.E de nuevo.

## Actualizar

En P.D.E, entra a **Actualizaciones → Buscar actualizaciones**. Si hay una versión nueva, verás sus notas y el botón **Actualizar** (solo se habilita con la caja cerrada). La aplicación descarga el instalador, comprueba que sea auténtico y lo ejecuta. Tus datos y tu licencia se conservan. Al terminar, abre P.D.E con el ícono de siempre.

Las actualizaciones no se aplican solas: tú decides cuándo.
