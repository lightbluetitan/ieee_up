---
title: "Sintaxis Markdown"
author: "Renzo Cáceres Rossi"
date: "2022/07/01"
subtitle: Markdown - RMarkdown
---

<!-- Añadir comentarios a nuestro documento Markdown - HTML Tags -->

# Sintaxis Básica Markdown


## Encabezados - Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6


## Negrita - Cursiva - Tachado - Subrayado

**Texto formateado como Negrita**

*Texto formateado como Cursiva*

~~Texto tachado~~


<u>Texto subrayado</u> <!--HTML tags-->


## Enlaces - Añadir links a nuestros documentos


<https://www.facebook.com/USAC.CS>

[IEEE USAC](https://www.facebook.com/USAC.CS)

[IEEE USAC](https://www.facebook.com/USAC.CS "Ingresa al IEEE CS USAC")



## Imágenes  - Añadir imágenes a nuestro documento Markdown

<center>

![](logo_r.png)


![](https://d33wubrfki0l68.cloudfront.net/aee91187a9c6811a802ddc524c3271302893a149/a7003/images/bandthree2.png){width=400}

</center>


## Código - Añadir código de R - Python - SQL


    summary(mtcars)
    
La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.    


```
x <- table(mtcars$cyl)

colores <- c(orange,blue,"purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)

```


```Python
import matplotlib.pyplot as plt
 

eje_x = [Python, R, Node.js, 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()

```

    SELECT id_usuario,usuario_nombre.usuario_apellido FROM usuarios;
    
```sql

USE Northwind;

SELECT * FROM Products;

```













