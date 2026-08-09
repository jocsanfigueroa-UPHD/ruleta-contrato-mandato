# 🎡 Ruleta Jurídica - Contrato de Mandato

Juego interactivo basado en el informe académico sobre el Contrato de Mandato.

## Características

- Ruleta de categorías.
- 10 preguntas.
- 2 a 4 jugadores.
- 30 segundos por pregunta.
- 10 puntos por respuesta correcta.
- Marcador individual.
- Pantalla final con ganador.
- Diseño responsive.
- No requiere servidor, PHP ni base de datos.

## Ejecutar en Visual Studio Code

1. Abre la carpeta del proyecto en Visual Studio Code.
2. Abre `index.html`.
3. Puedes abrirlo directamente en el navegador.
4. Recomendado: instalar la extensión **Live Server** y seleccionar:
   `Open with Live Server`.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube `index.html`.
3. En el repositorio entra a:
   **Settings → Pages**
4. En **Build and deployment**, selecciona:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
5. Guarda.
6. GitHub generará el enlace público de tu juego.

## Modificar preguntas

Dentro de `index.html` busca:

```javascript
const questions = [
```

Cada pregunta tiene esta estructura:

```javascript
{
  cat: "Concepto",
  q: "¿Pregunta?",
  o: ["Respuesta A", "Respuesta B", "Respuesta C", "Respuesta D"],
  c: 1
}
```

`c` indica la respuesta correcta:

- `0` = A
- `1` = B
- `2` = C
- `3` = D
