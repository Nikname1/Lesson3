# Lesson3
<p>Домашнее задание Урок №3( Домашнее задание №2)</p>
1)Даны натуральные числа от 20 до 50.Напечатать те из них, которые делятся на 3, но не делятся на 5.
Решение
<?php
if($i=1,$i<101,$i++){
console.log($i);
}
Si = 1;
while ($i < 101) {
console.log($i);
$i++;
}
?>
2)С помощью цикла while() напишите скрипт вывода всех четных чисел в диапазоне от 2 до 100 включительно.
Решение:
<?php
//while
$x = 2;
while ($x<100){
echo "$x<br>";
$x+=2;
}
?>
3)Сделать программу, выводящую факториал числа (произведение чисел от 1 одного до n), где n любое число больше 1.
Решение
<?php
function factorial($n)
{
if ($n== 0){
return 1;
} else {
return $n* factorial($n-1);
}
}
for ($n=0; $n<=1; $n++){
echo($n. "! = " . factorial($n) . "\n");
}                            
?>
4) Числа Фибоначчи.(Кролики)
<?php
function fibonacci($n)
{
    if($n < 2) {
        yield $n;
    }
    $x = fibonacci($n-1);
    $y = fibonacci($n-2);
    yield $x->current() + $y->current();
}
for($i = 0; $i <= 10; $i++) {
    $x = fibonacci($i);
    $value = $x->current();
    echo $i , ' -> ' , $value, PHP_EOL;
}
?>
