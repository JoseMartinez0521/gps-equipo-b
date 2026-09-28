# Arquitectura del sistema

## 1. Punto de entrada

El archivo `index.php` funciona como punto de entrada principal de la aplicación.

Carga la configuración mediante `config/app.php` y posteriormente incluye diferentes controladores y modelos.

Entre ellos se encuentran los módulos de usuarios, carreras, materias, evaluaciones, visitas, chat, solicitudes de residencia y otros componentes.

También incluye los archivos de PHPMailer.

Finalmente crea un objeto `Plantilla` y ejecuta:

`$plantilla -> verPlantilla();`

## 2. .htaccess

El archivo `.htaccess` activa la reescritura de URLs mediante:

`RewriteEngine On`

La regla encontrada dirige las solicitudes hacia:

`index.php?url=$1`

Por lo tanto, `index.php` funciona como punto central de entrada de las solicitudes.

## 3. Ejemplo del patrón MVC

Se analizaron los siguientes archivos:

- `Controladores/carrerasC.php`
- `Modelos/carrerasM.php`

El controlador `CarrerasC` contiene operaciones para:

- Crear carreras.
- Consultar carreras.
- Editar carreras.
- Actualizar carreras.
- Eliminar carreras.

El controlador utiliza métodos de `CarrerasM`.

El modelo `CarrerasM` utiliza `ConexionBD` y PDO para realizar operaciones sobre la base de datos.

Se identificaron operaciones:

- INSERT
- SELECT
- UPDATE
- DELETE

## 4. Flujo general

El flujo identificado es:

Navegador

↓

.htaccess

↓

index.php

↓

Controladores

↓

Modelos

↓

ConexionBD / PDO

↓

Base de datos

## 5. Ejemplo de flujo de carreras

`Controladores/carrerasC.php`

↓

`Modelos/carrerasM.php`

↓

`ConexionBD`

↓

Base de datos

## 6. Dependencias identificadas

El repositorio contiene componentes externos como:

- `PHPMailer`
- `tcpdf`
- `impExcel`

También se identificó una gran cantidad de archivos JavaScript, imágenes, hojas de estilos y otros recursos dentro del repositorio.

## 7. Conclusión

La estructura observada presenta una separación entre controladores y modelos que corresponde al patrón MVC.

Los controladores contienen la lógica relacionada con las operaciones de la aplicación, mientras que los modelos concentran las operaciones relacionadas con el acceso a los datos.

El archivo `index.php` funciona como punto de entrada y `.htaccess` participa en el direccionamiento de las solicitudes.
