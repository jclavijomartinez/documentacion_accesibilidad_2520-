# 🧭 Guía rápida: Configuración inicial de Kolibri

Esta guía te ayudará a realizar los primeros pasos para iniciar Kolibri por primera vez y dejarlo listo para su uso en un entorno educativo.

---

## Paso 1: Acceder a la IP donde está Kolibri

1. Abrir el navegador web de tu preferencia
2. Ingresar a la IP asignada al servidor.  
   Ejemplo: `http://192.168.1.101:8080`

![Acceso a IP](https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/1ingresoaPlataforma.png)

---

## Paso 2: Configurar el idioma predeterminado

1. Selecciona el idioma en el que va a estar kolibri, como el contenido del curso está en español, es el recomendado.

![idioma]( https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/2idioma.png)

## Paso 3: Configurar tipo de centro donde estará kolibri

1. Selecciona si Kolibri estará en una biblioteca, centro juvenil u otro entorno.
2. La recomendación es poner la opcion formal y de nombre: Biblioteca Alfonso Borrero Cabal S.J.

![Tipo de establecimiento]( https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/3tipoDeLugar.png)

---

## Paso 4: Configurar el accesso como invitado

1. La recomendación es que SI, se permita ver el contenido sin iniciar sesion o crear cuenta

![Configuración de cuentas]( https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/4accesoComoInvitado.png)

---

## Paso 5: Permitir a cualquiera crear una cuenta de estudiante

1. La recomendación para este numeral es que los administradores tengan que crear las cuentas de estudiantes, poner NO.

![Modo de acceso]( https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/5cuentaEstudiante.png)

---

## Paso 6: Activar contraseñas en las cuentas de estudiantes

1. La recomendación para este numeral es que, como se busca que cualquiera tenga acceso al contenido del curso, poner NO.

![Modo de acceso]( https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/6contrase%C3%B1ascuentasest.png)

---

## Paso 7: Crear la cuenta de superusuario

1. Crea la cuenta de **superadministrador**: esta tendrá control total sobre la plataforma. proporcionar nombre completo, crear el nombre para el super usuario y la contraseña. TENER MUY EN CUENTA CREAR CONTRASEÑAS SEGURAS.

![Modo de acceso]( https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/7cuentaSuperusuario.png)

---

## ✅ Paso 8: Importar el contenido

1. Desde el panel del dispositivo, selecciona la opción **"Importar"**.

2. Puedes importar contenido desde:  
   - Kolibri Studio (si hay acceso a internet)  
   - Red local  
   - Unidad de almacenamiento conectada  

   ![Fuentes de importación](https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/8punto2fuentesImportacion.png)

3. Para importar el contenido de este curso, ingresa el token `zazuz-kogan` en el campo correspondiente.  

   ![Token](https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/8punto3punto1token.png)

   ![ingresar token](https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/8punto3punto2token.png)

4. Selecciona la carpeta donde está el contenido del curso y haz clic en **"Importar"**.  

   ![Seleccionar carpeta](https://raw.githubusercontent.com/jclavijomartinez/documentacion_accesibilidad_2520-/refs/heads/master/8punto4carpeta.png)

5. Espera a que se descarguen los recursos desde internet y haz clic en **"Cerrar"** cuando finalice.

---

- 📝 **Sugerencia:** Una vez configurado, revisa los roles asignados y realiza una prueba de navegación como estudiante.

- 📝 **Sugerencia 2:** Si alguna vez la plataforma falla, y puedes verificar que el problema es el contenedor, el flujo a seguir es el siguiente:
  - Apagar el contenedor con el comando `docker compose down`
  - borrar la carpeta data con el comando `sudo rm -rf data/`
  - volver a instanciar el contenedor con el comando `COMPOSE_BAKE=true docker compose up -d --build --force-recreate`
  - Con estos pasos debería bastar para que todo vuelva a estas bien, debes dirigirte al paso 1 de esta documentación
