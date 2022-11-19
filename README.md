# The Rust Programming Language
Proyecto en el que seguiré los pasos el libro oficial de Rust https://doc.rust-lang.org/book


## Installation
Visitar https://www.rust-lang.org/tools/install e instalar la versión recomendada para tu SO

Instalar y ejecutar los siguientes comandos

> rustup toolchain install stable-x86_64-pc-windows-gnu  

> rustup default stable-x86_64-pc-windows-gnu

rustup es un programa de línea de comando que sirve para gestionar las versiones de rust.

Comprobamos que se ha instalado correctamente:
> rustc --version
> cargo --version

## Getting Started

Crear carpeta para el proyecto 
> mkdir rust-demo
> cd rust-demo

Creamos fichero main.rs con la siguiente función:
```
fn main() {
    println!("Hello, world!");
}
```

Todo programa Rust debe de contener una función "fn" main.

### Compilando fichero main.rs con rustc

    rustc main.rs
    .\main.exe

### Mejor gestionar el proyecto con un gestor de paquetes, CARGO!

Cargo es el gestor de paquetes oficial de rust y nos ayuda con los siguientes comandos:

```
cargo new nombre_proyecto 
cargo build
cargo run
```

NOTAS:
- Cargo genera carpeta target con los ficheros compilados, entre ellos el .exe
- Ruta de fichero compilado: target\debug\nombre_proyecto.exe
- Usa fichero Cargo.toml para gestionar las propiedades y dependencias del proyecto
- Ejemplo de fichero Cargo.toml que se genera:
  
    ```
    [package]
    name = "rust-demo"
    version = "0.1.0"
    edition = "2021"

    # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

    [dependencies]
    ```

#### NEW:

Para crear un nuevo proyecto.

```
cargo new nombre_proyecto 
```

Genera:
- Carpeta con nombre del proyecto indicado
- Carpeta src con fichero y función main
- Crea repositorio git con fichero .gitignore
- Fichero Cargo.toml

#### BUILD:

Para compilar el proyecto

```
cargo build
```

Genera:
- Carpeta target

#### RUN:

Para compilar y ejecutar el proyecto

```
cargo run
```

- Genera carpeta target
- Ejecuta .exe





