# AClient Entities Repository

Repositorio de almacenamiento y distribucion de custom entities para **AClient**.

## Como funciona la descarga automatica

Cuando un usuario de AClient entra a una partida y otro jugador está usando un pack de entities registrado en Supabase, el cliente descarga la textura directamente desde:
`	ext
https://raw.githubusercontent.com/AgusClient/entities/main/<nombre_entidad>.png
`

El archivo se almacena en:
downloaded_entities/<nombre_entidad>.png
quedando disponible inmediatamente en memoria para renderizar en tiempo real el bloque hookeado por ese jugador.

---

## Como agregar nuevas entities

1. Asegurarse de que el archivo cumpla con las proporciones estandar de Teeworlds/DDNet (cuadricula 16x16 de 1024x1024 o proporcional en formato RGBA).
2. Nombrar el archivo <nombre_entidad>.png (por ejemplo lat.png o ddnet.png).
3. Colocar el archivo .png en la raiz de este repositorio.
4. Hacer commit y push a la rama main.