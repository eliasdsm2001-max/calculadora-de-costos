# 🎬 Higgsfield · Content Cost Calculator

Herramienta gratuita para **creadores de contenido con IA** que usan [Higgsfield.ai](https://higgsfield.ai).  
Calcula el costo real de cada video, cuántos créditos gastaste y cuánto cobrarle a tu cliente.

 ![Preview](https://img.shields.io/badge/HTML-Solo%20archivo-purple?style=flat-square)
 ![License](https://img.shields.io/badge/Licencia-MIT-green?style=flat-square)
 ![Higgsfield](https://img.shields.io/badge/Higgsfield.ai-Compatible-blueviolet?style=flat-square)

---

## ✨ ¿Qué hace?

- 📋 **Registra tu proyecto** con nombre y los modelos IA que usaste
- 🤖 **Calcula créditos** consumidos por modelo (Kling 3.0, Veo 3, Sora 2, Seedance 2.0, etc.)
- 💵 **Convierte a COP o USD** automáticamente (tasa ~4,100 COP/USD)
- 💪 **Incluye tu mano de obra** — tus horas × tu tarifa por hora
- 💰 **Sugiere el precio al cliente** con tu margen de ganancia configurado
- 📁 **Guarda historial** de proyectos con totales acumulados de facturación y ganancia

---

## 🚀 Uso rápido

No necesitas instalar nada. Es un solo archivo HTML.

```bash
# Opción 1 — Abrir directo en el navegador
Doble clic en index.html

# Opción 2 — Servidor local (opcional)
npx serve .
# o
python3 -m http.server 8080
```

Luego abre `http://localhost:8080` en tu navegador.

---

## 📊 Modelos incluidos (precios verificados mayo 2026)

| Modelo | Créditos por clip | Duración | Notas |
|---|---|---|---|
| Kling 3.0 | ~6 cr | 5s | 720p |
| Kling 3.0 (4K) | ~18 cr | 5s | 3× más que 720p |
| Seedance 2.0 | ~25 cr | 5s | Audio nativo incluido |
| Veo 3 Fast | ~22 cr | 8s | 720p con audio |
| Veo 3 Full | ~58 cr | 8s | Solo Plus/Ultra |
| Sora 2 | ~55 cr | 5s | 40–70 cr según duración |
| Hailuo 02 | ~10 cr | 5s | |
| WAN 2.6 | ~5 cr | 5s | Unlimited en ciertos planes |
| Soul V2 | GRATIS | 5s | 5000 gens/mes en Plus |
| Nano Banana Pro | ~2 cr | imagen | 4K, texto preciso |
| Flux.2 Pro | ~3 cr | imagen | Unlimited en Plus/Ultra |
| Ideogram | ~4 cr | imagen | |

### Planes Higgsfield (anuales)

| Plan | Precio/mes | Créditos | Costo/crédito |
|---|---|---|---|
| Starter | $15 USD | 200 | $0.075/cr |
| Plus | $39 USD | 1,000 | $0.039/cr |
| Ultra | $99 USD | 3,000 | $0.033/cr |

---

## 🌐 Demo en GitHub Pages

Si activas GitHub Pages en este repo, la calculadora queda disponible en:

```
https://TU_USUARIO.github.io/higgsfield-calculator/
```

---

## 📁 Estructura del proyecto

```
higgsfield-calculator/
├── index.html          ← La calculadora completa (un solo archivo)
├── README.md           ← Este archivo
├── LICENSE             ← Licencia MIT
└── .gitignore          ← Archivos ignorados por Git
```

---

## 🛠 Personalización

Puedes editar directamente el archivo `index.html`:

- **Tasa COP/USD** → busca `const USD_TO_COP = 4100` y cambia el valor
- **Agregar modelos** → añade un objeto al array `MODELS` con `{id, name, cat, cr, dur, unit, color, note}`
- **Cambiar precios de planes** → edita el objeto `PLANS`

---

## 🤝 Contribuir

1. Haz fork del repositorio
2. Crea una rama: `git checkout -b feature/nuevo-modelo`
3. Haz tus cambios en `index.html`
4. Commit: `git commit -m "feat: agregar modelo X"`
5. Push: `git push origin feature/nuevo-modelo`
6. Abre un Pull Request

---

## 📄 Licencia

MIT — Libre para usar, modificar y distribuir.  
Hecho con ❤️ para creadores de contenido con IA en Colombia y Latinoamérica.
