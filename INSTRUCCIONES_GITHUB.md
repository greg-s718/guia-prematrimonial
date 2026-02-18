# 📚 GUÍA PREMATRIMONIAL - INSTRUCCIONES DE DESPLIEGUE EN GITHUB PAGES

## 🎯 RESUMEN

Tienes 3 archivos listos para desplegar en GitHub Pages:
1. `index.html` - La guía completa interactiva
2. `sw.js` - Service Worker para funcionalidad offline  
3. Este archivo README con instrucciones

## 🚀 PASO 1: CREAR REPOSITORIO EN GITHUB

1. Ve a https://github.com
2. Haz clic en el botón verde "New" (Nuevo repositorio)
3. Nombra tu repositorio: `guia-prematrimonial` (o el nombre que prefieras)
4. Marca como **Public** (público) para que funcione con GitHub Pages gratis
5. NO marques "Add a README file"
6. Haz clic en "Create repository"

## 📤 PASO 2: SUBIR LOS ARCHIVOS

### Opción A: Subir directamente en GitHub (MÁS FÁCIL)

1. En tu nuevo repositorio, haz clic en "uploading an existing file"
2. Arrastra los 2 archivos:
   - `index.html`
   - `sw.js`
3. En el campo "Commit changes", escribe: "Versión inicial de la guía"
4. Haz clic en "Commit changes"

### Opción B: Usar Git desde tu computadora

```bash
# En tu terminal:
cd /ruta/donde/guardaste/los/archivos
git init
git add index.html sw.js
git commit -m "Versión inicial de la guía"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/guia-prematrimonial.git
git push -u origin main
```

## 🌐 PASO 3: ACTIVAR GITHUB PAGES

1. En tu repositorio, haz clic en "Settings" (Configuración)
2. En el menú izquierdo, haz clic en "Pages"
3. En "Source", selecciona "Deploy from a branch"
4. En "Branch", selecciona "main" y carpeta "/ (root)"
5. Haz clic en "Save"
6. ¡Espera 1-2 minutos!

## ✅ PASO 4: OBTENER TU URL

Después de 1-2 minutos, recarga la página de Settings → Pages

Verás un mensaje verde:
**"Your site is live at https://TU-USUARIO.github.io/guia-prematrimonial/"**

**¡Esa es la URL que compartirás con la pareja!** 🎉

## 📱 CÓMO USAR LA GUÍA

### Para la Pareja:

1. Abre la URL en cualquier navegador (Safari, Chrome, etc.)
2. Funciona en teléfonos, tablets y computadoras
3. Funciona OFFLINE después de la primera carga
4. Pueden añadirla a su pantalla de inicio como una app

#### En iPhone/iPad:
- Safari → Compartir → "Añadir a pantalla de inicio"

#### En Android:
- Chrome → Menú (⋮) → "Añadir a pantalla de inicio"

### Características Interactivas:

- **📝 Resaltar texto:** Clic en cualquier párrafo
  - Amarillo = Importante
  - Verde = Completado
  - Rosa = Preguntas

- **✅ Marcar progreso:** Casillas de verificación

- **💾 Guardar progreso:** Botón "Guardar Mi Progreso"
  - Descarga archivo JSON
  - Pueden guardarlo en Drive/iCloud/email
  - Restaurar con "Restaurar Progreso"

- **📊 Ver resumen:** Botón "Mis Destacados"
  - Ve todo lo resaltado organizado por color

## 🔄 CÓMO ACTUALIZAR EL CONTENIDO (IMPORTANTE)

Cuando quieras añadir o modificar contenido:

### Método 1: Directamente en GitHub (MÁS FÁCIL)

1. Ve a tu repositorio en GitHub
2. Haz clic en `index.html`
3. Haz clic en el ícono del lápiz ✏️ (Edit)
4. Haz los cambios que necesites
5. Scroll hacia abajo
6. En "Commit changes", describe qué cambiaste
7. Haz clic en "Commit changes"
8. **Los cambios aparecerán en 1-2 minutos en la URL**

### Método 2: Pedirle a Claude que actualice

1. Ven a este chat de Claude
2. Di: "Claude, añade una nueva sección sobre [TEMA] al Capítulo [X]"
3. Claude te dará el código actualizado
4. Copia el código nuevo
5. Ve a GitHub → index.html → Edit
6. Reemplaza el contenido
7. Commit changes

**Ejemplo:**
```
Tú: "Claude, añade una sección sobre 'Manejo del Estrés Ministerial' 
     al Capítulo 10"

Claude: [Te dará el HTML actualizado]

Tú: Copias y pegas en GitHub
```

## 💾 DÓNDE SE GUARDAN LOS DATOS

### iPhone/iPad:
- **Ubicación:** Safari → Local Storage
- **Persistencia:** Se mantiene mientras no borren datos de Safari
- **Backup:** Usar botón "Guardar Mi Progreso"

### Android:
- **Ubicación:** Chrome → Local Storage  
- **Persistencia:** Se mantiene mientras no borren datos de Chrome
- **Backup:** Usar botón "Guardar Mi Progreso"

### ⚠️ IMPORTANTE:
Si borran el historial/datos del navegador, perderán su progreso.
**SIEMPRE recomienda usar "Guardar Mi Progreso" regularmente.**

## 🔐 PRIVACIDAD

- ✅ Los destacados/notas se guardan SOLO en el dispositivo de ellos
- ✅ NADA se envía a internet
- ✅ Solo ellos pueden ver su progreso
- ✅ Cada dispositivo tiene su propio progreso
- ✅ Pueden transferir progreso entre dispositivos con Export/Import

## 🎨 PERSONALIZACIÓN FUTURA

Si quieres cambiar colores, fuentes, o diseño:

1. Di a Claude: "Cambia el color principal a [COLOR]"
2. Claude actualizará el CSS
3. Copia y pega en GitHub

## 📊 VERSIÓN ACTUAL

**Versión:** 1.0  
**Fecha:** Febrero 2026
**Contenido:** 
- Introducción
- 10 Capítulos completos (demostración)
- Cuestionario (pendiente añadir)
- Ejercicios (pendiente añadir)
- Recursos (pendiente añadir)

**NOTA PARA TI, GREG:**
La versión actual es una DEMOSTRACIÓN con la estructura completa.
Para añadir TODO el contenido de las 4 partes (67 páginas):

1. Dime cuándo estés listo
2. Te daré el HTML completo con TODOS los capítulos
3. Lo copias y pegas en GitHub
4. ¡Listo!

## 🆘 SOLUCIÓN DE PROBLEMAS

### "No puedo ver la página"
- Espera 2-3 minutos después de activar GitHub Pages
- Verifica que el repositorio sea público
- Revisa Settings → Pages para ver el estado

### "Los cambios no aparecen"
- GitHub Pages puede tardar 1-2 minutos en actualizar
- Haz "hard refresh": Ctrl+Shift+R (PC) o Cmd+Shift+R (Mac)
- Borra caché del navegador

### "Se perdió mi progreso"
- Usa el archivo JSON que descargaste con "Guardar Mi Progreso"
- Botón "Restaurar Progreso" → Selecciona el archivo
- Si no hicieron backup, no se puede recuperar

### "No funciona offline"
- Asegúrate de haber visitado la página al menos una vez con internet
- El Service Worker necesita la primera carga con conexión
- Después funciona totalmente offline

## 📞 SOPORTE

Si tienes problemas:
1. Vuelve a este chat de Claude
2. Describe el problema
3. Claude te ayudará a solucionarlo

## 🎯 SIGUIENTE PASO

**AHORA:** 
1. Crea el repositorio en GitHub
2. Sube index.html y sw.js
3. Activa GitHub Pages
4. Comparte la URL con la pareja

**CUANDO ESTÉS LISTO:**
Dime y te daré el HTML completo con las 67 páginas de contenido.

---

¿Preguntas? ¡Pregúntale a Claude! 🤖
