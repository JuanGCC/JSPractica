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
La expresión `**switch**` evalúa una expresión, comparando el valor de esa expresión con una instancia `**case**`
</details>
</p>