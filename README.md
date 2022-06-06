# Diccionarios en python
Un diccionario es un tipo de datos que sirve para asociar pares de objetos.

Un diccionario puede ser visto como una colección de llaves, cada una de las cuales tiene asociada un valor. Las llaves no están ordenadas y no hay llaves repetidas. La única manera de acceder a un valor es a través de su llave.

# Ejercicio 1
```python
a = {'a': 14, 'b': 23, 'c': 88}
b = {12: True, 55: False, -2: False}
c = dict()
d = {1: [2, 3, 4], 5: [6, 7, 8, 9], 10: [11]}
e = {2 + 3: 4, 5: 6 + 7, 8: 9, 10: 11 + 12}
```

# Recorrido de diccionarios

1. Escriba una función hay_llaves_pares(d) que indique si el diccionario d tiene alguna llave que sea un número par.

```python
d1 = {1: 2, 3: 5}
d2 = {2: 1, 6: 7}
hay_valores_pares(d1)
True
hay_valores_pares(d2)
False
hay_llaves_pares(d1)
False
hay_llaves_pares(d2)
True
```

---
2. Escriba una función maximo_par(d) que entregue el valor máximo de la suma de una llave y un valor del diccionario d.
```python
d = {5: 1, 4: 7, 9: 0, 2: 2}
maximo_par(d)
11
```
---

3. Escriba una función invertir(d) que entregue un diccionario cuyas llaves sean los valores de d y cuyos valores sean las llaves respectivas.
```python
invertir({1: 2, 3: 4, 5: 6})
{2: 1, 4: 3, 6: 5}
apodos = {
...   'Suazo': 'Chupete',
...   'Sanchez': 'Maravilla',
...   'Medel': 'Pitbull',
...   'Valdivia': 'Mago',
... }
invertir(apodos)
{'Maravilla': 'Sanchez', 'Mago': 'Valdivia', 'Chupete': 'Suazo', 'Pitbull': 'Medel'}
```

# Contar letras y palabras

1. Escriba la función contar_letras(oracion) que retorne un diccionario asociando a cada letra la cantidad de veces que aparece en la oracion
```python
contar_letras('El elefante avanza hacia Asia')
{'a': 8, 'c': 1, 'e': 4, 'f': 1, 'h': 1, 'i': 2, 'l': 2, 'n': 2, 's': 1, 't': 1, 'v': 1, 'z': 1}
```
---

2. Escriba la función contar_vocales(oracion) que retorne un diccionario asociando a cada vocal la cantidad de veces que aparece en la oracion. Si una vocal no aparece en la oración, de todos modos debe estar en el diccionario asociada al valor 0
```python
contar_vocales('El elefante avanza hacia Asia')
{'a': 8, 'e': 4, 'i': 2, 'o': 0, 'u': 0}
```
---

3. Escriba la función contar_iniciales(oracion) que retorne un diccionario asociando a cada letra la cantidad de veces que aparece al principio de una palabra
```python
contar_iniciales('Varias vacas vuelan sobre Venezuela')
{'s': 1', 'v': 4}
```
---

4. Escriba la función obtener_largo_palabras(oracion) que retorne un diccionario asociando a cada palabra su cantidad de letras
```python
obtener_largo_palabras('el gato y el pato son amigos')
{'el': 2, 'son': 3, 'gato': 4, 'y': 1, 'amigos': 6, 'pato': 4}
```
---

5. Escriba la función contar_palabras(oracion) que retorne un diccionario asociando a cada palabra la cantidad de veces que aparece en la oración
```python
contar_palabras('El sobre esta sobre el pupitre')
{'sobre': 2, 'pupitre': 1, 'el': 2, 'esta': 1}
```
---

6. Escriba la función palabras_repetidas(oracion) que retorne una lista con las palabras que están repetidas
```python
palabras_repetidas('El partido termino cero a cero')
['cero']
palabras_repetidas('El sobre esta sobre el mueble')
['el', 'sobre']
palabras_repetidas('Ay, ahi no hay pan')
[]
```
---

fuente: http://progra.usm.cl/apunte/ejercicios/2/recorrido-diccionarios.html
