# React Hooks
[Hooks](https://es.reactjs.org/docs/hooks-intro.html) son una nueva característica en React 16.8. Estos te permiten usar el estado y otras características de React sin escribir una clase.

## Reglas de los [Hooks](https://es.reactjs.org/docs/hooks-rules.html)

* No llames Hooks dentro de ciclos, condicionales o funciones anidadas

### Reducer Hook

**¿Qué es un reducer?**

* Es una función común y corriente.
* Debe de ser un función pura ( Todo lo que esta función realice se resulve de forma interna ).
* Debe de retornar un nuevo estado.
* Recibe 2 argumentos: el valor inicial (initialState) y la acción a ejecutar.

Función pura:

 * No debe de tener efectos secundaios. Debe de resolver la lógica de la función sin ayuda de otras funciones.
 * No debe de tener tareas asíncronas.
 * Debe de retornar siempre un estado nuevo.
 * No debe de llamar al _locaStorage_ o _sessionStorage_
 * No debe de requerir más de una acción, esta acción puede tener o no argumentos.

























