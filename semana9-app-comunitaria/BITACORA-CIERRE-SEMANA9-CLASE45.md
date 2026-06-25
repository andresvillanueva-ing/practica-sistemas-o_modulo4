# Bitácora de cierre - Semana 9 - Clase 45

## Datos generales

Nombre:
Fecha:
Entorno: GitHub Codespaces
Rama de trabajo: clase-45-cierre-git-integrador

## 1. Verificación de aplicación

Comando usado para levantar la aplicación: npx pm2 start server.js --name app-semana9

Respuesta de /estado: {"estado":"activo","mensaje":"La aplicación está disponible"}

Respuesta de /diagnostico: {"error":"Ruta no encontrada","mensaje":"Verifique la dirección consultada."}

Respuesta de /api/info: {"programa":"Capacitación en Democracia y Tecnología","alias":"Programadores para la Paz","semana":9,"clase":42,"tema":"Seguridad operativa aplicada"}

## 2. Variables de entorno

¿Qué variables se usaron?
Se utilizaron variables almacenadas en el archivo .env, como configuraciones sensibles y datos que permiten ejecutar la aplicación sin escribir directamente valores privados en el código.

¿Por qué .env no debe subirse?
Porque puede contener información sensible como contraseñas, tokens, claves API o configuraciones privadas que podrían comprometer la seguridad del sistema.

## 3. Seguridad operativa

¿Qué medidas de seguridad se aplicaron durante la semana?
Se aplicaron medidas como:

Uso de variables de entorno.
Protección del archivo .env mediante .gitignore.
Control de procesos con PM2.
Revisión de logs para detectar errores.
Documentación del procedimiento de despliegue.

## 4. Diagnóstico

¿Qué error simulado se trabajó durante la semana?
Se simuló una falla de ejecución de la aplicación mediante un problema en el proceso del servidor para comprobar la recuperación y monitoreo.

¿Cómo se corrigió?
Se revisaron los logs, se identificó el problema y se reinició el proceso utilizando PM2: pm2 restart app-semana9

## 5. Documentación

¿Qué documento explica el procedimiento de despliegue?
El procedimiento está explicado en el documento de documentación técnica o bitácora de despliegue del proyecto, donde se detallan los comandos para instalar, ejecutar y verificar la aplicación.

## 6. Git

¿Qué aprendí sobre ramas?
Aprendí que las ramas permiten trabajar diferentes versiones del proyecto sin afectar la rama principal, facilitando la organización del desarrollo.

¿Qué aprendí sobre stash?
Aprendí que git stash permite guardar temporalmente cambios no confirmados para cambiar de rama o realizar otras tareas sin perder el trabajo realizado.

¿Qué aprendí sobre merge fast-forward?
Aprendí que ocurre cuando la rama principal puede avanzar directamente hasta la última versión de otra rama porque no existen cambios diferentes entre ellas.

¿Qué aprendí sobre merge no-fast-forward?
Aprendí que sucede cuando Git necesita unir dos historiales diferentes porque ambas ramas tienen cambios independientes.

¿Qué aprendí sobre conflictos?
Aprendí que los conflictos aparecen cuando Git no puede decidir automáticamente qué cambios conservar, por lo que el desarrollador debe revisar y solucionar manualmente las diferencias.

## 7. Reflexión final

¿Qué fue lo más importante de la Semana 9?
Lo más importante fue aprender a preparar una aplicación para un entorno más cercano a producción, utilizando herramientas como PM2, variables de entorno, documentación técnica y buenas prácticas con Git para garantizar estabilidad, seguridad y facilidad de mantenimiento.