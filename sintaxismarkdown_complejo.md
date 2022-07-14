---
title: "Lenguaje de Marcado Ligero - Markdown"
author: "Renzo Cáceres Rossi"
date: "2022/02/21"
subtitle: Markdown - RMarkdown
---

<!-- Añadir comentarios a nuestro documento Markdown - HTML Tags -->

# Sintaxis Básica Markdown

**Markdown** es un lenguaje de marcado ligero (***Lightweight Markup Language***);siendo **RMarkdown**[^1] uno de sus dialectos, una de sus variantes, uno de sus sabores (**Markdown Flavours**).

[^1]: **RMarkdown es un paquete del lenguaje de programación R, que nos permite crear documento científicos y técnicos en distintos formatos HTML,PDF,Microsoft Word entre otros**

## Encabezados - Títulos

# Título 1

## Título 2

### Título 3

#### Título 4

##### Título 5

##### Título 6

# Título 1

## Título 2

## Separaciones - Línea Horizontal

***

---

***

---

## Citas - Añadir citas a nuestro documento Markdown

> "La tecnología no es nada. Lo importante es que tengas fe en la gente, que sean básicamente buenas e inteligentes, y si les das herramientas, harán cosas maravillosas con ellas".
>
> **Steve Jobs**

## Negrita - Cursiva - Tachado - Subrayado

**Texto formateado como Negrita**

*Texto formateado como Cursiva*

***Texto formateado como Negrita y Cursiva***

~~Texto tachado~~

<u>Texto subrayado</u> <!-- HTML Tags -->


[Regresa Inicio Documento](##Encabezados - Títulos)

## Listas

### Lista Viñetas - Lista Anidada

-   Lista 1
-   Lista 2
-   Lista 3
-   Lista 4
-   Lista 5
    -   Lista 5.1
    -   Lista 5.2
    -   Lista 5.3
-   Lista 6
-   Lista 7
-   Lista 8

### Lista Numerada

1.  Lista 1
2.  Lista 2
3.  Lista 3
4.  Lista 4
5.  Lista 5
6.  Lista 6

### Lista ordenada alfabéticamente

a.  Lista A
b.  Lista B
c.  Lista C
d.  Lista D
e.  Lista E
f.  Lista F

### Lista Tareas

-   [ ] TAREA A
-   [ ] TAREA B
-   [ ] TAREA C
-   [ ] TAREA D
-   [ ] TAREA E
-   [ ] TAREA F

### Casos - Ejemplos

-   Lista 1
-   Lista 2
-   Lista 3
-   Lista 4
-   Lista 5
-   Lista 6
-   Lista 7
-   Lista 8
-   Lista 9

1.  Lista 1
2.  Lista 2
3.  Lista 3
4.  Lista 4
5.  Lista 5
6.  Lista 6

## Enlaces - Añadir links a nuestro documento Markdown

<https://www.youtube.com>

[YouTube](https://www.youtube.com)

[YouTube](https://www.youtube.com "Ingresar a YouTube")

## Imágenes - Añadir imágenes a nuestro documento Markdown

<center>

![](F:%5CDISCO3%5CDocuments%5Cpython_folium%5Clenguaje_R.png)

![](https://d33wubrfki0l68.cloudfront.net/aee91187a9c6811a802ddc524c3271302893a149/a7003/images/bandthree2.png)

</center>

## Tablas - Añadir tablas a nuestro documento Markdown

| TABLA A | TABLA B | TABLA C |
|:-------:|:-------:|:-------:|
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |
|    A    |    B    |    C    |



## Mapas - Añadir mapas a nuestro documento Markdown

<center>

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3901.980822578654!2d-77.03197518561798!3d-12.044840345143056!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8b5d35662c7%3A0x15f0bda5ccbd31eb!2sPalacio%20de%20Gobierno%20del%20Per%C3%BA!5e0!3m2!1ses!2spe!4v1645459221285!5m2!1ses!2spe" width="600" height="450" style="border:0;" allowfullscreen loading="lazy" data-external="1">

</iframe>

</center>

## Código - Añadir código de distintos lenguajes de programación a nuestro documento Markdown (R - Python - SQL)

    summary(mtcars$cyl)

La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.

    x <- table(mtcars$cyl)

    colores <- c("orange","blue","purple")

    barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)

``` r
y <- table(mtcars$gear)

barplot(y,xlab="Engranajes",ylab="Frecuencias",main="Número de Cilindros",col=rainbow(3))
```

``` python
import matplotlib.pyplot as plt

eje_x=[4,6,8]

eje_y=[11,7,14]

colores=['orange','blue','purple']

plt.bar(eje_x,eje_y,color=colores)

plt.title('Número de Cilindros')

plt.xlabel('Cilindros')

plt.ylabel('Frecuencias')

plt.show()
```

    SELECT id_usuario.usuario_nombre,usuario_apellido FROM usuario;

``` sql
USE Northwind;

SELECT * FROM Products;
```

## Anular Sintaxis Markdown

\# Esto debería ser un título tipo 1

\*\*Esto debería ser texto formateado como Negrita\*\*

\*Esto debería ser texto formateado como cursiva\*

## Pie de página

## Ecuaciones - Fórmulas - Sintaxis y comandos LaTeX, añadir ecuaciones y fórmulas a nuestro documento Markdown

### Superíndice - Potencia

$$
E=mc^2
$$

------------------------------------------------------------------------

$$
a^2 + b^2 = c^2
$$

------------------------------------------------------------------------

### Subíndice

$$
H_2O
$$

------------------------------------------------------------------------

$$
NH_3
$$

------------------------------------------------------------------------

### Fracciones - Casos - Ejemplos

$$
\frac{1}{2}
$$

$$
\frac{4}{5} + \frac{7}{8}
$$

$$
\frac{4}{5} - \frac{8}{6}
$$

$$
\frac{6}{7} \times \frac{9}{4}
$$

$$
\frac{1}{2} \cdot \frac{4}{6}
$$

$$
\frac{4}{7} \div \frac{9}{3}
$$

$$
(\frac{6}{7})
$$

$$
\left(\frac{4}{6}\right)^2
$$

Dada la fracción $\tfrac{5}{6}$, podemos determinar el valor de la variable...

Dada la fracción $\frac{5}{6}$, podemos determinar el valor de la variable...

Dada la fracción $\dfrac{5}{6}$, podemos determinar el valor de la variable...

### Sumatoria

$$
\sum_{i=1}^5 i
$$

$$
\sum_{i=1}^5 2i
$$

$$
\sum_{i=2}^7 \frac{i^2}{i+1}
$$

### Logaritmos

$$
\log_7{49} = 2
$$

$$
log_6{216} = 3
$$

$$
\log_3{81}= 4
$$

### Raíces

$$
\sqrt{2} 
$$

$$
\sqrt{3}
$$

$$
\sqrt{4}
$$

$$
\sqrt[3]{\frac{250}{25}}
$$

### Matrices

$$
\begin{matrix}
7 & 9 & 10 \\
10 & 5 & 7 \\
11 & 8 & 5
\end{matrix}
$$

$$
\begin{pmatrix}
7 & 9 & 10 \\
10 & 5 & 7 \\
11 & 8 & 5
\end{pmatrix}
$$

$$
\begin{bmatrix}
7 & 9 & 10 \\
10 & 5 & 7 \\
11 & 8 & 5
\end{bmatrix}
$$

$$
\begin{Bmatrix}
7 & 9 & 10 \\
10 & 5 & 7 \\
11 & 8 & 5
\end{Bmatrix}
$$

$$
\begin{vmatrix}
7 & 9 & 10 \\
10 & 5 & 7 \\
11 & 8 & 5
\end{vmatrix}
$$

$$
\begin{Vmatrix}
7 & 9 & 10 \\
10 & 5 & 7 \\
11 & 8 & 5
\end{Vmatrix}
$$

### Ecuaciones

Dada la función

$$
\begin{equation}
f(x)=y
\end{equation}
$$

podemos determinar el valor de la variable

$$
\text{Fórmula Ecuación 2º Grado}\quad x=\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

### Símbolos Matemáticos

$$
[900]
$$

$$
(900)
$$

$$
|900|
$$

$$
\|900\|
$$

$$
900 > 877
$$

$$
900 < 765
$$

$$
900 >= 876
$$

$$
344 <= 788
$$
