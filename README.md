# 🛠️ Piloto MES: Mesa Promods v3.5

**Sistema de Trazabilidad y Planos de Carpintería**

Aplicación web para escaneo QR de piezas de muebles, extracción de datos técnicos de producción y acceso a planos en tiempo real.

---

## 🚀 Características Principales

✅ **Escaneo QR en Vivo** - Cámara integrada para captura en tiempo real

✅ **Galería de Fotos** - Detecta QR en imágenes guardadas

✅ **Datos Técnicos** - Visualiza medidas, canteados e instrucciones

✅ **Responsive Mobile** - Optimizado para smartphones en línea de producción

✅ **Sin Backend Requerido** - Funciona localmente (ideal para intranets)

---

## 📱 Inicio Rápido

### Opción 1: Acceso Online (Recomendado)
```
https://salvadoryahirex-spec.github.io/Cidecsa-
```
*(Requiere activar GitHub Pages en Settings)*

### Opción 2: Localmente
1. Descargar el repositorio
2. Abrir `index.html` directamente en navegador (Chrome, Firefox, Safari)
3. ¡Listo! Permite acceso a cámara cuando lo pida

### Opción 3: Servidor Local (Desarrollo)
```bash
npm install
npm start
```

---

## 🔍 Códigos QR Válidos (Ejemplos)

| Código | Pieza | Medidas |
|--------|-------|----------|
| `PROMODS-01-CUB` | Cubierta Principal | 1200 x 600 x 25 mm |
| `PROMODS-01-PAT1` | Pata Izquierda A | 725 x 450 x 18 mm |
| `PROMODS-01-PAT2` | Pata Derecha B | 725 x 450 x 18 mm |
| `PROMODS-01-FAL` | Faldón Refuerzo | 1080 x 300 x 18 mm |

---

## 📋 Estructura de Datos

Cada pieza contiene:
- **Mueble Origen** - Identificador del proyecto
- **Pieza Identificada** - Nombre técnico de la parte
- **Medidas de Corte** - Dimensiones en mm
- **Instrucción de Canteado** - Especificación de bordes/terminados
- **Link a Plano** - URL al archivo CAD/imagen técnica

---

## 🔧 Tecnologías

- **HTML5 QR Code** - Librería de escaneo sin dependencias
- **Vanilla JavaScript** - Sin frameworks pesados
- **CSS3** - Diseño responsive moderno
- **Compatible**: iOS Safari, Android Chrome, Web Browsers

---

## 📝 Cómo Agregar Más Piezas

Editar `index.html` y agregar al objeto `excelMesaPromods`:

```javascript
"PROMODS-02-NUEVA": {
    mueble: "Mesa Promods (Lote 2)",
    pieza: "Nueva Pieza",
    medidas: "XXXX mm x YYYY mm x ZZ mm",
    canto: "Especificación de canteado",
    linkPlano: "URL-a-imagen-o-archivo"
}
```

---

## 🛡️ Seguridad

- ✅ Sin almacenamiento en servidor (datos en caché del navegador)
- ✅ Cámara solo activa con permiso del usuario
- ✅ Compatible con HTTPS obligatorio en producción
- ✅ Funciona offline después de primer acceso

---

## 📞 Soporte

**Problemas comunes:**

1. **"No funciona la cámara"**
   - Verificar permisos en Ajustes del dispositivo
   - Usar HTTPS (o localhost para desarrollo)

2. **"QR no se detecta"**
   - Mejorar iluminación
   - Mantener distancia 10-15 cm
   - Usar opción de galería si está borroso

3. **"Código no reconocido"**
   - Verificar que el QR esté en la base de datos
   - Contactar a administración para agregarlo

---

## 📄 Licencia

Desarrollo interno CIDECSA - 2026

---

**Versión:** 3.5 | **Última actualización:** Mayo 2026