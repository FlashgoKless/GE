Все задания по вебу выполняются в одном файле, стили приписываем в тэге style в шапке 

* [Базовая структура](#1)
* [Задание 1](#2)
* [Задание 2](#3)


# <a id='1'>Базовая структура</a> 
1) Что бы создать базовую структуру страницы, ставим ! и тыкаем enter
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

↑ вот что должно получиться

2) Далее под основное тело html (под тэг body) кидаем тэг style

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    
</head>
<body>
    
</body>
<style></style> ← вот он
</html>
```

# <a id='2'>Задание 1</a>
Необходимо сделать так, чтобы только элементы «Пункт 2» и «Пункт 3» были красными, 
и с нижними отступами между элементами. А вокруг списка должна быть пунктирная рамка (цвет: blueviolet) 
с кругленными краями (dashed)

![alt text](image.png)

```
<!DOCTYPE html>
<body>
  	<ul>
        <li>Пункт 1</li>
        <li>Пункт 2</li>
        <li>Пункт 3</li>
        <li>Пункт 4</li>
      </ul>
</body>
<style>
li {
  color: black;
}
</style>
```

В задании дана базовая структура. у нас есть неупорядоченный список (ul).  
Первое, что нужно сделать - проставим классы на теги li, что бы разделить красные элементы и черные, и класс на тэг ul, чтобы было)   
Пусть черные будут point, а красные - colored_point.  
Так же добавим в тэг style три класса: вместо li - li.colored_point и li.point, и ul.list. Можно написать просто .point, .colored_point и .list, разницы никакой.  

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <ul class="list">
            <li class="point">Пункт 1</li>   ← изменение
            <li class="colored_point">Пункт 2</li>   ← изменение
            <li class="point">Пункт 3</li>   ← изменение
            <li class="colored_point">Пункт 4</li>   ← изменение
        </ul>
    </body>
    <style>
        li.point{  ← изменение
        }
        li.colored_point{  ← изменение
        }
        ul.list{  ← изменение
        }
    </style>
</html>
```
<img src="image-1.png" alt="image-1" width="450"/>

Коротко об отступах  
у каждого элемента есть рамка - border, мы можем задать ей размер, цвет и другие параметры. пространство за пределами рамки - margin. пространство внутри рамки - padding. соотвественно у каждого из этих параметров есть верх, низ, право и лево (top, bottom, right, left). прим.: margin-top: 2 px - верхний внешний отступ 2 px от другого элемента  


Накинем цвет и нижние отступы между элементами на li и рамку на list в стили
```
    <style>
        li.point{
            color: black;
            margin-bottom: 4px
        }
        li.colored_point{
            color: red;
            margin-bottom: 4px
        }
        ul.list{
            border: 2px dashed blueviolet; 
            <!-- dashed - прерывистая рамка -->
            border-radius: 8px;
        }
    </style>
```

можно еще сделать вот так
```
    <style>
        li{
            margin-bottom: 10px;  
        }
        li.point{
            color: black;
        }
        li.colored_point{
            color: red;
        }
        .list{
            border: 2px dashed blueviolet;
            border-radius: 8px;
        }
    </style>
```

