# Ejercicios

- [1. Ejercicio 1](#1-ejercicio-1)
  - [1.1. Objetivo](#11-objetivo)
  - [1.2. Solución](#12-solución)
- [2. Ejercicio 2](#2-ejercicio-2)
  - [2.1. Objetivo](#21-objetivo)
  - [2.2. Solución](#22-solución)

## 1. Ejercicio 1

### 1.1. Objetivo

Una empresa utiliza ficheros XML para realizar el inventario, entre otras cosas, de impresoras. Para cada impresora se quiere guardar su número de serie, marca, modelo, peso, tamaños de papel con los que puede trabajar, el cartucho que usa, el tipo, el año de compra y si está en red o no.

Un ejemplo de estos ficheros sería:

```xml
<impresoras>
  <impresora numSerie="i245" tipo="láser" compra="2010">
    <marca>Epson</marca>
      <modelo>EPL300</modelo>
      <peso>4.52</peso>
      <tamaño>A4</tamaño>
      <tamaño>A5</tamaño>
      <cartucho>C-123BV</cartucho>
      <enred/>
  </impresora>
  <impresora numSerie="i246" tipo="matricial">
    <marca>HP</marca>
    <modelo>LaserJet 2410</modelo>
    <peso>3.2</peso>
    <tamaño>A4</tamaño>
    <cartucho>C-456P</cartucho>
  </impresora>
</impresoras>
```

**Escribe un XML Schema** para estos ficheros, eligiendo los tipos de datos más apropiados y teniendo en cuenta que:

- El peso es un número positivo y no puede tener más de dos decimales.
- Puede haber más de un tamaño.
- El atributo tipo sólo puede tomar los valores `matricial`, `láser` y `tinta`. Es obligatorio.
- El atributo `numSerie` es obligatorio y hace de identificador.
- El cartucho está formado por una `C` mayúscula, un guión, tres números y una o dos letras mayúsculas.
- Todos los elementos son obligatorios, menos `<enred>`.
- El elemento `<enred>` es opcional. De estar presente, es un elemento vacío.
- El atributo `<compra>`, opcional, guarda el año de compra. Es un número entero positivo.
- En cada fichero hay datos para una o más impresoras.

### 1.2. Solución

Tu solucion debe estar en el fichero [doc/ej01/inventario.xml](ej01/inventario.xml).

## 2. Ejercicio 2

### 2.1. Objetivo

Un asociación de jugadores de mus utiliza ficheros XML para almacenar la información de los torneos que organiza. Para cada torneo se quiere guardar el año en que se realizó, el anterior ganador (su id) y la información de los participantes. De los participantes se quiere almacenar su identificador, el de su pareja, su nombre completo, edad, país y también si es cabeza de serie o no.

Un ejemplo de estos ficheros sería:

```xml
<torneo edicion="1998" anteriorGanador="j01">
  <participante idP="j01" pareja="j02">
    <nombre>Manuel Pérez</nombre>
    <edad>23</edad>
    <pais> España</pais>
    <cabezaDeSerie/>
  </participante>
  <participante idP="j02" pareja="j01">
    <nombre>Manuel Gómez</nombre>  
    <edad>25</edad>
    <pais>España</pais>
  </participante>
  <participante idP="j03" pareja="j04">
    <nombre>Ana Puertas</nombre>
    <edad>22</edad>
    <pais> E5spaña</pais>
    <cabezaDeSerie/>
  </participante>
  <participante idP="j04" pareja="j03">
    <nombre>Paco Fraile</nombre>  
    <edad>45</edad>
    <pais>España</pais>
  </participante>
</torneo>
```

**Escribe un DTD adecuado** para estos ficheros, teniendo en cuenta que:

- Todos los atributos son obligatorios.
- El atributo `idP` hace de identificador.
- El atributo `pareja` es el identificador de otro participante que forzosamente debe estar presente en el fichero.
- El elemento `cabezaDeSerie` es opcional, los demás son obligatorios.
- En cada fichero hay datos para un solo torneo.
- El torneo tiene que tener participantes.

### 2.2. Solución

Tu solucion debe estar en el fichero [doc/ej02/torneo.xml](ej02/torneo.xml).
