# 🚚 Sistema de Tracking GPS - VERSIÓN SIMPLE

Sistema minimalista de rastreo GPS para mensajeros.

## 📁 Archivos

- **mobile-simple.html** - App para mensajeros (abrir en teléfonos)
- **admin-simple.html** - Panel de administración (abrir en PC)
- **README-SIMPLE.md** - Este archivo

---

## 🚀 PRUEBA RÁPIDA (mismo dispositivo)

### Opción más fácil para probar:

1. Abre `admin-simple.html` en una pestaña de Chrome
2. Abre `mobile-simple.html` en otra pestaña de Chrome
3. En la app móvil, ingresa tu nombre
4. Dale "INICIAR" → Acepta permisos de ubicación
5. Dale "INICIAR TRACKING"
6. Ve a la pestaña del admin → ¡Deberías verte en el mapa! 🎉

---

## 📱 USO EN 2 DISPOSITIVOS (Demo real)

### PASO 1: Preparar tu PC

1. Descarga los archivos a una carpeta
2. Abre la terminal/CMD en esa carpeta
3. Ejecuta un servidor HTTP:

**Python 3:**
```bash
python -m http.server 8000
```

**Python 2:**
```bash
python -m SimpleHTTPServer 8000
```

**Node.js:**
```bash
npx http-server -p 8000
```

4. Encuentra tu IP:
   - **Windows:** Abre CMD → escribe `ipconfig` → busca "IPv4"
   - **Mac/Linux:** Abre Terminal → escribe `ifconfig` → busca "inet"
   - Ejemplo: `192.168.1.100`

### PASO 2: En tu PC

- Abre Chrome
- Ve a: `http://localhost:8000/admin-simple.html`
- Deja esta ventana abierta

### PASO 3: En el teléfono

1. Conecta el teléfono a la **misma red WiFi** que tu PC
2. Activa el **GPS** del teléfono
3. Abre **Chrome** o **Safari**
4. Escribe en la URL: `http://TU_IP:8000/mobile-simple.html`
   - Ejemplo: `http://192.168.1.100:8000/mobile-simple.html`
5. Ingresa el nombre del mensajero
6. Dale "INICIAR" → **ACEPTA permisos** cuando aparezcan
7. Dale "INICIAR TRACKING"

### PASO 4: Ver el resultado

- Ve a tu PC
- En el panel deberías ver el mensajero en el mapa
- Se actualiza automáticamente cada 3 segundos

---

## ❌ SI NO FUNCIONA

### Error: "Permisos denegados"

**Android - Chrome:**
1. Toca el candado 🔒 junto a la URL
2. Toca "Permisos"
3. Activa "Ubicación"
4. Recarga la página

**iPhone - Safari:**
1. Ve a Ajustes → Safari → Ubicación
2. Selecciona "Preguntar" o "Permitir"
3. Cierra Safari completamente
4. Abre de nuevo

### Error: "No se puede conectar"

- ✅ Verifica que estés en la **misma red WiFi**
- ✅ Verifica que la **IP sea correcta**
- ✅ Verifica que el **servidor esté corriendo** (python/node)
- ✅ Intenta desactivar el **firewall** temporalmente

### Error: "GPS no disponible"

- ✅ Activa el **GPS** en configuración del teléfono
- ✅ Sal al **exterior** (mejor señal)
- ✅ Espera **1-2 minutos** (GPS necesita tiempo)
- ✅ Prueba con **Google Maps** primero para verificar que el GPS funcione

---

## 💡 TIPS PARA LA DEMO

✅ **Prepara con anticipación:**
- Prueba todo 1 hora antes
- Ten los teléfonos cargados
- Anota la IP de tu PC

✅ **Ubicación ideal:**
- Cerca de ventana
- En exterior si es posible
- Con buena señal WiFi

✅ **Durante la demo:**
- Ten 2 teléfonos con nombres diferentes
- Camina con ellos para mostrar el tracking
- Muestra el panel en proyector/pantalla grande

✅ **Plan B:**
- Graba un video de la demo funcionando
- Si falla en vivo, muestra el video

---

## 🔍 DIFERENCIAS CON LA VERSIÓN ANTERIOR

Esta versión es más simple:

✅ **Menos código** = menos errores
✅ **Permisos más básicos** = más compatible
✅ **UI minimalista** = funciona en más navegadores
✅ **Sin funciones complejas** = más estable

❌ No tiene:
- Diseño muy elaborado
- Validaciones complejas
- Múltiples animaciones

Pero **funciona mejor** para una demo.

---

## 📊 ¿Qué sigue después?

Si aprueban el proyecto, para implementarlo en producción necesitarían:

1. **Backend real** (Node.js + PostgreSQL o Firebase)
2. **Hosting en la nube** (AWS, Google Cloud, Heroku)
3. **Autenticación** (login con usuario/contraseña)
4. **App nativa** (opcional - mejor experiencia)
5. **Historial** de rutas guardado
6. **Reportes** y estadísticas

**Costo aproximado:** $50-200 USD/mes según uso

---

## ✅ CHECKLIST ANTES DE LA DEMO

- [ ] Archivos descargados
- [ ] Servidor HTTP corriendo en PC
- [ ] IP de la PC anotada
- [ ] Teléfonos conectados a WiFi
- [ ] GPS activado en teléfonos
- [ ] Chrome/Safari instalado
- [ ] Prueba funcionando
- [ ] Batería suficiente

---

**¡Buena suerte con tu presentación! 🎉**

Si funciona bien, será una demo muy impresionante para Importadoras Asociadas.
