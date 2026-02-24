# 🧩 Flex, Flex-Grow y Flex-Shrink

## 📌 ¿Qué es flex?

Flex es una propiedad abreviada que combina tres propiedades:

- **flex-grow**

- **flex-shrink**

- **flex-basis**

Su sintaxis completa sería:

*flex: grow shrink basis;*

#### 🔎 ¿Qué significa flex: 1?;

En realidad equivale a:
```css

flex: 1 1 0%;
```
O
```css

  flex-grow: 1;    
  flex-shrink: 1;  
  flex-basis: 0%;
```


Esto significa:

Puede crecer si hay espacio disponible.

Puede reducirse si falta espacio.

Parte de una base flexible.

En el proyecto, esto hace que ambas tarjetas ocupen el mismo espacio dentro del contenedor.

#### 🔎 ¿Qué significa flex: auto?

Equivale a:
```css

flex: 1 1 auto;
```
O
```css

  flex-grow: 1;    
  flex-shrink: 1;  
  flex-basis: auto;
```

Esto significa:

El elemento puede crecer.
Puede reducirse.

Su tamaño base depende de su contenido.

En el proyecto, la tarjeta .featured usa auto para ocupar todo el espacio extra disponible.

#### 🔎 ¿Qué significa flex: initial?

Equivale a:
```css

    flex: 0 1 auto;

```
o
```css

  flex-grow: 0;    
  flex-shrink: 1;  
  flex-basis: 100%;
```

Esto significa:

No crece.

Puede reducirse.

Su tamaño depende solo de su contenido.

En el proyecto, la tarjeta .associated solo ocupa el espacio que necesita.



Esto permite crear un layout flexible sin usar medidas fijas ni cálculos manuales.
