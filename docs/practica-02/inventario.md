# Inventario del sistema

## Objetivo

Realizar un inventario inicial del repositorio del Sistema de Control Escolar de Servicio Social y Residencia Profesional.

## Inventario

| Elemento | Archivos | Clasificación |
|---|---:|---|
| Vistas | 6992 | Código / recursos |
| Modelos | 261 | Código propio |
| impExcel | 229 | Componente externo |
| tcpdf | 108 | Librería de terceros |
| Controladores | 19 | Código propio |
| Documentos | 11 | Datos/documentos |
| PHPMailer | 6 | Librería de terceros |
| ImportarExcel | 6 | Componente funcional |
| IMSS | 5 | Módulo |
| Kardex | 5 | Módulo |
| Servicio | 4 | Módulo |
| Documentacion | 4 | Documentación |
| config | 2 | Configuración |
| expExcel | 2 | Componente |
| Ajax | 1 | Código |
| index.php | 1 | Punto de entrada |
| .htaccess | 1 | Configuración |
| importarUser.xls | 1 | Datos/documentos |
| Archivos SQL | 3 | Base de datos |

## Tipos de archivo principales

- `.js`: 3825
- `.png`: 1211
- `.svg`: 741
- `.php`: 592
- `.css`: 415
- `.html`: 163
- `.json`: 110
- `.less`: 98
- `.md`: 80
- `.gif`: 64
- `.txt`: 40
- `.scss`: 32
- `.pdf`: 27
- `.jpg`: 18

## Observaciones

La carpeta `Vistas` concentra la mayor cantidad de archivos del repositorio. También se identificaron dependencias y componentes externos como `tcpdf`, `PHPMailer` e `impExcel`.

Los conteos fueron obtenidos mediante `git ls-tree -r --name-only HEAD`.
