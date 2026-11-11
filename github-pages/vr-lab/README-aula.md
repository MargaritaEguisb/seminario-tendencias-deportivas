# Laboratorio Web/VR para aula (pantallas inteligentes)

Este laboratorio está optimizado para **presentación en aula y pantallas inteligentes** (touch/interactivas), con modo 3D navegable y recorrido guiado.

## Archivos
- `index.html`: laboratorio interactivo (A-Frame/WebXR).

## Requisitos
- **Navegador moderno:** Google Chrome o Microsoft Edge (recomendado) actualizados.
- **Conexión a internet:** necesaria para cargar A-Frame desde CDN (`aframe.io`).
- **Pantalla inteligente:** funciona con mouse/teclado o táctil (botones grandes, panel informativo ampliado).
- **VR inmersivo (opcional):** visor compatible con WebXR y botón “Enter VR” del navegador/escena.

> No requiere instalar Unity/Unreal ni SDKs para su uso web en aula.

## Cómo ejecutarlo (recomendado en aula)
1. Abrir PowerShell en la carpeta `vr-lab`.
2. Iniciar servidor local:
   ```powershell
   python -m http.server 8080
   ```
3. Abrir en el navegador:
   - `http://localhost:8080`
4. Pulsar **Pantalla completa** (o tecla `F`).

### Alternativa rápida
- Abrir `index.html` con doble clic. (Puede funcionar, pero un servidor local es más estable para interacción/navegadores.)

## Controles para clase
- **Siguiente / Anterior:** botones en pantalla o teclas `→` / `←`.
- **Recorrido:** avanza automáticamente entre estaciones (cada 12 s).
- **Pantalla completa:** botón o tecla `F`.
- **Ocultar/mostrar paneles:** botón o tecla `H` (útil para proyectar solo la escena 3D).
- **Interacción 3D:** clic/toque en paneles de estaciones; arrastrar para girar; `WASD` para moverse (si hay teclado).
- **Vista general:** doble clic en el fondo.

## Contenido incluido
- ENAFIS 2025-2026 (actividad física y sedentarismo, Colombia)
- Auge de pádel y pickleball
- Bienestar urbano: running y ciclismo
- Deportes urbanos, extremos y alternativos (Slackline, Lacrosse, Parkour, Roller Freestyle, Long Board, etc.)
- eSports y transformación digital (Ley 2507 de 2025)
- Dimensiones del Técnico Deportivo (ciclo integral)
- Tecnología, OMS y reglamentación

## Notas para pantallas inteligentes
- Si el tacto es impreciso, usar los botones **Anterior/Siguiente** y la lista de estaciones.
- Si la red es inestable, considerar guardar una copia local de A-Frame o publicar en una red interna con el recurso disponible.
- Para máxima compatibilidad en visores WebXR, servir por **HTTPS** o en red local según el dispositivo.
