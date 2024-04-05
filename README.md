# fp64-maria-cleancode

### He realizado esta kata https://www.codewars.com/kata/5239f06d20eeab9deb00049b

#### Las instrucciones del ejercicio:
The function 'fibonacci' should return an array of fibonacci numbers. The function takes a number as an argument to decide how many no. of elements to produce. If the argument is less than or equal to 0 then return empty array.

#### La solución que hice fue:
 
function fibonacci(number) {

  if (number <= 0) {
    return []
  }
  if (number === 1) {
    return [1]
  }
  const fibonacciSequence = [0, 1];
  for (let i = 2; i < number; i++) {
    fibonacciSequence.push(fibonacciSequence[i - 1] + fibonacciSequence[i - 2]);
  }
  return fibonacciSequence;
}

console.log(fibonacci(5));

#### Las reglas de clean code que he aplicado han sido:
##### El nombre de la función y el argumento ya estaban dados, así que lo que he hecho ha sido darle nombre a la variable const fibonacciSequence intentando que sea lo más descriptiva posible.
#### Al principio había hecho un else if y un else pero los he eliminado porque no eran necesarios.
#### He prestado mucha atención a la indentación.
