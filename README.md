

```markdown
# Proyecto de modelado 3d 

Este proyecto es un ejemplo de un renderizador gráfico simple utilizando Rust y algunas bibliotecas como `nalgebra_glm` y `minifb`. A continuación se detallan las instrucciones para configurar y ejecutar el proyecto.

## Requisitos

Asegúrate de tener instalado Rust y Cargo. Puedes instalar Rust siguiendo las instrucciones en [rustup.rs](https://rustup.rs/).

## Inicialización del Proyecto

Si aún no has inicializado el proyecto, puedes hacerlo con el siguiente comando:

```bash
cargo init nombre_del_proyecto
```

Esto creará una nueva carpeta con el nombre del proyecto y generará un archivo `Cargo.toml` y un directorio `src`.

## Estructura de Archivos

El proyecto tiene la siguiente estructura de archivos:

```
nombre_del_proyecto/
├── Cargo.toml
└── src/
    ├── main.rs
    ├── framebuffer.rs
    ├── triangle.rs
    ├── line.rs
    ├── vertex.rs
    ├── obj.rs
    ├── color.rs
    ├── fragment.rs
    └── shaders.rs
```

- **Cargo.toml**: Archivo de configuración del proyecto que incluye las dependencias.
- **src/main.rs**: Punto de entrada del programa donde se inicializa la ventana y se ejecuta el bucle principal.
- **src/framebuffer.rs**: Módulo que maneja el framebuffer para el renderizado.
- **src/triangle.rs**: Módulo que contiene funciones relacionadas con el manejo de triángulos.
- **src/line.rs**: Módulo para el manejo de líneas (si es necesario).
- **src/vertex.rs**: Módulo que define la estructura de los vértices.
- **src/obj.rs**: Módulo para cargar y manejar archivos OBJ.
- **src/color.rs**: Módulo que define colores y conversiones.
- **src/fragment.rs**: Módulo que maneja los fragmentos generados durante el renderizado.
- **src/shaders.rs**: Módulo que contiene los shaders utilizados en el renderizado.

## Compilación y Ejecución

Para compilar y ejecutar el proyecto, utiliza el siguiente comando:

```bash
cargo run --release
```

El flag `--release` compila el proyecto en modo de liberación, lo que optimiza el rendimiento.

## Dependencias

Asegúrate de agregar las siguientes dependencias en tu archivo `Cargo.toml`:

```toml
[dependencies]
nalgebra-glm = "0.15"  # Para operaciones matemáticas
minifb = "0.22"        # Para la creación de ventanas y manejo de eventos
tobj = "4.0.2"         # Para cargar archivo del tipo obj
```

## Control de Entrada

El programa permite controlar la posición, rotación y escala del objeto utilizando las siguientes teclas:

- **Flecha derecha**: Mover a la derecha
- **Flecha izquierda**: Mover a la izquierda
- **Flecha arriba**: Mover hacia arriba
- **Flecha abajo**: Mover hacia abajo
- **S**: Aumentar escala
- **A**: Disminuir escala
- **Q**: Rotar hacia la izquierda (eje X)
- **W**: Rotar hacia la derecha (eje X)
- **E**: Rotar hacia la izquierda (eje Y)
- **R**: Rotar hacia la derecha (eje Y)
- **T**: Rotar hacia la izquierda (eje Z)
- **Y**: Rotar hacia la derecha (eje Z)
- **Escape**: Salir del programa

## Contribuciones

Las contribuciones son bienvenidas. Si deseas contribuir, por favor abre un issue o un pull request.

## MI nave obj

![image](https://github.com/user-attachments/assets/18bb3549-6ed6-4a09-8232-a37239e887be)

```
