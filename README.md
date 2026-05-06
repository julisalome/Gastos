# 💸 CAJA — Control de Gastos

Mini webapp para registrar y visualizar gastos **grandes** (expensas, tarjetas, internet, etc.) y **hormiga** (comida, kiosco, delivery, etc.).

## ¿Qué incluye?

- 📊 Dashboard con totales, barra proporcional y desglose por categoría
- 📋 Lista filtrable por tipo y mes
- ➕ Formulario rápido con categorías prearmadas
- 💾 Datos guardados en localStorage (persisten en el navegador)
- 📱 Diseño mobile-first

---

## Cómo subir a GitHub Pages

### Opción A — desde el navegador (más fácil)

1. Entrá a [github.com](https://github.com) y creá un repositorio nuevo
   - Nombre sugerido: `caja-gastos`
   - Dejalo en **Public**
   - **No** marques "Add a README"

2. Una vez creado, hacé clic en **"uploading an existing file"**

3. Arrastrá el archivo `index.html` y hacé commit

4. Andá a **Settings → Pages**

5. En *Source*, elegí **Deploy from a branch**

6. Branch: `main` / Folder: `/ (root)` → guardá

7. En 1-2 minutos tu app va a estar disponible en:
   ```
   https://TU-USUARIO.github.io/caja-gastos/
   ```

---

### Opción B — desde la terminal (con Git)

```bash
# 1. Inicializá el repo local
git init
git add index.html
git commit -m "Initial commit"

# 2. Conectá con GitHub (reemplazá con tu usuario y repo)
git remote add origin https://github.com/TU-USUARIO/caja-gastos.git
git branch -M main
git push -u origin main
```

Luego activá GitHub Pages desde Settings → Pages como en el paso 4 de la Opción A.

---

## Estructura de archivos

```
caja-gastos/
└── index.html   ← todo en un solo archivo, sin dependencias
```

No necesitás instalar nada ni correr ningún build. Es HTML/CSS/JS puro.

---

## Personalización rápida

Las categorías están al inicio del `<script>` en `index.html`:

```js
const CATS_GRANDE = ["Expensas","Tarjeta","Internet","Alquiler","Seguro","Cuota","Servicio","Otro"];
const CATS_HORMIGA = ["Comida","Kiosco","Transporte","Café","Delivery","Farmacia","Varios"];
```

Editá esas líneas para agregar o cambiar categorías.
