# Prueba Técnica: Frontend (Next.js)

**Tiempo sugerido:** 1 hora

Bienvenido a la prueba técnica de Frontend. Este proyecto ya cuenta con Next.js (App Router) y Tailwind CSS preconfigurados. A continuación encontrarás 3 problemas diseñados para evaluar tu dominio del framework y buenas prácticas.

## ⚠️ Instrucciones de Control de Versiones (Git)
Es obligatorio que manejes tu progreso usando buenas prácticas de Git. **Cada problema se considera un fix o feature independiente**. Por lo tanto, para CADA problema debes:
1. Crear una rama nueva desde la rama principal (ej: `feature/problema-1`).
2. Resolver el problema y hacer tus commits correspondientes.
3. Hacer push de tu rama y crear un **Pull Request (PR)** hacia la rama principal.
4. Volver a la rama principal para iniciar el siguiente problema.

---

## Problema 1: Data Fetching y Server Components (15 min - Básico)
**Objetivo:** Evaluar el uso del App Router y componentes de servidor.
- Crea una ruta nueva en `/users`.
- Dentro del `page.tsx` de esta ruta (como Server Component), haz un fetch a una API pública (puedes usar `https://jsonplaceholder.typicode.com/users`).
- Renderiza una lista simple con los nombres y correos de los usuarios.
- Implementa un archivo `loading.tsx` para mostrar un estado de carga mientras se obtienen los datos.

## Problema 2: Routing Dinámico y Estado Local (15 min - Intermedio)
**Objetivo:** Evaluar Client Components y rutas dinámicas.
- Crea una ruta dinámica en `/users/[id]`.
- Al entrar a un usuario específico, muestra el ID en pantalla.
- Implementa un pequeño contador interactivo (Botones de `+` y `-`) en esta misma página.
- **Importante:** Justifica correctamente la adición de `"use client"` en el lugar adecuado sin romper las reglas de composición (manteniendo el layout/page lo más "Server" posible si es viable).

## Problema 3: Server Actions y Optimistic Updates (30 min - Avanzado)
**Objetivo:** Evaluar las características más recientes de Next.js.
- Crea un formulario sencillo para agregar un "Nuevo Usuario" a una lista local (puedes hacer la lista mockeada).
- Utiliza **Server Actions** (`"use server"`) para manejar el `submit` del formulario (simulando un delay de 2 segundos en el servidor).
- Implementa **Optimistic Updates** (usando `useOptimistic` de React). Al enviar el formulario, el nuevo usuario debe aparecer en la lista instantáneamente en la interfaz de usuario, y si la Server Action falla, debe revertirse el estado.

---
¡Mucho éxito! No te preocupes si no logras completar todos los puntos, enfócate en demostrar tus buenas prácticas y tu proceso de razonamiento.
