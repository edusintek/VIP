# EDUSINTEK/VIP · Landing del Intensivo

Página estática (un solo `index.html` + carpeta `assets/`). No necesita base de datos ni dominio propio.

## Opción A · GitHub Pages (gratis, recomendada)

La dirección queda así: **`https://edusintek.github.io/VIP/`**

1. Crea una cuenta (u organización) de GitHub llamada **`edusintek`**. Si ese nombre está ocupado, usa uno parecido (`edusintekvip`, `edusintek-trading`).
2. Crea un repositorio público llamado **`VIP`**.
3. Sube todo el contenido de esta carpeta (`index.html`, `assets/`, etc.) a la raíz del repositorio.
4. En el repositorio ve a **Settings → Pages**, en *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
5. En 1–2 minutos la página estará en `https://edusintek.github.io/VIP/`.

## Opción B · Railway

La dirección queda así: **`https://edusintek-vip.up.railway.app`**

1. Sube esta carpeta a un repositorio de GitHub (puede ser el mismo de la opción A).
2. En Railway: **New Project → Deploy from GitHub repo** y elige el repositorio.
3. Railway detecta `package.json` y ejecuta `npm start` (sirve la página con `serve`).
4. En **Settings → Networking → Generate Domain** escribe `edusintek-vip` como subdominio.

## Probar en tu computador

```bash
npm install
npm start
```

Y abre `http://localhost:3000`.

## Datos que se editan rápido

Al final de `index.html`, en el bloque `<script>`:

- `WHATSAPP`: número de Yeri (sin `+` ni espacios).
- `WA_MSG`: mensaje que aparece escrito al abrir WhatsApp.
- `START`: fecha y hora de la primera clase (la cuenta regresiva y la "hora local" salen de aquí).

El precio ($40 USD) y los horarios por país están escritos directamente en el HTML.
