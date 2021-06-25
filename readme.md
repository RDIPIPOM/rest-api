# Todos API

Edgar Marcelino Zamora Cruz 6°K

El presente proyecto tiene la misión de servir como un servidor tipo rest que puede ofrecer la consulta de pendientes llamadas "todos".


## Installation
Primeramente deberás descargar todos los archivos desde el repositorio de github con el siguiente comando:
```git clone https://github.com/RDIPIPOM/rest-api.git```

Para poner en funcionamiento desde IntelliJ IDEA basta con abrir el archivo App ubicado en \src\main\java\mx\ucol\ y presionar Ctrl+Mayús+F10 para correrlo.
También existe una manera de correrlo desde la línea de comandos (a mí no me funcionó pero puede ser problema de mi máquina) ejecutando los siguientes comandos:

```mvn assembly:assembly package```

Posteriormente ejecutamos el JAR con dependencias:

```java -jar target/rest-server-1.0-SNAPSHOT-jar-with-dependencies.jar```

Es necesario resaltar que el servidor correrá a través del puerto 8000 y éste puede ser cambiado desde el archivo App

## Endpoints

La API solo cuenta con un solo endpoint:

```api/v1/todos```: Devuelve todos los registros de la tabla todos (pendintes)

## Usage

Para hacer uso del endpoint mencionado podemos hacer uso de la herramienta curl

```curl localhost:8000/api/v1/todos```

que nos debería de retornar la siguiente respuesta:

```
{
   id: 1,
   title: "First ToDo",
   completed: false,
}
```

**Don't forget to attach the screenshots of your clients**
