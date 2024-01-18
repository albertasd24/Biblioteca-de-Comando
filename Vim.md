# Vim
> Vim es un editor de código que funciona por medio de la terminal. Su forma de emplear es mediante el teclado por sus atajos
## Paso 1: Abrir un archivo con Vim

1. **Abrir una terminal:**
   - Abre una terminal en tu sistema operativo (Linux, macOS o WSL en Windows).

2. **Abrir un archivo con Vim:**
   - Puedes abrir un archivo existente con Vim utilizando el siguiente comando:
     ```bash
     vim nombre_del_archivo
     ```
   - Si el archivo no existe, Vim lo creará al guardar los cambios.

## Paso 2: Modos de Vim

Vim tiene diferentes modos que determinan su comportamiento. Los dos modos principales son el modo de comando y el modo de inserción.

- **Modo de Comando (Normal):**
  - En este modo, puedes navegar por el documento y ejecutar comandos.
  - Presiona la tecla `Esc` para asegurarte de estar en el modo de comando.

- **Modo de Inserción:**
  - En este modo, puedes escribir y editar texto.
  - Presiona `i` en el modo de comando para ingresar al modo de inserción.

## Paso 3: Navegación en el Documento

En el modo de comando:

- **Moverse por caracteres:**
  - `h`: Izquierda
  - `j`: Abajo
  - `k`: Arriba
  - `l`: Derecha

- **Saltar palabras:**
  - `w`: Siguiente palabra
  - `b`: Anterior palabra
  - `e`: Fin de palabra

- **Desplazarse por líneas:**
  - `0`: Principio de la línea
  - `$`: Fin de la línea

## Paso 4: Edición Básica

- **Insertar texto:**
  - Presiona `i` en el modo de comando para entrar en el modo de inserción.

- **Eliminar y cortar:**
  - `x`: Eliminar el carácter bajo el cursor.
  - `dd`: Cortar la línea actual.

- **Copiar y pegar:**
  - `yy`: Copiar la línea actual.
  - `p`: Pegar el texto copiado.

## Paso 5: Guardar y Salir

- **Guardar cambios:**
  - `:w`: Guardar el archivo.

- **Guardar y salir:**
  - `:wq`: Guardar y salir.
  - `ZZ`: Atajo para `:wq`.

- **Salir sin guardar:**
  - `:q!`: Salir sin guardar.

## Paso 6: Búsqueda y Reemplazo

- **Buscar:**
  - `/palabra`: Buscar la palabra hacia adelante.
  - `?palabra`: Buscar la palabra hacia atrás.
  - Presiona `n` para encontrar la siguiente coincidencia.

- **Reemplazar:**
  - `:%s/old/new/g`: Reemplazar todas las ocurrencias de "old" con "new" en todo el archivo.

## Paso 7: Otros Comandos Útiles

- **Deshacer y rehacer:**
  - `u`: Deshacer.
  - `Ctrl + r`: Rehacer.

- **Seleccionar y copiar texto:**
  - `v`: En el modo de comando, selecciona texto con las teclas de navegación y luego `y` para copiar.

Este tutorial proporciona una introducción básica a Vim. Recuerda que Vim tiene una curva de aprendizaje pronunciada, pero a medida que te acostumbras a los comandos, te volverás más eficiente. Experimenta con estos comandos y practica para mejorar tus habilidades con Vim.
