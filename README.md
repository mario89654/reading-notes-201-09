# Mitos y Verdades sobre el DOM y Expresiones Regulares

### 1. Usar `querySelector()` siempre devuelve una colección de nodos, incluso si selecciona uno solo.  
**Mito** – `querySelector()` solo devuelve el primer elemento que coincide con el selector, no una colección de nodos. Para obtener múltiples elementos, se usa `querySelectorAll()`.  

### 2. El DOM permite manipular estilos CSS directamente desde JavaScript usando propiedades específicas como `.style` y `.classList`.  
**Verdad** – El DOM permite manipular estilos CSS desde JavaScript mediante `.style` para modificar propiedades individuales y `.classList` para agregar o eliminar clases.  

### 3. Una expresión regular (Regex) siempre devolverá el mismo resultado sin importar el contexto o idioma del texto que analice.  
**Mito** – Las expresiones regulares pueden devolver resultados diferentes dependiendo del contexto, como el idioma, el conjunto de caracteres y las opciones de configuración (`i` para insensible a mayúsculas, `u` para compatibilidad con Unicode, etc.).  

### 4. Utilizar `querySelectorAll()` es menos eficiente que `getElementById` cuando se busca un único elemento por su ID.  
**Verdad** – `getElementById()` es más eficiente que `querySelectorAll()` para seleccionar un elemento por su ID, ya que `getElementById()` accede directamente al nodo sin necesidad de analizar selectores CSS.  

### 5. Todos los métodos del DOM devuelven elementos del mismo tipo, no existen diferencias entre ellos.  
**Mito** – Los métodos del DOM devuelven diferentes tipos de elementos; por ejemplo, `getElementById()` devuelve un único nodo, `querySelectorAll()` devuelve una `NodeList` estática, y `getElementsByClassName()` devuelve una `HTMLCollection` viva.  

### 6. `querySelectorAll()` permite seleccionar múltiples elementos y devuelve una lista estática (no viva) de nodos.  
**Verdad** – `querySelectorAll()` devuelve una `NodeList` estática, lo que significa que no se actualiza automáticamente si el DOM cambia después de la selección.  

### 7. Las expresiones regulares (Regex) se pueden utilizar para transformar contenido de texto (Markdown a HTML, por ejemplo) sin necesidad de librerías externas.  
**Verdad** – Las expresiones regulares pueden usarse para transformar texto, como convertir Markdown a HTML, aunque en casos complejos suele ser más eficiente usar librerías especializadas.  

### 8. Los cambios realizados en los nodos del DOM usando JavaScript son permanentes incluso después de refrescar la página.  
**Mito** – Los cambios en el DOM con JavaScript son temporales y desaparecen al recargar la página, a menos que se almacenen en `localStorage`, `sessionStorage` o una base de datos.  
