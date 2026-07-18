# Steven

App nativa Android generada a partir de [https://www.webtonative.com/?utm_source=google_ad&utm_medium=cpc&utm_campaign=growth_pmax&gad_source=1&gad_campaignid=22857354190&gbraid=0AAAAABfIQjWFw1_tGQJHd5J1Vsu9Wiou6&gclid=CjwKCAjwyOzSBhBTEiwAmxvJ-ihx7qS4Rsj53oZljLrSSEzVXmkscAi53ZslBVprbbOaCcUk1Wq8mhoCv-cQAvD_BwE](https://www.webtonative.com/?utm_source=google_ad&utm_medium=cpc&utm_campaign=growth_pmax&gad_source=1&gad_campaignid=22857354190&gbraid=0AAAAABfIQjWFw1_tGQJHd5J1Vsu9Wiou6&gclid=CjwKCAjwyOzSBhBTEiwAmxvJ-ihx7qS4Rsj53oZljLrSSEzVXmkscAi53ZslBVprbbOaCcUk1Wq8mhoCv-cQAvD_BwE) usando [Capacitor](https://capacitorjs.com).

## Cómo obtener el APK

1. Ve a la pestaña **Actions** de este repositorio.
2. Abre la ejecución más reciente de "Build Android APK" (se dispara sola con cada push).
3. Cuando termine, descarga el artefacto **app-debug-apk** y desempaqueta el `.apk`.

Este APK está firmado en modo debug: sirve para instalar y probar en un dispositivo o emulador, pero **no** para publicar en Play Store. Para eso necesitas generar tu propio keystore de firma y actualizar el workflow con un paso `assembleRelease`.

## Actualizar la app

- Cambiar el sitio que carga: edita `server.url` en `capacitor.config.json`.
- Cambiar el color de splash / barra de estado: edita `backgroundColor`.
- Cambiar el ícono: reemplaza `resources/icon.png` (cuadrado, 1024×1024 px o más) y vuelve a hacer push. El workflow regenera todos los tamaños automáticamente.
- Cualquier cambio en tu sitio web en vivo se refleja solo, ya que la app carga la URL en tiempo real — no hace falta recompilar salvo que cambies configuración nativa.

Generado con un panel libre y de código abierto, sin cuotas ni marca de agua.
