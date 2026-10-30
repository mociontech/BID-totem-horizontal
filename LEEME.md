# Reproductor del tótem horizontal

Abre `index.html` en Chrome o Edge. Pulsa F11 para pantalla completa. No requiere instalación ni conexión a internet. El diseño conserva una proporción horizontal de 1920 × 1080 (16:9) y se adapta al espacio disponible, con márgenes si la pantalla tiene otra proporción.

La portada usa directamente `Images/Pantalla_Principal.png` en formato 1920 ? 1080, sin recortes. El bot?n animado se superpone mediante `Images/TocaParaComenzar.png`; no lo incluyas en la imagen de portada para evitar duplicarlo.

La barra de tiempo se dibuja con CSS en una sola capa, con los colores originales azul (#005CFF) y azul claro (#CFE1FF), para evitar bordes claros por superposici?n de im?genes. Los archivos Barra_1.png y Barra_2.png ya no se utilizan.

Toca la portada para comenzar. Las indicaciones, los controles y la barra pulsan durante 7 segundos con el video detenido. Después empieza el video y se ocultan las ayudas. Un toque en el video muestra u oculta los controles. La barra y los controles se ocultan tras 2 segundos sin uso; cada interacción reinicia ese plazo. Mientras mantienes pulsado un botón o arrastras la barra, permanecen visibles. Los cinco botones de la franja inferior permiten reiniciar, retroceder 10 segundos, pausar/reproducir, avanzar 10 segundos y volver a la portada. También puedes arrastrar la barra para cambiar de posición. Al finalizar el video vuelve la portada.

Los controles conservan los iconos independientes y su versión azul al presionarlos. El botón central muestra Pause durante la reproducción y Start cuando el video está pausado, también durante las instrucciones.

Durante las instrucciones se muestra `Images/Video_Indicaciones.jpg` y la barra se mantiene al 50 %, con el video detenido en cero. Después de los 7 segundos se retira la imagen y la barra refleja el progreso real.

Para reemplazar el video, guarda el nuevo archivo como `Images/Video.mp4` y recarga la página. Usa MP4 compatible con el navegador (habitualmente H.264/AAC), preferentemente 1920 × 1080. Reemplaza también `Images/Video_Indicaciones.jpg` por un fotograma del nuevo archivo. Tanto el video como el fotograma se muestran completos con `object-fit: contain`, sin deformación ni recortes.

Si el navegador impide la reproducción automática con sonido tras las indicaciones, aparece un mensaje para iniciarla con un toque.
