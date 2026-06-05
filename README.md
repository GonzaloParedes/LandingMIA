# Korda Agent for DAWs

Landing page estatica para presentar un posible proyecto de tesis/trabajo final: un asistente creativo basado en IA para flujos de produccion musical en DAWs.

## Estructura

```text
.
├── index.html
├── styles.css
├── script.js
└── README.md
```

## Como correrlo localmente

No requiere instalacion ni dependencias.

Opcion simple:

1. Abrir `index.html` directamente en el navegador.

Opcion con servidor local:

```bash
python -m http.server 8080
```

Luego visitar:

```text
http://localhost:8080
```

## Personalizacion

Reemplazar los placeholders en `index.html`:

- `[Mi nombre]`
- `[Carrera / Universidad]`
- `[Breve descripción personal]`
- `[Email]`
- `[LinkedIn]`
- `[GitHub]`

## Deploy

### Vercel

1. Subir estos archivos a un repositorio de GitHub.
2. Entrar a Vercel y crear un nuevo proyecto.
3. Importar el repositorio.
4. Como es un sitio estatico, no hace falta configurar build command.
5. Publicar.

### Netlify

1. Subir estos archivos a un repositorio de GitHub.
2. Entrar a Netlify y elegir "Add new site".
3. Importar el repositorio.
4. Dejar el build command vacio.
5. Usar `/` como publish directory.
6. Publicar.

### GitHub Pages

1. Subir el proyecto a GitHub.
2. Ir a `Settings > Pages`.
3. En `Build and deployment`, elegir `Deploy from a branch`.
4. Seleccionar la rama principal y la carpeta `/root`.
5. Guardar.

## Dominio propio

Pasos generales:

1. En la plataforma de deploy, agregar el dominio personalizado.
2. Copiar los registros DNS que indique la plataforma.
3. En el proveedor del dominio, crear o actualizar los registros DNS.
4. Esperar la propagacion DNS.
5. Activar HTTPS desde la plataforma de deploy si no se activa automaticamente.

Para Vercel y Netlify normalmente se usa un registro `CNAME` para `www` y registros `A` o `ALIAS/ANAME` para el dominio raiz, segun indique cada plataforma.
