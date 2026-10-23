# PixelVault Games — Modelo 4+1 Vistas con PlantUML

Laboratorio de Arquitectura de Software. Se diseña la arquitectura de una tienda
e-commerce de videojuegos usando el **Modelo de 4+1 Vistas de Philippe Kruchten**,
especificado como código con **PlantUML**, y luego se genera un prototipo web
funcional con **IA generativa** a partir de esos diagramas.

## Contenido

| Archivo | Descripción |
|---|---|
| `arquitectura.puml` | Las 5 vistas del modelo 4+1 en PlantUML |
| `index.html` | SPA de PixelVault Games (Tailwind CSS + JavaScript puro) |

## Vistas del modelo 4+1

1. **Casos de uso (Escenarios):** actores y requerimientos RF1 a RF4.
2. **Lógica:** diagrama de clases (`Producto`, `Cliente`, `Arriendo`, `Venta`, `DetalleVenta`).
3. **Procesos:** diagrama de secuencia del arriendo y la devolución con multa.
4. **Desarrollo:** componentes (Frontend, API Gateway, microservicios, base de datos).
5. **Despliegue:** nodos de infraestructura (navegador, Node.js/Express, PostgreSQL).

Para visualizar los diagramas, pega cada bloque `@startuml … @enduml` en
[plantuml.com](https://www.plantuml.com/plantuml) o usa la extensión de PlantUML en VS Code.

## Prototipo web

Abre `index.html` en el navegador. No requiere instalación.

- **Catálogo:** búsqueda y filtros por plataforma (PS5, Xbox, Switch, PC) y formato (Físico/Digital).
- **Carrito:** control de stock, IVA del 19% y cupón de descuento (`PIXEL10`).
- **Arriendos:** tarifa de $2.000 por día y multa de $1.500 por día de atraso.
- **Modo Cliente VIP:** 10% de descuento en arriendos y acumulación de puntos.

## Cómo se generó

El código del prototipo se obtuvo inyectando en un prompt estructurado los diagramas
PlantUML de la Vista Lógica y la Vista de Desarrollo, de modo que las clases del
código JavaScript respetan los nombres y métodos definidos en el modelo.

## Autor

Nombre Apellido — Asignatura de Arquitectura de Software
