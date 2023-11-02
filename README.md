# TAREA UNIDAD 2 GRAFOS

Explique las 4 formas de representar los grafos entre las representaciones estáticas y dinámicas a
continuación:

- Matriz de adyacencia
- Listas ligadas de adyacencia
- Multilista de adyacencia
- Matriz de incidencia

### Matriz de adyacencia

En una matriz de adyacencia se representan las conexiones de los vertices por medio del uso de filas y columnas y el uso de unos y ceros, en el caso de que un vertice sea adyacente a otro se escribe un uno (1) en la correspondiente celda y en el caso de que haya adyacencia se coloca un cero (0) [Tambien se escribe 0 en caso de que el vertice de una columna corresponda al vertice de una fila]. La matriz de adyacencia es una representación estatica.

Ejemplo:

```txt

a----b  
|\  /  
| \/  
| /\  
|/  \  
c    d  

     a    b    c    d  
a    0    1    1    1  
b    1    0    1    0  
c    1    1    0    0  
d    1    0    0    0  

```


### Listas ligadas de adyacencia

La lista de adyacencia es muy parecida a la matriz de adyacencia, es una representación de todas las aristas o arcos de un grafo con el uso de una lista ligada donde se almacena la referencia a na lista de los vértices adyacentes de i.

Para organizarla se crea una columna en la que cada fila contiene uno de los valores del grafo, después se agregan más columnas y se van añadinedo los valores adyacentes  ya sea de menor a mayor o de mayor a menor en cada celda, cuando un vertice ya no tiene más vertices adyacentes se omíte la opercación con este y se cuntinua con los restantes.

Ejemplo:    

```txt

1----2  
|\  /  
| \/  
| /\  
|/  \  
3    4  

   |1   |2   |3   |4  
   |2   |1   |3   |  
   |3   |1   |2   |  
   |4   |1   |    |  

```

*En un grafo dirigido sólo se ponen los valores a los que se pueden llegar desde cada vertice*

### Multilista de adyacencia

En la multilista de adyacencia iniciamos con una lista sencilla dónde se encuentran todos los vértices, por cada vertice existen enlaces adicionales a los vertices con los cuales tiene arista cada vertice de la lista inicial inicial.

Ejemplo:  

```txt

     5  
  a----b  
  |\  /7  
 2| \/  
  | /\  
  |/  \3  
  c    d  

   |a   |b5   |c2   |d3  
   |b   |a5   |c7   |  
   |c   |a2   |b7   |  
   |d   |a3   |     |  

```

*Este tipo de lista se usa cuando tenemos un grafo con mucha información*

### Matriz de incidencia

En una matriz de incidencia se nombran las aristas y se escribe un 1 en la matriz se el vertice inside en una arista y un 0 en el caso contrario, a diferencia de la matiz de adyacencia dónde se tienen en cuenta son los vértices

Ejemplo:    

```txt

    e1  
  a----b  
  |\  /e4  
e2| \/  
  | /\  
  |/  \e3  
  c    d  

     e1  e2  e3  e4  
  a  1   1   1   0  
  b  1   0   0   1  
  c  0   1   0   1  
  d  0   0   1   0  

```

## Biblografía

AULA DE MATEMÁTICA. (2020, 1 septiembre). MATRICES DE ADYACENCIA e INCIDENCIA [Vídeo]. YouTube. https://www.youtube.com/watch?v=D7Gk4NOlB4c

CHOCHY. (2021, 22 noviembre). Algoritmos de grafos - lista de adyacencia [Vídeo]. YouTube. https://www.youtube.com/watch?v=KHyGn4cRjN4

Carlos Henriquez. (2020, 23 marzo). Representación grafos: multilista [Vídeo]. YouTube. https://www.youtube.com/watch?v=nb6r_qDNoMk
