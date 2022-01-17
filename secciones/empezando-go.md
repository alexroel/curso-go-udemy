# Empezando con lenguaje Go

1. [Playground de Go](#playground-de-go)
2. [Instalar Go](#instalar-go)
3. [Instalar VSCode](#instalar-vscode)
4. [Hola Mundo](#hola-mundo)
5. [Mi Primer Función](#mi-primer-función)
6. [Comentarios](#comentarios)

---
## Playground de Go
El Playground de Go, es una herramienta para probar y ejecutar código de lenguaje Go sin tener que instalar herramienta de desarrollo en nuestro computados. 
Lo podemos encontrar en su pagina oficial https://go.dev/play/

---
## Instalar Go 
Para instalar la herramienta de desarrollo de Go, solo vamos a descargar Go desde su página oficial y seguir la guía de la instalación. 
- Descargar Go: https://go.dev/dl/
- Guía de Instalación:https://go.dev/doc/install

Para trabajos con Go, tenemos 	que estructurar nuestro espacio de trabajo de la siguiente forma. 

~~~
go/
    bin/
    src/
    pkg/
~~~

- `bin/` En esta carpeta van los binarios que usemos en nuestros proyectos o los binarios que nosotros vamos a generar. 
- `src/` En esta carpeta van todos los proyectos que vamos a desarrollar con Go. 
- `pkg/` En esta carpeta van todos los paquetes que vamos usar en nuestros proyectos ya sea del lenguaje o de terceros. 


---
## Instalar VSCode
Para instalar el editor de código Visual Studio Code vamos a su página oficial para descargar y luego seguir la guía de instalación. 

Para configurar Visual Studio Code para que trabaje con Go, solo descargamos los paquetes e instalar algunas herramientas de trabajo

- [Paquete para trabajos con Go](https://marketplace.visualstudio.com/items?itemName=golang.Go)

---
### Hola Mundo

El siguiente código se muestra cómo hacer una aplicación simple de mostrar hola mundo en la consola.

~~~go
package main

import "fmt"

func main() {
	fmt.Println("Hola Mundo")
}
~~~

Para ejecutar esta aplicación y ver los resultados, tenemos que dirigirnos a nuestra terminal y ejecutar con el siguiente comando. 

- `go run` Es para ejecutar y probar nuestro código sin generar un archivo compilado. 
- `go build` Es para generar un archivo compilado lista para la producción. 

~~~
go run hola.go
~~~

~~~
go build hola.go
~~~
Para ejecutar ese archivo en windows 
~~~
hola.exe
~~~
Para ejecutar ese mismo archivo en Mac o Linux
~~~
./hola
~~~

---
## Mi Primer Función
Vamos crear nuestra primera función en Go, esta función va ser muy simple, el cual no va tener parámetros. Simplemente al llamarla va ejecutarse. 


~~~go
package main

import "fmt"

func main() {
	fmt.Println("Hola Mundo")
	saluda()
}

func saluda() {
	fmt.Println("Hola desde la Función")
}
~~~

---
## Comentarios
Para hacer los comentarios en Go se hacer con `//`, esto es para los cometarios de línea, para los comentarios de múltiples líneas se abre con `/*` y se cierra con `*/`. 

~~~go
//Esto es un comentario de linea 
/* Esto es 
comentario de 
multiples lineas */

package main //Indicar el paquete principal 

import "fmt" //Importar el paquete FMT 

//Funcion principal 
func main() {
	fmt.Println("Hola Mundo")
	saluda()//Ejecutando la funcion 
}

//Funcion que imprime un saludo
func saluda() {
	fmt.Println("Hola desde la Función")
}
~~~


