Scope это власть видимости
Global scope-это глобальная область видимости
Local scope бывает 2 видов
Function scope-это функциональная область видимости всё пишется внутри function является function scope
Block scope- это она работает внутри определенной области допустим for или if и тд .
Module scope- она нужно для того чтобы объединить две или более файла чтобы они имели доступ друг к другу.


Hosting это механизм который сначала вызываеш а потом создаёш цикл или просто вериэбл
Hosting работает в двух случаях в вериэбле var ответ которого будет underfine
Function declaration  ответ которого будет обычный то есть он просто покажет ответ функции но это считается hosting
 В остальных случаях покажет ошибку before iniziliator ,   ReferenceError  который в падает в мёртвую зону
Tdz  это мёртвая зона
TDZ (Temporal Dead Zone) — это промежуток времени в JavaScript, в течение которого переменная объявлена, но ещё не инициализирована
console.log(x); // ReferenceError: Cannot access 'x' before initialization
let x = 5;
console.log(a); // undefined (var инициализируется как undefined)
var a = 1;

console.log(b); // ReferenceError
let b = 2;

console.log(c); // ReferenceError
const c = 3;
function example() {
  console.log(foo); // ReferenceError: Cannot access 'foo' before initialization
  let foo = "Hello";
}
example();
TDZ помогает избегать ошибок, связанных с доступом к переменным до их инициализации, что делает код более предсказуемым и надёжным
