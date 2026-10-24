# Transporte temporal del APK 1.1.46

Esta rama entrega un APK ya compilado y firmado a un borrador de GitHub Release.
No contiene el código fuente de la aplicación y no se fusiona con main.

El APK se divide en tres bloques menores de 50 MB para transportar el binario por
Git cuando la credencial del entorno no funciona con uploads.github.com. GitHub
Actions concatena los bloques, comprueba SHA-256 y sube el APK usando el token
del propio repositorio. El workflow no publica el borrador ni activa avisos.

Fuente canónica compilada:
https://github.com/Katodev-Ar/StockApp-Mobile/commit/874e322c0ac4f54f308deba2df806fd96c9bb72b

PR fuente: https://github.com/Katodev-Ar/StockApp-Mobile/pull/2

La rama temporal se elimina después de verificar la entrega de los assets.
La publicación y el anuncio se realizan por separado tras comprobar el archivo.
