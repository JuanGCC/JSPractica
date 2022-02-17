# Java Script
<details><summary>Tipos de datos y tipos de Operadores</summary>
<p>

### Tipos de datos
- Number
- String
- Boolean
- Array
- Null
- Undefined
<!--<h3> Tipos de datos</h3>-->


  <table>
      <thead>
        <tr>
          <th scope="row" colspan="5">Operadores aritméticos</th>
        </tr>
        <tr>
          <th>Operador</th>
          <th>Descripción</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>=</td>
          <td>Operador de Asignación</td>
        </tr>
        <tr>
          <td>+</td>
          <td>Operador de suma <br> Se usa para sumar dos o más numeros, o juntar dos cadenas en una</td>
        </tr>
        <tr>
          <td>-, *, /</td>
          <td>Hacen lo mismo que en las matemáticas básicas</td>
        </tr>
        <tr>
          <td>==</td>
          <td>Operador de igualdad</td>
        </tr>
        <tr>
          <td>===</td>
          <td>Comprueba si dos valores son iguales entre sí, y devuelve un valor de true/false (booleano)<br> 
          Tambien conocido como operador de igualdad estricta</td>
        </tr>
        <tr>
          <td>!, !==, !=</td>
          <td>El primero niega una comparación, ejemplo: <br> let variable = 3; <br> !variable === 3 <br> 
          El segundo comprobamos estrictamente si el valor no es igual a X cosa, ejemplo: <br>variable = 3; <br> variable !== 3;
          <br>El tercero es parecido al segundo, pero no es tan estricto</td>
        </tr>
        <tr>
          <td>A++</td>
          <td>Incrementa una cantidad posterior a su ejecución</td>
        </tr>
        <tr>
          <td>++A</td>
          <td>Incrementa una cantidad anterior a su ejecución</td>
        </tr>
        <tr>
          <td>--A</td>
          <td>Decrementa una cantidad anterior a su ejecución</td>
        </tr>
        <tr>
          <td>A--</td>
          <td>Incrementa una cantidad posterior a su ejecución</td>
        </tr>
        <tr>
          <td>%</td>
          <td>Operador de residuo</td>
        </tr>
        <tr>
          <td>A**B</td>
          <td>Operador de exponenciación</td>
        </tr>
      </tbody>
      <thead>
        <tr>
          <th scope="row" colspan="5">Operadores Relacionales</th>
        <tr>
      </thead>
      <tbody>
        <tr>
          <td><</td>
          <td>Operador menor que</td>
        </tr>
        <tr>
          <td>></td>
          <td>Operador mayor que</td>
        </tr>
        <tr>
          <td><=</td>
          <td>Operador menor o igual a</td>
        </tr>
        <tr>
          <td>>=</td>
          <td>Operador mayor o igual a</td>
        </tr>
      </tbody>
      <thead>
        <tr>
          <th scope="row" colspan="5">Operadores Lógicos</th>
        <tr>
      </thead>
      <tbody>
        <tr>
          <td>&&</td>
          <td>AND lógico</td>
        </tr>
        <tr>
          <td>||</td>
          <td>OR lógico</td>
        </tr>
      </tbody>
      <thead>
        <tr>
          <th scope="row" colspan="5">Operador Ternario</th>
        <tr>
      </thead>
      <tbody>
        <tr>
          <td>(condición ? ifTrue : ifFalse)</td>
          <td>El operador condicional devuelve uno de dos valores según el valor lógico de la condición</td>
        </tr>
      </tbody>
      <thead>
        <tr>
          <th scope="row" colspan="5">Operadores de Asignación</th>
        <tr>
      </thead>
      <tbody>
        <tr>
          <td>*=</td>
          <td>Asignación de multiplicación</td>
        </tr>
        <tr>
          <td>/=</td>
          <td>Asignación de divición</td>
        </tr>
        <tr>
          <td>%=</td>
          <td>Asignación de residuo</td>
        </tr>
        <tr>
          <td>+=</td>
          <td>Asignación de suma</td>
        </tr>
        <tr>
          <td>-=</td>
          <td>Asignación de sustracción</td>
        </tr>
      </tbody>
      <thead>
        <tr>
          <th scope="row" colspan="5">Tipos de Strings</th>
        <tr>
      </thead>
      <tbody>
        <tr>
          <td>"", '' </td>
          <td>Permite ingresar una cadena de texto</td>
        </tr>
        <tr>
          <td>``</td>
          <td>Permite ingresar una cadena de texto y variables mediante: `${variable}` y son llamados Template String</td>
        </tr>
      </tbody>
  </table>
</details>
  </p>
<!--
**Siguiente paso**
- [Condicionales y ciclos](./CondicionalesYciclos.md) -->


<details><summary>Condicionales</summary>
<p>

### Condicional If
La condición if evalua si la condición evaluada es verdadera o falsa y su sintaxis es:
```javascript
  if(Condicion){
    // True
  }else{
    // False
  }
```
Tambien se pueden anidar multiples sentencias if
```javascript
  if(Condicion1)}{
    // Acción1
  }else if(Condicion2){
    // Acción2
  }else if(Condicion3){
    // Acción3
  }
  ...
  else{
    //AcciónN
  }
```
Dentro de las sentencias if deben ir operadores lógicos, relacionales.... (previamente visto en el apartado `Tipos de datos y tipos de Operadores`)
Ejemplo:
```javascript
  let edad = 18
  if(edad >= 18){
    console.log("Eres mayor de edad!");
  }else{
    console.log("Eres menor de edad");
  }
```

### Condicional multiple (Switch)
La expresión **`switch`** evalúa una expresión, comparando el valor de esa expresión con una instancia **`case`**
y ejecuta declaraciones asociadas a ese **`case`**, así como las declaraciones en los **`case`** que siguen.
##### Sintaxis 
```javascript
switch (expresión) {
  case valor1:
    //Declaraciones ejecutadas cuando el resultado de expresión coincide con el valor1
    break;
  case valor2:
    //Declaraciones ejecutadas cuando el resultado de expresión coincide con el valor2
    break;
  ...
  case valorN:
    //Declaraciones ejecutadas cuando el resultado de expresión coincide con valorN
    break;
  default:
    //Declaraciones ejecutadas cuando ninguno de los valores coincide con el valor de la expresión
    break;
}
```
**Nota**: La declaración **`break`** es opcional y está asociada con cada etiqueta de case y asegura que el programa salga del switch una vez que se ejecute la instrucción coincidente y continúe la ejecución en la instrucción siguiente. Si se omite el  break  el programa continúa la ejecución en la siguiente instrucción en la declaración de **`switch`** .
##### Operación única con múltiples casos
Este es un ejemplo de operación única con sentencia switch secuencial, donde cuatro valores diferentes se comportan exactamente de la misma manera:
```javascript
var Animal = 'Jirafa';
switch (Animal) {
  case 'Vaca':
  case 'Jirafa':
  case 'Perro':
  case 'Cerdo':
    console.log('Este animal subirá al Arca de Noé.');
    break;
  case 'Dinosaurio':
  default:
    console.log('Este animal no lo hará.');
}
```
</details>
</p>

<details><summary>Ciclos</summary>
<p>

### Ciclo for
 Crea un bucle que consiste en tres expresiones opcionales, encerradas en paréntesis y separadas por puntos y comas, seguidas de una sentencia ejecutada en un bucle.
 ```javascript
 for (var i = 0; i < 9; i++) {
   n += i;
   mifuncion(n);
}
 ```
### Ciclo for...in
La instrucción **`for...in`** itera una variable especificada sobre todas las propiedades enumerables de un objeto. Para cada propiedad distinta, JavaScript ejecuta las instrucciones especificadas. Una declaración for...in tiene el siguiente aspecto:
```javascript
function dump_props(obj, obj_name) {
  let result = '';
  for (let i in obj) {
    result += obj_name + '.' + i + ' = ' + obj[i] + '<br>';
  }
  result += '<hr>';
  return result;
}
```
### Ciclo for...of
La declaración **`for...of`** crea un bucle que se repite sobre objetos iterables (incluidos Array, Map, Set, objetos arguments y así sucesivamente), invocando un bucle de iteración personalizado con declaraciones que se ejecutarán para el valor de cada distinta propiedad.

El siguiente ejemplo muestra la diferencia entre un bucle **`for...of`** y un bucle **`for...in`**. Mientras que **`for...in`** itera sobre los nombres de propiedad, **`for...of`** itera sobre los valores de propiedad:
```javascript
const arr = [3, 5, 7];
arr.foo = 'hola';

for (let i in arr) {
   console.log(i); // logs "0", "1", "2", "foo"
}

for (let i of arr) {
   console.log(i); // logs 3, 5, 7
}
```
### Ciclo while
Es muy parecido al ciclo for
El siguiente bucle while itera mientras n es menor que tres.
```javascript
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```
###  Ciclo Do While
En el siguiente ejemplo, el bucle **`do`** itera al menos una vez y se repite hasta que i ya no sea menor que 5.
```javascript
let i = 0; 
do { 
  i += 1; console.log(i); 
  } 
while (i < 5);
```
</details>
</p>
