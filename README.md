##Ruby — це інтерпретована, повністю об'єктно-орієнтована мова програмування,
Мова відрізняється високою ефективністю розробки програм і увібрала в себе кращі риси Perl, Java, Python, Smalltalk, Eiffel, Ada і Lisp.
Мова була створена Юкіхіро Мацумото, котрий почав працювати над Ruby 24 лютого 1993 року. 
Метою було створення об'єктно-орієнтованої, легкої в розробці, інтерпретованої мови програмування. 
Перша загальнодоступна версія 0.95 побачила світ 1995 року. «Ruby» був названий так  через жарт, що ходив у колі друзів Мацумото, і був алюзією до назви мови програмування Perl (перлина)

##RVM — Ruby Version Manager 
Програма для управління версіями Ruby.
rvm list - список версій рубі
rvm install ruby 2.2.3
rvm use ruby-2.2.1
rvm use ruby 1.9.2 --default

Як бути якщо один проект використовує Рубі 1.8.7, а інший 1.9.2? А що якщо при цьому у вас 2 проекти під версією 1.9.2, але з різними наборами гемов? 
Хотілося б вам мати окремі набори gem's для кожного проекту?

gem — пакет(файл) с библиотекой или приложением. Имеет стандартизированный вид и расположен в хранилище в сети.
https://rubygems.org/gems

gem install devise

Идеология Ruby:
• люди отличаются друг от друга, поэтому существует несколько способов
решения одной задачи. Каждый выбирает тот способ, который ему по душе;
• опытные программисты не должны сталкиваться с неожиданным поведе-
нием своих программ (принцип наименьшего удивления);
• программирование должно приносить удовольствие. Все рутинные дей-
ствия должны выполняться компьютером.
• Програмісти ліниві)
 1. Не дублюй код (DRY - don't repeat yourself)
 2. KISS (англ. keep it simple, stupid — «не ускладнюй, дурню» або більш ввічливий варіант англ. keep it short and simple — «роби коротше і простіше»)
 3. Не зроби велосипеда.
 • Рубісти щедрі, вони люблють ділитися своїм кодом і готовими рішеннями
 
 
##Типи Даних
Fixnum (целые числа, меньшие 2^{30}),
Bignum (целые числа, большие 2^{30}),
Float (числа с плавающей запятой),
nil
Array (массивы),
String (строки),
Symbols
Hash (ассоциативные массивы).
Диапазоны (Range)


Змінні Ruby містять не самі об'єкти, а посилання на них. Присвоєння — це не передача значення, а копіювання посилання на об'єкти.  Наприклад:
```
a = "abcdefg"   =>   "abcdefg"
b = a           =>   "abcdefg"
b               =>   "abcdefg"
a[3] = 'R'      =>   "R"
b               =>   "abcRefg"
```

##Методи
```
def name(variable)
  puts variable
end

To call a methods

name variable
or
name(variable)

def hi
 puts "Hello World!"
end

hi
```
##Цикл

```
for i in 1...10
   print i, " Hello\n";
end 
```

##Conditional statements
```
if cond
  # code to do
end
///////////

if cond
   puts "x is 2"
else
   puts "I can't guess the number"
end


unless cond
  # code to do
end

age = 3
case $age
when 0 .. 2
  puts "baby"
when 3 .. 6
  puts "little child"
when 7 .. 12
  puts "child"
when 13 .. 18
  puts "youth"
else
  puts "adult"
end
```