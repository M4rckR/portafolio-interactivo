# Portafolio Interactivo – PC3

**Curso:** Hojas de Estilo en Cascada Avanzado
**Alumno:** Italo

Landing page responsiva construida con **Bootstrap 5**, **Transformaciones CSS** y **Animaciones CSS**.

## Estructura

```
portafolio-interactivo/
├── index.html
├── css/
│   └── styles.css
└── README.md
```

## Bootstrap 5

- **Navbar** `bg-dark` con logo y menú (Inicio, Proyectos, Contacto) que colapsa en menú hamburguesa en móviles.
- **Grid** con `container`, `row`, `col-sm-12`, `col-md-6`, `col-md-4`.
- **Formulario** con `form-label`, `form-control` y `mb-3` (Nombre, Email, Mensaje).
- **Botones** "Enviar" (`btn btn-primary`) y "Limpiar" (`btn btn-secondary`) dentro de `d-grid gap-2`.

## Transformaciones 2D (hover + transition)

Sección **Proyectos**, tres cajas con `transition: transform 0.5s ease`:

| Caja | Transformación |
| --- | --- |
| Caja 1 | `rotate(8deg)` |
| Caja 2 | `scale(1.1)` |
| Caja 3 | `translateY(-15px) skew(-6deg)` |

## Transformación 3D

- Contenedor padre `.escena-3d` con `perspective: 1000px`.
- Tarjeta `.tarjeta-3d` con `transform-style: preserve-3d`.
- Al hacer hover gira con `transform: rotateX(15deg) rotateY(180deg)` mostrando su cara trasera.

## Animaciones (@keyframes)

- **`deslizarIzquierda`**: el título aparece deslizándose desde la izquierda (1 iteración, `ease-out`).
- **`colorTamano`**: el texto cambia de color y tamaño constantemente (`infinite`, `alternate`, `ease-in-out`).
- **`girar`** (Loader): spinner girando infinitamente al inicio de la página (`infinite`, `linear`).
- **`ocultarLoader`**: oculta el loader después de 2 segundos.

Propiedades usadas: `animation-duration`, `animation-iteration-count`, `animation-timing-function`, `animation-direction`, `animation-delay`, `animation-fill-mode`.

## Responsividad

Diseño adaptable a móvil, tablet y escritorio con el grid de Bootstrap, media query propia y `overflow-x: hidden` para evitar desbordamiento horizontal.
