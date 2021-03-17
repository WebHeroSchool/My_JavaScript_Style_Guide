# JavaScript Style Guide
###### Здесь показаны некоторые правила по написанию кода в JavaScript. Эти правила носят рекомендательный характер для упрощения читабельности кода. Но при необходимости от правил можно отступать.

## 1. Используйте ключевые слова при объявлении переменной для каждой из них.
Плохо:
```javascript
let i = 0,
	b = 1,
    c = 2;

let a = 0, b = 1, c = 2;
```
Хорошо:
```javascript
let a = 0;
let b = 1;
let c = 2;
```

## 2. Используйте отступы табуляцией или двумя пробелами. Это упростит читабельность кода
Плохо:
```javascript
if (a < b) {
console.log(a);
}
```
Хорошо:
```javascript
if (a < b) {
  console.log(a);
}
```

## 3. Если имя переменной состоит из нескольких слов, используйте стиль camelCase
Плохо:
```javascript
const longlongname = 1;
```
Хорошо:
```javascript
const longLongName = 1;
```

## 4. Ставбте один пробел перед открывающейся фигурной скобкой у блока
Плохо:
```javascript
function getName(){
  console.log('Игорь');
}
```
Хорошо:
```javascript
function getName() {
  console.log('Игорь');
}
```

## 5. Разделяйте операторы пробелами
Плохо:
```javascript
const x=y+5;
```
Хорошо:
```javascript
const x = y + 5;
```

## 6. Не добавляйте пробелы между круглыми и квадратными скобками и их содержимым. Но добавляйте пробелы между фигурными скобками и их содержимым
Плохо:
```javascript
if ( a < b ) {
  console.log(a);
}

const foo = [ 1, 2, 3 ];
console.log(foo[ 0 ]);

const foo = {name: 'Игорь'};
```
Хорошо:
```javascript
if (a < b) {
  console.log(a);
}

const foo = [1, 2, 3];
console.log(foo[0]);

const foo = { name: 'Игорь' };
```

## 7. Не используйте в качестве названий переменных зарезервированные слова
Плохо:
```javascript
const let = 1;
let for = 2;
```
Хорошо:
```javascript
const variableOne = 1;
let variableTwo = 2;
```

## 8. В качестве названия переменной используйте понятное название, отражающее то, что лежит в переменной
Плохо:
```javascript
const a = 18;
let n = 'Игорь';
```
Хорошо:
```javascript
const userAge = 18;
let userName = 'Игорь';
```

## 9. Используйте шаблонные строки вместо конкатенации. Это позволяет сократить код
const userAge = 18;
let userName = 'Игорь';

Плохо:
```javascript
console.log('Имя ' + userName + ', возраст ' + userAge);
```
Хорошо:
```javascript
console.log(`Имя ${userName}, возраст ${userAge}`);
```

## 10. Для создания объекта используйте литеральную нотацию
Плохо:
```javascript
const user = new Object();
const user2 = new Array [];
```
Хорошо:
```javascript
const user = {};
const user2 = [];
```
