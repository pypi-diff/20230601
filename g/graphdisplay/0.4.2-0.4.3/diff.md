# Comparing `tmp/graphdisplay-0.4.2.tar.gz` & `tmp/graphdisplay-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.4.2.tar", last modified: Tue May 30 07:40:39 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.3.tar", last modified: Thu Jun  1 11:51:08 2023, max compression
```

## Comparing `graphdisplay-0.4.2.tar` & `graphdisplay-0.4.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:40:39.134507 graphdisplay-0.4.2/
--rw-rw-rw-   0        0        0     5408 2023-05-30 07:40:39.133501 graphdisplay-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:40:39.091488 graphdisplay-0.4.2/graphdisplay/
--rw-rw-rw-   0        0        0      101 2023-05-16 13:30:34.000000 graphdisplay-0.4.2/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     2148 2023-05-29 18:05:23.000000 graphdisplay-0.4.2/graphdisplay/about_win_manager.py
--rw-rw-rw-   0        0        0     5148 2023-05-30 07:40:26.000000 graphdisplay-0.4.2/graphdisplay/general_config.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:40:39.104453 graphdisplay-0.4.2/graphdisplay/graphs/
--rw-rw-rw-   0        0        0       24 2023-05-16 13:30:34.000000 graphdisplay-0.4.2/graphdisplay/graphs/__init__.py
--rw-rw-rw-   0        0        0    23057 2023-05-30 06:46:16.000000 graphdisplay-0.4.2/graphdisplay/graphs/graph.py
--rw-rw-rw-   0        0        0     7686 2023-05-24 10:13:04.000000 graphdisplay-0.4.2/graphdisplay/json_manager.py
--rw-rw-rw-   0        0        0    35596 2023-05-30 07:27:26.000000 graphdisplay-0.4.2/graphdisplay/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:40:39.105450 graphdisplay-0.4.2/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.4.2/graphdisplay/store/__init__.py
--rw-rw-rw-   0        0        0    17294 2023-05-30 06:46:16.000000 graphdisplay-0.4.2/graphdisplay/tools_win_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:40:39.132502 graphdisplay-0.4.2/graphdisplay/trees/
--rw-rw-rw-   0        0        0       88 2023-05-16 13:30:34.000000 graphdisplay-0.4.2/graphdisplay/trees/__init__.py
--rw-rw-rw-   0        0        0     3612 2023-05-16 13:30:34.000000 graphdisplay-0.4.2/graphdisplay/trees/auto_balance_tree.py
--rw-rw-rw-   0        0        0     3253 2023-05-27 13:25:51.000000 graphdisplay-0.4.2/graphdisplay/trees/binary_search_tree.py
--rw-rw-rw-   0        0        0     6197 2023-05-28 10:30:46.000000 graphdisplay-0.4.2/graphdisplay/trees/binary_tree.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:40:39.101461 graphdisplay-0.4.2/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     5408 2023-05-30 07:40:38.000000 graphdisplay-0.4.2/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-05-30 07:40:38.000000 graphdisplay-0.4.2/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:40:38.000000 graphdisplay-0.4.2/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 07:40:38.000000 graphdisplay-0.4.2/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 07:40:39.135495 graphdisplay-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-05-19 10:30:27.000000 graphdisplay-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.478979 graphdisplay-0.4.3/
+-rw-rw-rw-   0        0        0     6795 2023-06-01 11:51:08.477986 graphdisplay-0.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.454082 graphdisplay-0.4.3/graphdisplay/
+-rw-rw-rw-   0        0        0      101 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-01 09:21:30.000000 graphdisplay-0.4.3/graphdisplay/about_win_manager.py
+-rw-rw-rw-   0        0        0     5199 2023-06-01 11:51:06.000000 graphdisplay-0.4.3/graphdisplay/general_config.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.470458 graphdisplay-0.4.3/graphdisplay/graphs/
+-rw-rw-rw-   0        0        0       24 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/graphs/__init__.py
+-rw-rw-rw-   0        0        0    23057 2023-05-30 06:46:16.000000 graphdisplay-0.4.3/graphdisplay/graphs/graph.py
+-rw-rw-rw-   0        0        0     7686 2023-05-24 10:13:04.000000 graphdisplay-0.4.3/graphdisplay/json_manager.py
+-rw-rw-rw-   0        0        0    36268 2023-06-01 09:58:48.000000 graphdisplay-0.4.3/graphdisplay/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.471456 graphdisplay-0.4.3/graphdisplay/store/
+-rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.4.3/graphdisplay/store/__init__.py
+-rw-rw-rw-   0        0        0    17294 2023-05-30 06:46:16.000000 graphdisplay-0.4.3/graphdisplay/tools_win_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.477441 graphdisplay-0.4.3/graphdisplay/trees/
+-rw-rw-rw-   0        0        0       88 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/trees/__init__.py
+-rw-rw-rw-   0        0        0     3612 2023-05-16 13:30:34.000000 graphdisplay-0.4.3/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-rw-   0        0        0     3253 2023-05-27 13:25:51.000000 graphdisplay-0.4.3/graphdisplay/trees/binary_search_tree.py
+-rw-rw-rw-   0        0        0     6197 2023-05-28 10:30:46.000000 graphdisplay-0.4.3/graphdisplay/trees/binary_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:51:08.467469 graphdisplay-0.4.3/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     6795 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 11:51:08.000000 graphdisplay-0.4.3/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:51:08.479977 graphdisplay-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2023-06-01 10:05:17.000000 graphdisplay-0.4.3/setup.py
```

### Comparing `graphdisplay-0.4.2/PKG-INFO` & `graphdisplay-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,98 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.2
-Summary: Librería para representar visualmente grafos de tipo diccionario
+Version: 0.4.3
+Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
-Author: Alberto Penas Díaz
+Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
-# graphdisplay
+<p align="center">
+  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
+  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
+  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
+</p>
 
-## Resumen
+## 💡Resumen
 
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
-Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
 
-## ¿Quieres contribuir?
+## ⚡️¿Quieres contribuir?
 
 Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
 en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
 
-## Método de uso 
+## 📐Método de uso
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
-para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
-antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
-grafos grandes y complejos:
-+ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
-de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
-implementación de grafos que viene por defecto con el paquete.
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
+asignatura, por lo que también son importables.
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón. 
+Junto con el grafo, el resto de argumentos son los siguientes: 
++ graph: es el objeto de tipo grafo/árbol que se va a representar **ES MUY IMPORTANTE** que éste sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la implementación de grafos que viene por defecto con el paquete.
 + node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
 ```python
+from graphdisplay import GraphGUI, Graph
+
 g = Graph([1, 2, 3])
 g.addEdge(1, 2)
 g.addEdge(2, 3)
 
 # Para representar el grafo con todos los valores por defecto
 GraphGUI(g)
 
-# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
-GraphGUI(g, 32, 700, 700)
-
-# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
-GraphGUI(g, scr_width=200)
+# Para ajustar el radio de los nodos a 32, y el tema a 'dark'
+GraphGUI(g, node_radius=32, theme='dark')
 ```
+Ejemplo con árboles binarios de búsqueda:
+```python
+from graphdisplay import GraphGUI, BinarySearchTree
+from random import randint
 
-Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
+tree = BinarySearchTree()
+for _ in range(80):
+    tree.insert(randint(1, 1000))
+   
+GraphGUI(tree)
+```
 
-## Ejemplo de uso
+## ⚡️Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
+después poder cargarlo en cualquier momento.
+
+Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
+al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
+Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
+issue #16
+## 🎯Ejemplos de uso
 
 Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
+from graphdisplay import GraphGUI, Graph
+
 labels = ['A', 'B', 'C', 'D', 'E']
 g = Graph(labels)
 
 # Now, we add the edges
 g.addEdge('A', 'C', 12)  # A->(12)C
 g.addEdge('A', 'D', 60)  # A->(60)D
 g.addEdge('B', 'A', 10)  # B->(10)A
@@ -84,13 +105,16 @@
 Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
 
 ```python
     GraphGUI(g)
 ```
 Y nos mostrará la ventana:
 
-<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/0abc6d79-120e-470f-8d9b-7035e38def40" width="400" height="400">
+
+Sabiendo cómo instanciar grafos y reorganiando un poco los vértices, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 25, theme="la gran ola")`
 
-Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/a1edfcbf-4cec-4b08-98c6-709b87b7892d" width="800" height="500">
 
-<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
+De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
 
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/3afa798a-28c3-4c6f-9357-8d849018dfa5" width="1000" height="480">
```

### Comparing `graphdisplay-0.4.2/README.md` & `graphdisplay-0.4.3/graphdisplay.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,98 @@
-# graphdisplay
+Metadata-Version: 2.1
+Name: graphdisplay
+Version: 0.4.3
+Summary: Librería para representar grafos visualmente
+Home-page: https://github.com/seniorbeto
+Author: Alberto Penas Díaz (@seniorbeto)
+Author-email: albertopenasdiaz@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
+  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
+  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
+</p>
 
-## Resumen
+## 💡Resumen
 
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
-Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
 
-## ¿Quieres contribuir?
+## ⚡️¿Quieres contribuir?
 
 Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
 en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
 
-## Método de uso 
+## 📐Método de uso
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
-para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
-antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
-grafos grandes y complejos:
-+ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
-de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
-implementación de grafos que viene por defecto con el paquete.
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
+asignatura, por lo que también son importables.
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón. 
+Junto con el grafo, el resto de argumentos son los siguientes: 
++ graph: es el objeto de tipo grafo/árbol que se va a representar **ES MUY IMPORTANTE** que éste sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la implementación de grafos que viene por defecto con el paquete.
 + node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
 ```python
+from graphdisplay import GraphGUI, Graph
+
 g = Graph([1, 2, 3])
 g.addEdge(1, 2)
 g.addEdge(2, 3)
 
 # Para representar el grafo con todos los valores por defecto
 GraphGUI(g)
 
-# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
-GraphGUI(g, 32, 700, 700)
-
-# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
-GraphGUI(g, scr_width=200)
+# Para ajustar el radio de los nodos a 32, y el tema a 'dark'
+GraphGUI(g, node_radius=32, theme='dark')
 ```
+Ejemplo con árboles binarios de búsqueda:
+```python
+from graphdisplay import GraphGUI, BinarySearchTree
+from random import randint
 
-Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
+tree = BinarySearchTree()
+for _ in range(80):
+    tree.insert(randint(1, 1000))
+   
+GraphGUI(tree)
+```
 
-## Ejemplo de uso
+## ⚡️Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
+después poder cargarlo en cualquier momento.
+
+Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
+al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
+Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
+issue #16
+## 🎯Ejemplos de uso
 
 Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
+from graphdisplay import GraphGUI, Graph
+
 labels = ['A', 'B', 'C', 'D', 'E']
 g = Graph(labels)
 
 # Now, we add the edges
 g.addEdge('A', 'C', 12)  # A->(12)C
 g.addEdge('A', 'D', 60)  # A->(60)D
 g.addEdge('B', 'A', 10)  # B->(10)A
@@ -67,13 +105,16 @@
 Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
 
 ```python
     GraphGUI(g)
 ```
 Y nos mostrará la ventana:
 
-<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/0abc6d79-120e-470f-8d9b-7035e38def40" width="400" height="400">
+
+Sabiendo cómo instanciar grafos y reorganiando un poco los vértices, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 25, theme="la gran ola")`
 
-Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/a1edfcbf-4cec-4b08-98c6-709b87b7892d" width="800" height="500">
 
-<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
+De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
 
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/3afa798a-28c3-4c6f-9357-8d849018dfa5" width="1000" height="480">
```

### Comparing `graphdisplay-0.4.2/graphdisplay/about_win_manager.py` & `graphdisplay-0.4.3/graphdisplay/about_win_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         buton.pack(side=tk.BOTTOM)
 
         self.canvas = tk.Canvas(self, width=400, height=400, bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
         self.canvas.pack()
         self.turtle = turtle.RawTurtle(self.canvas, visible=False)
         self.canvas.configure(bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
         self.turtle.speed(0)
+        self.canvas.create_text(0, -100, text="by @seniorbeto",
+                                fill=self.__graphgui._AUTHOR_NAME_COLOR, font=("Courier", 15))
         text = "GraphDisplay v"+VERSION
         self.canvas.create_text(0, -150, text=text, font=("Courier", 20),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
         self.canvas.create_text(0, 147, text="An open source proyect made", font=("Courier", 13),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
         self.canvas.create_text(0, 165, text="by and for students!", font=("Courier", 13),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
```

### Comparing `graphdisplay-0.4.2/graphdisplay/general_config.py` & `graphdisplay-0.4.3/graphdisplay/general_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-VERSION = '0.4.2'
+VERSION = '0.4.3'
+DEFAULT_SCR_WIDTH = 600
+DEFAULT_SCR_HEIGHT = 600
 BUTTON_HEIGHT = 30
 BUTTON_WIDTH = 60
 XMARGEN = 7
 YMARGEN = 7
 THEMES = {
     "BROWN":{
         "BUTTON_COLOR": "#ede4cc",
```

### Comparing `graphdisplay-0.4.2/graphdisplay/graphs/graph.py` & `graphdisplay-0.4.3/graphdisplay/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.2/graphdisplay/json_manager.py` & `graphdisplay-0.4.3/graphdisplay/json_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.2/graphdisplay/main.py` & `graphdisplay-0.4.3/graphdisplay/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,35 +30,31 @@
     :param scr_height: The height of the window.
     :param theme: color scheme of the node display.
     """
 
     # Using a instance-counter will determine how many GraphGUI objects are wanted
     instance = 0
 
-    def __new__(cls, graph, node_radius: int = 30, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
+    def __new__(cls, graph, node_radius: int = 30, theme: str = 'BROWN'):
         GraphGUI.instance += 1
         if GraphGUI.instance > 5:
             raise Exception("For safety reasons, only five instances of GraphGUI can be created")
 
         # Generate multiprocessing
 
         if platform.system() == "Linux":
             mp.Process(target=cls._generate, args=(graph,
                                                     GraphGUI.instance,
                                                     node_radius,
-                                                    scr_width,
-                                                    scr_height,
                                                     theme)).start()
         else:
             try:
                 pid = mp.Process(target=cls._generate, args=(graph,
                                                              GraphGUI.instance,
                                                              node_radius,
-                                                             scr_width,
-                                                             scr_height,
                                                              theme))
                 pid.start()
             except RecursionError:
                 print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "For how GraphGUI works, high-demanding recursion trees are"
                                                                  " not supported. Sorry for the inconvenience. ")
             except RuntimeError:
 
@@ -76,19 +72,19 @@
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def __setattr__(self, name, value):
         return setattr(self.instance, name, value)
 
     @staticmethod
-    def _generate(graph, instance, node_radius, scr_width, scr_height, theme):
-        GraphGUI.__GraphGUI(graph, instance, node_radius, scr_width, scr_height, theme)
+    def _generate(graph, instance, node_radius, theme):
+        GraphGUI.__GraphGUI(graph, instance, node_radius, theme)
 
     class __GraphGUI:
-        def __init__(self, graph, instance, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
+        def __init__(self, graph, instance, node_radius: int = 40, theme: str = 'BROWN'):
             """
             Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
             The creation of the window will stop the execution of the program until the window is closed. Thus, it is recommended
             to create the GraphGUI object at the end of the program.
             :param graph: The graph to be displayed
             :param node_radius: The radius of the nodes (default 40)
             :param scr_width: The width of the window (default 600)
@@ -97,28 +93,22 @@
 
             # Begin time measurement
             start = time.time()
 
             # Parameter validation
             if type(node_radius) != int:
                 raise TypeError("The parameter node_radius must be an integer")
-            if type(scr_width) != int or type(scr_height) != int:
-                raise TypeError("The parameters scr_width and scr_height must be integers")
             if node_radius < 10 or node_radius > 100:
                 raise ValueError("The parameter node_radius must be a value between 10 and 100")
-            if scr_width < 200 or scr_height < 200:
-                raise ValueError("The parameters scr_width and scr_height must be values greater than 200")
-            if scr_width > 2000 or scr_height > 2000:
-                raise ValueError("The parameters scr_width and scr_height must be values less than 2000")
 
             self.__ACTUAL_INSTANCE = instance
             self._graph = graph
             self.__node_radius = node_radius
-            self.__scr_width = scr_width
-            self.__scr_height = scr_height
+            self.__scr_width = DEFAULT_SCR_WIDTH
+            self.__scr_height = DEFAULT_SCR_WIDTH
             self.__XMARGIN = XMARGEN
             self.__YMARGIN = YMARGEN
             self._theme = theme.upper()
             self.nodes = []
             self.edges = []
             self.__canvas_node_relation = {}
             try:
@@ -155,34 +145,46 @@
                 for vertex in graph._vertices:
                     for adj in graph._vertices[vertex]:
                         self._graph.addEdge(vertex, adj._vertex, adj._weight)
 
             # Create the main window
             self.root = tk.Tk()
             self.root.title('GraphGUI')
-            self.root.resizable(False, False)
-            self.root.configure(bg=self._FRAME_COLOR, border=0, width=self.__scr_width, height=self.__scr_height)
+            self.root.geometry(f"{self.__scr_width}x{self.__scr_height}")
+            self.root.configure(bg=self._FRAME_COLOR, border=0)
+
+            # Button Frame
+            self.button_frame = tk.Frame(self.root, bg=self._FRAME_COLOR,
+                                         height=self.__YMARGIN + BUTTON_HEIGHT)
+            self.button_frame.pack(fill='x', side='bottom')
+
+            # Canvas Frame
+            self.__canvas_frame = tk.Frame(self.root, bg=self._BACKGROUND_CANVAS_COLOR)
+            self.__canvas_frame.pack(expand=1, fill='both', pady=self.__YMARGIN, padx=self.__XMARGIN)
 
             # Closing protocol
             self.root.protocol("WM_DELETE_WINDOW", self.__on_closing)
 
             # Canvas creation and placement
-            self.canvas = tk.Canvas(self.root, bg=self._BACKGROUND_CANVAS_COLOR, bd=0)
-            self.canvas.place(x=self.__XMARGIN,
-                              y=self.__YMARGIN,
-                              width=self.__scr_width - self.__XMARGIN * 2,
-                              height=self.__scr_height - self.__YMARGIN * 2 - BUTTON_HEIGHT)
+            self.canvas = tk.Canvas(self.__canvas_frame, bg=self._BACKGROUND_CANVAS_COLOR, bd=0,
+                                    width=self.__scr_width - self.__XMARGIN * 2,
+                                    height=self.__scr_height - self.__YMARGIN * 2 - BUTTON_HEIGHT)
+            self.canvas.pack(fill='both', expand=1)
 
             # Buttons display
             self.__display_buttons()
 
             # Main display
             self.json_manager = JsonManager(self.root, self)
             data = self.json_manager.get_data('__last_store_'+str(self.__ACTUAL_INSTANCE))
             self.__display(data)
+            if data:
+                actual_scr_width = data['Screen_dimensions'][0]
+                actual_scr_height = data['Screen_dimensions'][1]
+                self.root.geometry(f'{actual_scr_width}x{actual_scr_height}')
 
             # Tag_bind for movable canvas objects
             self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
             if self._is_tree and platform.system() != "Linux":
                 self.canvas.tag_bind("movil", "<Button-3>", self.on_press_left)
             self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
             self.selected_node = None
@@ -192,60 +194,73 @@
             print("Displayed in:", round(end-start, 4))
 
             # Main display protocol
             self.root.mainloop()
 
         def __display_buttons(self):
             # Reset button
-            self.reset_button = tk.Button(self.root, text="Reset", bg=self._BUTTON_COLOR, command=self.display_reset,
+            self.reset_button = tk.Button(self.button_frame,
+                                          text="Reset",
+                                          bg=self._BUTTON_COLOR,
+                                          command=self.display_reset,
                                           bd=0)
-            self.reset_button.place(x=self.__XMARGIN,
-                                    y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
+            self.reset_button.place(x = self.__XMARGIN,
+                                    y = 0,
                                     width=BUTTON_WIDTH,
                                     height=BUTTON_HEIGHT)
 
             # Load button
-            self.load_button = tk.Button(self.root, text="Load", bg=self._BUTTON_COLOR,
+            self.load_button = tk.Button(self.button_frame,
+                                         text="Load",
+                                         bg=self._BUTTON_COLOR,
                                          command=self.__call_manager_load,
                                          bd=0)
             self.load_button.place(x=self.__XMARGIN + BUTTON_WIDTH + self.__XMARGIN,
-                                   y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
+                                   y=0,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
             # Save button
-            self.save_button = tk.Button(self.root, text="Save", bg=self._BUTTON_COLOR,
+            self.save_button = tk.Button(self.button_frame,
+                                         text="Save",
+                                         bg=self._BUTTON_COLOR,
                                          command=self.__call_manager_save,
                                          bd=0)
             self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 2,
-                                   y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
+                                   y=0,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
             # Delete button
-            self.save_button = tk.Button(self.root, text="Delete", bg=self._BUTTON_COLOR,
+            self.save_button = tk.Button(self.button_frame,
+                                         text="Delete",
+                                         bg=self._BUTTON_COLOR,
                                          command=self.__call_manager_delete, bd=0)
             self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 3,
-                                   y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
-                                   width=BUTTON_WIDTH,
-                                   height=BUTTON_HEIGHT)
-
-            # About button
-            self.save_button = tk.Button(self.root, text="About", bg=self._BUTTON_COLOR,
-                                         command=self.__call_about_window, bd=0)
-            self.save_button.place(x=self.__scr_width - self.__XMARGIN - BUTTON_WIDTH,
-                                   y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
+                                   y=0,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
             # Tools button
-            self.save_button = tk.Button(self.root, text="Tools", bg=self._BUTTON_COLOR,
+            self.save_button = tk.Button(self.button_frame,
+                                         text="Tools",
+                                         bg=self._BUTTON_COLOR,
                                          command=self.__call_tools_window, bd=0)
             self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 4,
-                                   y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
+                                   y=0,
+                                   width=BUTTON_WIDTH,
+                                   height=BUTTON_HEIGHT)
+
+            # About button
+            self.save_button = tk.Button(self.button_frame,
+                                         text="About",
+                                         bg=self._BUTTON_COLOR,
+                                         command=self.__call_about_window, bd=0)
+            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 5,
+                                   y=0,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
         def __call_tools_window(self):
             """Generator of ToolWindow"""
             ToolWindow(self.root, self)
 
@@ -269,14 +284,17 @@
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
         def __call_manager_save(self):
             """Generator of Save Window"""
             if not self._is_tree:
                 curr_pos = {}
+                actual_scr_width = self.root.winfo_width()
+                actual_scr_height = self.root.winfo_height()
+                curr_pos['Screen_dimensions'] = (actual_scr_width, actual_scr_height)
                 for node in self.nodes:
                     curr_pos[node.id] = (node.pos_x, node.pos_y)
                 self.json_manager.generate_save_window(curr_pos)
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
         def display_reset(self, new_data: dict = None):
@@ -293,31 +311,43 @@
             If data is None, the default display will be showed. This is, in case of a simple graph,
             the first vertex in the middle of the screen and the rest surrounding it in a polygon shape.
             In case of a tree, it is always display in a tree-like structure.
 
             This function also checks if some node position has been stored outside the frames of the window,
             in which case will correct.
             """
+            # First, we store the actual dimensions of the screen
+            if data:
+                actual_scr_width = data['Screen_dimensions'][0]
+                actual_scr_height = data['Screen_dimensions'][1]
+            else:
+                actual_scr_width = self.root.winfo_width()
+                actual_scr_height = self.root.winfo_height()
+
+            # Now, we will restrict the screen to the canvas dimensions
+            actual_scr_width -= self.__XMARGIN * 2
+            actual_scr_height -= self.__YMARGIN * 2 + BUTTON_HEIGHT
+
             if not self._is_tree:
                 # Preparation for the nodes display
-                scr_center = ((self.__scr_width - 14) // 2, (self.__scr_height - 30) // 2)
-                display_radius = min(self.__scr_width - 30 - self.__node_radius, self.__scr_height - 14 - self.__node_radius) // 2 - self.__node_radius - 10
+                scr_center = ((actual_scr_width - 14) // 2, (actual_scr_height - 30) // 2)
+                display_radius = min(actual_scr_width - 30 - self.__node_radius, actual_scr_height - 14 - self.__node_radius) // 2 - self.__node_radius - 10
                 arch_angle = 360 / len(self._graph._vertices)
                 first_node_pos = (scr_center[0] - self.__node_radius, scr_center[1] - self.__node_radius)
 
                 # Display the nodes
                 self.nodes = []
                 i = 0
                 angle = 0
                 for vertex in self._graph._vertices:
                     # The first vertex will be displayed in the screen center
                     if i == 0:
                         if data and str(vertex) in data and \
-                                data[str(vertex)][0] < self.__scr_width and \
-                                data[str(vertex)][1] < self.__scr_height - 30 and \
+                                data[str(vertex)][0] < actual_scr_width and \
+                                data[str(vertex)][1] < actual_scr_height - 30 and \
                                 data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                                 data[str(vertex)][1] + self.__node_radius*2 > 0:
                             self.nodes.append(
                                 Node(self.canvas,
                                      self.__node_radius,
                                      data[str(vertex)][0],
                                      data[str(vertex)][1],
@@ -331,16 +361,16 @@
                                      first_node_pos[1],
                                      text=vertex,
                                      bg=self._VERTEX_COLOR))
                     else:
                         # Those vertices that are not the first, will surround the screen center, scrolling
                         # around an imaginary circumference.
                         if data and str(vertex) in data and \
-                                data[str(vertex)][0] < self.__scr_width and \
-                                data[str(vertex)][1] < self.__scr_height - 30 and \
+                                data[str(vertex)][0] < actual_scr_width and \
+                                data[str(vertex)][1] < actual_scr_height - 30 and \
                                 data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                                 data[str(vertex)][1] + self.__node_radius*2 > 0:
                             self.nodes.append(
                                 Node(self.canvas,
                                      self.__node_radius,
                                      data[str(vertex)][0],
                                      data[str(vertex)][1],
@@ -394,42 +424,42 @@
                         edge.show()
 
             elif self._is_tree:
                 # The tree display is slightly more complicated (it was a complete nightmare for a one man job
                 # to be honest). For information on how it works, please consider visiting: #TODO
                 self.nodes = []
                 self.edges = []
-                root_position = ((self.__scr_width - self.__node_radius*2) // 2, self.__YMARGIN + 33)
+                root_position = ((actual_scr_width - self.__node_radius*2) // 2, self.__YMARGIN + 33)
                 self.nodes.append(Node(self.canvas,
                                        self.__node_radius,
                                        root_position[0],
                                        root_position[1],
                                        text=self._graph._root.elem,
                                        bg=self._VERTEX_COLOR))
 
                 # We display the rest of the nodes in a tree-like structure by
                 # dividing the screen in levels and displaying the nodes in each level
                 level_order = self.__levelorder(self._graph._root)
                 levels = max(level_order.values()) + 1
-                level_height = (self.__scr_height - self.__YMARGIN - 60) // levels
+                level_height = (actual_scr_height - self.__YMARGIN - 60) // levels
 
                 # We determine how many nodes are in each level
                 last_nodes = [self._graph._root.elem]
                 for i in range(levels - 1):
                     if i != 0:
                         last_nodes = nodes_in_level
                     nodes_in_level = []
                     for node in level_order:
                         if level_order[node] == i + 1:
                             nodes_in_level.append(node)
 
                     level_grid = 2**(i + 1)
 
                     # We determine the x_axis of each node in the level
-                    x_axis = (self.__scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2)) // level_grid
+                    x_axis = (actual_scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2)) // level_grid
                     x_axis_counter = 0
 
                     final_nodes = nodes_in_level + last_nodes
                     final_nodes.sort()
                     for node in last_nodes:
                         # We look for the position x of the father
                         for aux in self.nodes:
@@ -458,16 +488,16 @@
                             new_edge.show()
                             self.edges.append(new_edge)
                             new_node.asociated_edges_IN.append(new_edge)
                             father_node.asociated_edges_OUT.append(new_edge)
 
                         if children_right or children_right == 0:
                             final_position_x = position_x + x_axis // 2
-                            if final_position_x >= self.__scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2) - 5:
-                                final_position_x = self.__scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2) - 5
+                            if final_position_x >= actual_scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2) - 5:
+                                final_position_x = actual_scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2) - 5
 
                             new_node = Node(self.canvas,
                                             self.__node_radius,
                                             final_position_x,
                                             root_position[1] + level_height*(level_order[children_right]),
                                             text=children_right,
                                             bg=self._VERTEX_COLOR)
@@ -478,19 +508,14 @@
                                             None,
                                             window_color=self._BACKGROUND_CANVAS_COLOR)
                             new_edge.show()
                             self.edges.append(new_edge)
                             new_node.asociated_edges_IN.append(new_edge)
                             father_node.asociated_edges_OUT.append(new_edge)
 
-
-            # Display author
-            self.__autor = self.canvas.create_text(self.__scr_width // 2, self.__YMARGIN + 3, text="by @seniorbeto",
-                                                   fill=self._AUTHOR_NAME_COLOR, font=("Courier", 10))
-
             # We will store each canvas TAGorID with each associated node object in order
             # to reduce movement complexity to O(1)
             self.__canvas_node_relation = {}
             for node in self.nodes:
                 self.__canvas_node_relation[node.circle] = node
                 self.__canvas_node_relation[node.text] = node
 
@@ -532,14 +557,17 @@
                     register[current.right.elem] = value + 1
 
             return register
 
         def __on_closing(self):
             """Store the current data at closing protocol"""
             data = {}
+            actual_scr_width = self.root.winfo_width()
+            actual_scr_height = self.root.winfo_height()
+            data['Screen_dimensions'] = (actual_scr_width, actual_scr_height)
             for node in self.nodes:
                 data[node.id] = (node.pos_x, node.pos_y)
             self.json_manager.save_data('__last_store_'+str(self.__ACTUAL_INSTANCE), data)
             self.root.destroy()
 
         def on_press_left(self, event):
             """
@@ -553,16 +581,14 @@
                         vertices = self.__levelorder(root)
                         new_tree = copy.copy(self._graph)
                         new_tree.remove_all()
                         for i in list(vertices.keys()):
                             new_tree.insert(i)
                 GraphGUI(new_tree,
                          self.__node_radius,
-                         self.__scr_width,
-                         self.__scr_height,
                          self._theme)
 
         def on_press(self, event):
             """Right mouse click protocol"""
             # Store the node if it has been right-clicked
             node = self.canvas.find_withtag(tk.CURRENT)
             self.selected_node = (node, event.x, event.y)
```

### Comparing `graphdisplay-0.4.2/graphdisplay/tools_win_manager.py` & `graphdisplay-0.4.3/graphdisplay/tools_win_manager.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.2/graphdisplay/trees/auto_balance_tree.py` & `graphdisplay-0.4.3/graphdisplay/trees/auto_balance_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.2/graphdisplay/trees/binary_search_tree.py` & `graphdisplay-0.4.3/graphdisplay/trees/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.2/graphdisplay/trees/binary_tree.py` & `graphdisplay-0.4.3/graphdisplay/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.2/graphdisplay.egg-info/SOURCES.txt` & `graphdisplay-0.4.3/graphdisplay.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 graphdisplay/__init__.py
 graphdisplay/about_win_manager.py
 graphdisplay/general_config.py
 graphdisplay/json_manager.py
 graphdisplay/main.py
 graphdisplay/tools_win_manager.py
```

### Comparing `graphdisplay-0.4.2/setup.py` & `graphdisplay-0.4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from setuptools import find_packages, setup
 from graphdisplay.general_config import *
 
 HERE = pathlib.Path(__file__).parent
 
 VERSION = VERSION
 PACKAGE_NAME = 'graphdisplay'
-AUTHOR = 'Alberto Penas Díaz'
+AUTHOR = 'Alberto Penas Díaz (@seniorbeto)'
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
 URL = 'https://github.com/seniorbeto'
 
 LICENSE = 'MIT' #Tipo de licencia
-DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario'
-LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
+DESCRIPTION = 'Librería para representar grafos visualmente'
+LONG_DESCRIPTION = (HERE / "../../README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = "text/markdown"
 
 
 INSTALL_REQUIRES = [
       'tk==0.1.1'
       ]
```

