# Reto #2 - Tarjeta de Producto Responsiva

Componente de "tarjeta de producto" para la tienda online **GadgetGrove**.
En móviles la imagen y el texto se muestran uno encima del otro; en pantallas más grandes, uno al lado del otro.

## Estructura

```
/reto-tarjeta-responsiva/
|-- /css/
|   |-- styles.css
|-- /images/
|   |-- drone.jpg
|-- index.html
```

- `index.html`: estructura de la tarjeta (Anexo 1) enlazada a la hoja de estilos externa.
- `css/styles.css`: estilos base (móvil) y media query para escritorio.
- `images/drone.jpg`: imagen del producto (Anexo 3).

## Estilos aplicados (Anexo 2)

| Propiedad | Valor |
| --- | --- |
| Punto de quiebre | `768px` |
| Borde de la tarjeta | `1px solid #dee2e6` |
| Relleno interno | `20px` |
| Espaciado (`gap`) entre imagen y texto | `20px` |

Los valores de borde, relleno y espaciado están definidos como variables CSS en `:root`, así se cambian en un solo lugar.

## Comportamiento

| Ancho de pantalla | Diseño |
| --- | --- |
| Menor a 768px | Vertical: imagen arriba y texto debajo (`flex-direction: column`) |
| 768px o más | Horizontal: imagen a la izquierda y texto a la derecha (`flex-direction: row`) |

## Cómo probarlo

1. Abrir `index.html` en el navegador.
2. Reducir el ancho de la ventana por debajo de 768px: la imagen pasa arriba y el texto debajo.
3. Ampliar la ventana hasta 768px o más: la imagen queda a la izquierda y el texto a la derecha.
4. El cambio ocurre al instante al cruzar el punto de quiebre.

## Autor

ujuanpolanco
