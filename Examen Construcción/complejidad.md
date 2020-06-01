# Examen: Respuesta inciso 40

**Alumno:** Sandoval Bravo Alejandro
**Matrícula:** S18012132

## Algoritmo

```pseint
Funcion juega
inicio
    ret = 0
    Para i=1 hasta 4
    inicio
        Lee a
        Si a<0 entonces
            ret = -1
        de otro modo
            d[i] = a
    end
    Si ret=0 entonces
    inicio
        k = 0
        Mientras k<4
        inicio
            Para j=1 a 3
                e[j] = abs(d[j]) - d[j+1])
            e[4] = abs(d[4]-d[1])
            k = 0
            Para i=1 a 4
            inicio
                d[i] = e[i]
                Si e[i]=0 entonces
                    k = k+1
            fin
            ret = ret+1
        fin
    fin
    Regresa ret
fin
```

## Grafo

![Grafo Parte 1][GRAF]
![Grafo Parte 2][GRAP]


[GRAF]: grafo_1.jpeg "Grafo 1.1"
[GRAP]: grafo_2.jpeg "Grafo 1.2"

## Calculo de complejidad

```
complejidad = rr + 1
            = 6 + 1
            = 7

complejidad = Nodos Predicado + 1
            = 6 + 1
            = 7 + 1

complejidad = Aristas - Nodos + 2
            = 31 - 26 + 2
            = 33 - 26
            = 7
```
