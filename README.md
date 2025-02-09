# Servidor Web en Java

Este es un servidor web simple escrito en Java que permite servir archivos estáticos a través del protocolo HTTP. El servidor escucha en el puerto 6789 y maneja múltiples solicitudes concurrentemente utilizando un pool de hilos.

## Requisitos
- Java Development Kit (JDK) instalado.

## Estructura del Proyecto
El proyecto consta de dos clases principales:
1. **ServidorWeb**: Inicia el servidor y acepta conexiones entrantes.
2. **SolicitudHttp**: Maneja cada solicitud HTTP de manera independiente.

## Instrucciones de Uso

### Compilar el código
Ejecuta el siguiente comando en la terminal dentro del directorio donde se encuentra el código fuente:
```sh
javac ServidorWeb.java
```

### Ejecutar el servidor
Ejecuta el siguiente comando:
```sh
java ServidorWeb
```

### Acceder al servidor
Abre un navegador web e ingresa la siguiente URL:
```
http://localhost:6789/index.html
```

El servidor intentará servir el archivo `index.html` si está presente en el mismo directorio donde se ejecuta el servidor.

## Características
- Soporte para archivos estáticos (`.html`, `.gif`, `.jpeg`, `.jpg`).
- Manejo de solicitudes concurrentes con `ExecutorService`.
- Respuesta con código `404 Not Found` si el archivo solicitado no existe.

## Notas
- Asegúrate de que el archivo solicitado se encuentre en el mismo directorio donde se ejecuta el servidor.
- Puedes modificar el puerto cambiando la variable `puerto` en la clase `ServidorWeb`.

## Estudiante
  Deiner Julian Motta
