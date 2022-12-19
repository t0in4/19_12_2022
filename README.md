На домашний компьютер не забываем установить node.js скачав в поисковике
после установки уставливаем
в powershell
npm install promt-sync

Hello! My name is Aid.
I was created in 2022.
Please, remind me your name.
> Max
What a great name you have, Max!
Let me guess your age.
Enter remainders of dividing your age by 3, 5 and 7.
> 1
> 2
> 1
Your age is 22: that's a good time to start programming!
Now I will prove to you that I can count to any number you want.
> 3
0 !
1 !
2 !
3 !
Let's test your programming knowledge.
Why do we use methods?
1. To repeat a statement multiple times.
2. To decompose a program into several small subroutines.
3. To determine the execution time of a program.
4. To interrupt the execution of a program.
> 4
Please, try again.
> 2
Congratulations, have a nice day!

***
const input = require("prompt-sync")({ sigint: true });
function greet(a, b) {
  console.log(`Hello! My name is ${a}`);
  console.log(`I was created in ${b}`);
}

function remind_name() {
console.log("Please, remind me your name.");
let name = input();
console.log("What a great name you have, " + name + "!");
}


function guess_age() {
console.log("Let me guess your age.");
console.log("Enter remainders of dividing your age by 3, 5 and 7.");
let rem3 = Number(input());
let rem5 = Number(input());
let rem7 = Number(input());
let age = (rem3 * 70 + rem5 * 21 + rem7 * 15) % 105;
console.log("Your age is " + age + "; that's a good time to start programming!");
}

function count() {
console.log("Now I will prove to you that I can count to any number you want.");

let number = Number(input());
let current = 0;

while (current <= number) {
console.log(current + " !");
current += 1;
}


function test() {
// дописать код
}
function end() {
  console.log("Completed, have a nice day!");
}

greet('Aid', '2020') // change it as you need
remind_name();
guess_age();
count();
test();
end();
