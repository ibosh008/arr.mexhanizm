# arr.mexhanizm
## Callback

Callback — функсияе, ки ҳамчун аргумент ба method дода мешавад.

```js
array.method((item) => {});
```

---

# forEach()

## Барои чи

Массивро мегардад.



1. Ҳар элемент мегра мешавад
2. Callback иҷро мешавад
3. return надорад

```js
let arr = [1, 2, 3];

arr.forEach((item) => {
  console.log(item);
});
```

# map()


Массиви нав месозад.


1. Ҳар элемент ба callback меравад
2. Callback value-и нав медиҳад
3. Value-ҳо дар массиви нав чам  мешаван

```js
let arr = [1, 2, 3];

let result = arr.map((item) => {
  return item * 2;
});

console.log(result);
```

## Натиҷа

```js
[2, 4, 6]
```

## Дохилан

```js
let newArr = [];

for (let i = 0; i < arr.length; i++) {
  newArr.push(callback(arr[i]));
}
```

---

# filter()
Элементҳоро фильтр мекунад.
let

1. Ҳар элемент ба callback меравад
2. Агар true шавад → массиви нав
3. Агар false шавад → намедарояд

```js
let arr = [1, 2, 3, 4];

let result = arr.filter((item) => {
  return item > 2;
});

console.log(result);
```

## Натиҷа

```js
[3, 4]
```

---

# find()

Аввалин элементи мувофиқро меёбад.

1. Ҳар элемент санҷида мешавад
2. Агар true шавад
3. Ҳамон элемент return мешавад

```js
let arr = [5, 10, 15];

let result = arr.find((item) => {
  return item > 7;
});

console.log(result);
```

## Натиҷа

```js
10
```

---

# some()

Месанҷад, ки ягон элемент мувофиқ аст ё не


1. Ҳар элемент санҷида мешавад
2. Агар 1 true шавад
3. Дарҳол true медиҳад

```js
let arr = [1, 2, 3];

let result = arr.some((item) => {
  return item > 2;
});

console.log(result);
```

## Натиҷа

```js
true
```

---

# every()

Месанҷад, ки ҳамаи элементҳо мувофиқан АСТАН Ё Не

1. Ҳама элементҳо санҷида мешаванд
2. Агар ҳама true бошанд
3. true медиҳад

```js
дуе arr = [2, 4, 6];

дуе result = arr.every((item) => {
  return item % 2 === 0;
});

console.log(result);
```

## Натиҷа

```js
true
```

---

# reduce()


Ҳама элементҳоро ба 1 value табдил медиҳад


1. accumulator мегира
2. Ҳар element илова мешава
3. Дар охир 1 value мемо

```js
let arr = [1, 2, 3, 4];

let result = arr.reduce((a, b) => {
  return a + b;
}, 0);

console.log(result);
```

## Натиҷа

```js
10
```

---

# sort(

Массивро сортировка мекунад.


```js
const arr = [4, 1, 3, 2];

arr.sort((a, b) => {
  return a - b;
});

console.log(arr);
```

## Натиҷа

```js
[1, 2, 3, 4]
```

