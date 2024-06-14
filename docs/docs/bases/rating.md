---
sidebar_position: 2
title: 'Системы рейтинга'
---

Рейтинг системы широко распространены в спортивных, киберспортивных и интеллектуальных соревнованиях. Они используются для подбора соперников по уровню. Как правило это означает, что

Согласно строгой постановке модели рейтинга нужны для линейного упорядочивания ряда объектов, которые можно сравнить только попарно.

Содержательный обзор темы представлен в формате презентации научного сотрудника института имени Стеклова Сергея Николенко об адаптации системы командного рейтинга TrueSkill к турниру "Что? Где? Когда?" в двух частях:
- постановка 
- [решение](https://logic.pdmi.ras.ru/~sergey/slides/NS11_ICMLtalk.pdf

<img class="img-center" src='/img/rating.excalidraw.png'/>

## Эло

Рейтинг Эло - подход к расчету силы игроков, основанный на предсказательной силе

:::tip

    Модель названа в автора физика и шахматиста Арпадом Эло. Эло адаптировал систему 

:::

Использование Эло в образовании
- [Applications of the Elo Rating System in Adaptive Educational Systems](https://www.fi.muni.cz/~xpelanek/publications/CAE-elo.pdf) - использование в [адаптационном подходе](/bases/test) в образовании. 
- [](https://aclanthology.org/W19-4451.pdf)


### Теоретическое описание

Рейтинг строится по принципу потенциала. Нулевой уровень задается произвольно. Вероятность победы задается через разницу уровней игроков, считающимися явно необозримыми переменыыми:

$$
    P(R_{ij}=1) = \frac{1}{1 + e^{-(\theta_i - \theta_j)}}
$$

, где $\theta_i$ - задает рейтинга участника. Подход к оценки совпадает с подходом Item Response Theory случайности совпадает с IRT[/bases/test]. 


:::note
    
    В литературе также популярна модель Брэдли-Терри.
    $$
        P(\theta)
    $$

    Заметим, что подмена $\gamma ~ exp(-\theta/\beta^2)$ позволяет отождествить подходы.

:::


### Практическое применение

В шахматной практике волатильность считается определенной и имеет стандартное отклонение равное 20:

$$
    \frac{1}{1+10^\frac{R_B-R_A}{400}}
$$

:::tip

    Экспоненциальный вид графика связан с предположением о том, что в стратегических играх существенное различие в навыке гарантирует победу

:::

По окончанию соревнования рейтинг каждого игрока обновляется

Обновление рейтинга выполняется по правилу

$$
    R^'_A = R_A
$$


Таким образом, в каждой игре.

### Примечательные свойство Эло


1. В отсутствии роста игрока его уровень не будет изменяться.

$$
    E_p(\theta) = p 
$$


2. Новый рейтинг задается 
 
```tip

    В модели Эло новый рейтинг

```


3.



## Система Глико

Модель Глико при присваивании балла также учитывает. http://www.glicko.net/glicko/glicko.pdf

:::note

    Модель Глико популярна в онлайн играх, поскольку пользователи могут играть нерегулярно

:::

Вводится переменная $RD$ отвечающая за волатильность.

$$
    
$$


##

$$

$$