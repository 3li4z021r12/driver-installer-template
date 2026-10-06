# Guía rápida: instalación segura de WiGLE Wireless Wardriving (APK/App)

Esta guía implementa un flujo práctico para dejar WiGLE listo de forma segura y útil, con herramientas complementarias para captura, exportación y análisis.

## 1) Confirmar tu entorno

Antes de empezar, identifica:

- **Teléfono Android:** marca/modelo y versión de Android.
- **PC (opcional):** Windows, macOS o Linux.
- **Uso esperado:** solo recolección básica o también análisis de datos en PC.

> Recomendación: en Android 10+ desactivar el throttling de escaneo Wi‑Fi en opciones de desarrollador mejora resultados.

## 2) Instalar la app principal por vía confiable

Opciones recomendadas (en orden):

1. **Google Play:**  
   https://play.google.com/store/apps/details?id=net.wigle.wigleandroid
2. **F-Droid (build FOSS):**  
   https://f-droid.org/en/packages/net.wigle.wigleandroid/

Si instalas APK manual:

- Descárgalo solo de una fuente oficial/confiable.
- Verifica firma/hash cuando sea posible.
- Evita APKs de terceros sin reputación.

## 3) Configurar Android para escaneo estable

Dentro del sistema Android:

- Activar **Ubicación precisa**.
- Dar permisos de **Ubicación**, **Bluetooth** y almacenamiento/exportación según necesidad.
- Activar **Opciones de desarrollador**.
- Desactivar **Wi‑Fi scan throttling** (si está disponible en tu versión de Android).

Dentro de WiGLE:

- Verificar permisos concedidos.
- Ajustar escaneo y guardado según batería/rendimiento.

## 4) Crear cuenta y vincular servicio

- Crear cuenta o iniciar sesión en: https://wigle.net
- Iniciar sesión en la app para:
  - sincronización,
  - estadísticas,
  - carga/exportación asociada a tu cuenta.

## 5) Instalar herramientas complementarias (uso legítimo)

### 5.1 ADB (Android Platform Tools)

Sirve para diagnóstico básico del dispositivo y transferencia/depuración.

- Descarga oficial: https://developer.android.com/tools/releases/platform-tools
- Comando de prueba:
  - `adb devices`

### 5.2 Análisis de base de datos SQLite

- **DB Browser for SQLite:** https://sqlitebrowser.org/
- Útil para revisar exportaciones `.sqlite` de WiGLE.

### 5.3 Visualización geográfica (KML/GPX)

- **Google Earth:** https://www.google.com/earth/about/versions/
- **QGIS:** https://qgis.org/

### 5.4 Análisis tabular (CSV)

- LibreOffice Calc, Excel o Google Sheets para revisar y filtrar CSV exportados.

## 6) Flujo de trabajo recomendado en campo

- Define perfil de escaneo (agresivo vs ahorro de batería).
- Habilita registro de ruta si te interesa GPX.
- Establece rutina de respaldo (diario/semanal) de la base de datos exportada.
- Organiza exportaciones por fecha/zona (carpetas claras).

## 7) Validación rápida de funcionamiento

Haz una prueba corta (5–10 minutos):

1. Inicia escaneo.
2. Recorre una zona pequeña.
3. Detén y exporta.
4. Verifica que puedes abrir:
   - CSV
   - KML
   - SQLite
   - GPX

Si alguno falla, revisa permisos y espacio disponible.

## 8) Buenas prácticas legales y de seguridad

- Usa la app solo para descubrimiento/mapeo autorizado.
- **No** intentes acceso no autorizado a redes.
- Respeta legislación local y privacidad de terceros.
- No compartas datos sensibles sin consentimiento.

---

## Checklist rápido

- [ ] App instalada desde fuente confiable
- [ ] Permisos correctos en Android
- [ ] Cuenta WiGLE vinculada
- [ ] ADB instalado y detectando dispositivo
- [ ] Exportación CSV/KML/SQLite/GPX validada
- [ ] Respaldo periódico definido
