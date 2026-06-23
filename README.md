# Gestión Patio Curauma

Sistema de gestión de tareas, sprint, equipo y coach para Carolina · Gestión Patio Curauma.

## Características

- **Tareas** con contexto (Casa / Bazar / Club), prioridad, frecuencia y vencimiento.
- **Sprint** semanal con responsables.
- **Equipo** y check-ins de compromisos activos.
- **Coach**: evaluación de estado de ánimo con recomendaciones e historial.
- **Autenticación** con correo y contraseña (Firebase Auth).
- **Base de datos** en la nube (Cloud Firestore), datos privados por usuario.

## Tecnología

- HTML + CSS + JavaScript (un solo archivo, sin build).
- Firebase: Authentication + Cloud Firestore (vía CDN).

## Ejecutar en local

```bash
npx live-server --port=5500
```

Luego abre http://localhost:5500/carolina-sistema-completo_3.html

## Reglas de seguridad de Firestore

Las reglas (`firestore.rules`) garantizan que cada usuario solo accede a su propio documento en la colección `users`.
