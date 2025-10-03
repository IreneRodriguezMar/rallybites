# RallyBites · Geo-Rally de Cafés, Comida y Bares

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](#licencia)
![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![Hacktoberfest](https://img.shields.io/badge/Hacktoberfest-Participating-%23ff8c00)
![Built with React](https://img.shields.io/badge/Built%20with-React-61dafb)

**RallyBites** es una app web (y futura app móvil) para **descubrir lugares** cercanos (cafés, restaurantes, bares, postres, veggie), **filtrarlos por categoría/distancia**, y **armar tu propio “rally”** seleccionando tus favoritos en el mapa.

> 🎯 **MVP**: mapa con filtros, lista ordenada por cercanía (Haversine), popups con info, selección de lugares y polyline de la ruta; alta de nuevos lugares con guardado local.

---

## Demo

> _Agrega aquí el link del deploy (Vercel/Netlify) y/o GIFs de la app._  
> Ej.: `https://rallybites.vercel.app`

---

## Características (MVP)

- 🗺️ **Mapa** (OpenStreetMap/Leaflet) con tu ubicación aproximada.  
- 🔎 **Filtros** por categoría y radio (km).  
- 📍 **Listado** ordenado por distancia real (Haversine).  
- ➕ **Agregar lugar** (formulario; guarda en LocalStorage).  
- 🧭 **Armar rally**: selecciona N lugares y genera la ruta (polyline).

**Próximos pasos (MLP):** clustering, compartir ruta por enlace, ratings, Supabase para persistencia real, dark mode, eventos/retos.

---

## Stack

- **Frontend web:** React + Vite + TypeScript  
- **Mapa:** Leaflet + react-leaflet  
- **Estado:** Zustand  
- **Estilos:** CSS simple (Tailwind opcional luego)  
- **Datos MVP:** LocalStorage + `SAMPLE_PLACES` (semilla)  
- **Backend futuro:** Supabase (Postgres + Realtime + Storage)  
- **Móvil (fase 2):** Expo / React Native con `react-native-maps`

---

## Requisitos

- **Node.js 18+**  
- Navegador moderno  
- _MVP sin claves de API_ (tiles de OpenStreetMap).  
  > Si migras a otro proveedor, configura `VITE_TILES_URL` (ver Issue “Config: tiles por .env”).

---

## Empezar (Dev)

```bash
# 1) Clonar
git clone https://github.com/<tu-usuario>/<tu-repo>.git
cd <tu-repo>

# 2) Instalar dependencias
npm i

# 3) Correr en desarrollo
npm run dev

# 4) Build de producción
npm run build
npm run preview
