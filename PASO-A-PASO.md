# 🏆 LEGACY Calculator - Guía de Despliegue

## Resumen del Proyecto

**LEGACY** es una calculadora de ganancias premium para la red de mercadeo Nu Skin Colombia. Permite a las empresarias calcular sus bonos y comisiones de forma visual y elegante.

### Características
- ✅ Búsqueda inteligente de productos (por nombre, SKU o categoría)
- ✅ Agregar múltiples productos
- ✅ Cálculo automático de 3 tipos de bonos:
  - **Ganancia Minorista**: Diferencia entre precio público y precio miembro
  - **Ganancia por Venta**: 4% a 20% según puntos acumulados
  - **Ganancia por Referir**: 4% a 24% según puntos acumulados
- ✅ Diseño luxury premium (oscuro con acentos dorados)
- ✅ Responsive (funciona en móvil y desktop)
- ✅ 60+ productos del catálogo Nu Skin Colombia

---

## 🚀 OPCIÓN 1: Despliegue Rápido con Vercel (Recomendado)

### Tiempo estimado: 5-10 minutos
### Costo: $0 (gratis)

### Paso 1: Crear cuenta en GitHub
1. Ve a [github.com](https://github.com)
2. Clic en "Sign up"
3. Sigue los pasos para crear tu cuenta

### Paso 2: Crear un repositorio nuevo
1. Una vez logueado, clic en el botón "+" (arriba a la derecha)
2. Selecciona "New repository"
3. Nombre: `legacy-calculator`
4. Dejarlo como "Public"
5. Clic en "Create repository"

### Paso 3: Subir los archivos
1. En tu repositorio vacío, clic en "uploading an existing file"
2. Arrastra los 3 archivos:
   - `index.html`
   - `package.json`
   - `vercel.json`
3. Clic en "Commit changes"

### Paso 4: Conectar con Vercel
1. Ve a [vercel.com](https://vercel.com)
2. Clic en "Sign up" → "Continue with GitHub"
3. Autoriza Vercel para acceder a tu GitHub
4. Clic en "Add New..." → "Project"
5. Busca y selecciona `legacy-calculator`
6. Clic en "Deploy"

### ¡Listo! 🎉
En 1-2 minutos tendrás tu calculadora en una URL como:
`https://legacy-calculator.vercel.app`

---

## 🖥️ OPCIÓN 2: Despliegue con GitHub Pages

### Tiempo estimado: 5 minutos
### Costo: $0 (gratis)

### Pasos:
1. Sigue los pasos 1-3 de la Opción 1
2. En tu repositorio, ve a "Settings"
3. En el menú lateral, busca "Pages"
4. En "Source", selecciona "Deploy from a branch"
5. Selecciona "main" y "/ (root)"
6. Clic en "Save"

Tu sitio estará disponible en:
`https://tu-usuario.github.io/legacy-calculator`

---

## 💻 OPCIÓN 3: Usar Claude Code o Cursor

### Tiempo estimado: 10-15 minutos

### Con Claude Code:
```bash
# 1. Clonar o crear el proyecto
mkdir legacy-calculator
cd legacy-calculator

# 2. Crear los archivos (copiar el contenido proporcionado)

# 3. Inicializar Git
git init
git add .
git commit -m "Initial commit"

# 4. Crear repo en GitHub y conectar
gh repo create legacy-calculator --public --source=. --push

# 5. Desplegar en Vercel
npx vercel
```

### Con Cursor:
1. Abre Cursor
2. Crea una nueva carpeta `legacy-calculator`
3. Copia los archivos proporcionados
4. Usa el terminal integrado para los comandos de Git y Vercel

---

## 🔧 Personalización Futura

### Cambiar el nombre "LEGACY"
En `index.html`, busca y reemplaza:
```html
<span className="gold-gradient">LEGACY</span>
```

### Cambiar colores
En la sección de configuración de Tailwind, modifica:
```javascript
'gold': '#c9a962',        // Color dorado principal
'gold-light': '#dfc07f',  // Dorado claro
'gold-dark': '#a68a4a',   // Dorado oscuro
```

### Agregar más productos
En el array `productsData`, agrega objetos con este formato:
```javascript
{
    sku: "XXXXXXXX",
    nombre: "Nombre del producto",
    categoria: "Categoría",
    precioPublicoSinImpuesto: 0,
    precioMiembroSinImpuesto: 0,
    bonoMinoristaSinImpuesto: 0,
    vv: 0
}
```

---

## 📱 Agregar Login (Fase 2)

Si en el futuro quieres agregar autenticación:

### Recursos necesarios:
- **Supabase** (gratis hasta 50,000 usuarios/mes)
- **Tiempo adicional**: 4-6 horas
- **Costo**: $0

### Beneficios del login:
- Control de quién accede
- Historial de cálculos por usuario
- Métricas de uso
- Posibilidad de roles (admin, empresaria)

Cuando estés listo para esta fase, podemos implementarlo juntos.

---

## 📞 Soporte

Si tienes dudas o necesitas ayuda:
1. Revisa que los archivos estén completos
2. Verifica que el repositorio sea público
3. Espera 2-3 minutos después del despliegue

---

**Desarrollado con ❤️ para las empresarias LEGACY**
