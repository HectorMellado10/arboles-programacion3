# Árbol Binario de Búsqueda (BST) en Java

**Estudiante:** Hector Mellado
**Curso:** Programación 3
**Tema:** Estructuras de datos no lineales — Árboles

---

## Cómo compilar y ejecutar

Desde la carpeta `arboles/`:

    javac -d target/classes src/main/java/umg/edu/progra/arboles/*.java
    java -cp target/classes umg.edu.progra.arboles.Principal

---

## Métodos nuevos implementados

### Problema 1 — contarNodos()
Cuenta el total de nodos del árbol usando recursividad, sin usar el campo tamanio.
- Entrada: árbol con 8 nodos
- Salida: contarNodos() = 8 / Coinciden: true

### Problema 2 — esBalanceado()
Verifica que para cada nodo la diferencia de alturas entre subárbol izquierdo y derecho sea <= 1.
- Entrada: árbol {50,30,70,20,40,60,80,10} → esBalanceado() = true
- Entrada: árbol {1,2,3,4,5} cadena → esBalanceado() = false

### Problema 3 — esBSTValido()
Verifica que el árbol cumple la propiedad de BST en todos sus nodos usando un rango (min, max).
- Entrada: BST construido correctamente → esBSTValido() = true
- Entrada: BST con nodo modificado manualmente → esBSTValido() = false

### Problema 4 — ancestroComunMasBajo(int a, int b)
Devuelve el ancestro común más bajo (LCA) de dos valores aprovechando la propiedad del BST.
- Entrada: LCA(10, 40) → 30
- Entrada: LCA(10, 80) → 50
- Entrada: LCA(60, 80) → 70

### Problema 5 — invertir()
Invierte el árbol en espejo intercambiando hijos izquierdo y derecho en todos los nodos.
- Antes:  InOrden: 10 20 30 40 50 60 70 80
- Después: InOrden: 80 70 60 50 40 30 20 10
