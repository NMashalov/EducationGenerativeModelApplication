---
sidebar_position: 3
title: Награды
---

Награды могут иметь разное происхождение, предназначение и формы. Например, в российском школьном образовании отличная учеба награждается медалями, а физкультурно-спортивные достижения сопровождаются знаками отличия. Награды поощряют вовлеченную учебу и позволяют 

Известные компании, предоставляющие инструменты разработки, как [Github](https://github.com/) и [Google Сloud](https://cloud.google.com/), также используют систему знаков - *бэйджей* для поощрения пользователей ресурса к эффективному использованию ресурсов платформы и прохождению сертификации. Предполагается, что наличие таких наград может стать причиной для делового сотрудничества или предложения работы. Другим примером является платформа [Stack Overflow](https://stackoverflow.com/), на которой публикуются вопросы преимущественно технической тематики. Согласно ее правилам бейдж присваивается в случае наличие лучшего ответа на популярный вопрос. Такая награда поощряет положительную конкуренцию, поощряет к созданию конструктивных и этичных ответов.

## Исследование постановки

Аналитическим исследованием системы наград занимается направление Badge Design, изучающее постановки в котором принципал, распределяет бейджи среди участников.

:::note
 
    *Принципалы* и *агенты* - лица,совместно выполняющие работу. Предполагается, что принципал имеет задачу, которую ему нужно поручить агенту для решения. Теория изучает как различие в знаниях позволяют принципалу задать постановку таким образом, чтобы она была решена наиболее качественно.

:::

Для оценки пользы награды используются скалярные функции полезности $U$. Как правило, такие функции являются скрытыми от наблюдения. Для изучения исследователи закладывают предположения о ее виде. Например, считают что полезность монотонно возрастает с ростом награды. 

### Дизайн механизмов

Оптимальное распределение ресурсов в аналитических постановках изучается с помощью [дизайна механизмов](https://en.wikipedia.org/wiki/Mechanism_design). Современный подход был предложен и развит Леонидом Гурвичем в работе Optimality and Informational Efficiency in Resource Allocation Processes для эффективной организации рабочих процессов.

Подход заключается в определение допустимых действий игроков таким образом, чтобы максимизировать функцию полезность организатора. Строгое определение вводится через понятие байесовых игр с неполной информацией, предполагающих наличие нескольких шагов, направленных на формирование оптимальной стратегии. 

*Определение 1* **Байесова игра** это набор исходов $(N,O,\Theta)$ таких что,
- $\mathbf{N}$ конечное множество агентов $n$
- $O$ множество исходов
- $\Theta = \Theta_1 \times \Theta_2 \dots \Theta_n $ множество 
- $u = (u_1, \dots, u_N)$, где $u_i: O \times \Theta \rightarrow \mathrm{R}$  функция полезности для игрока $i$


*Определение 2* **Механизм** для байесовой игры это пара $(A,M)$, где

- $A = A_1 \times \dots \times A_n$ набор действий доступный агенту i
- $M: A \rightarrow \Pi(O)$ соединяет действия с распределением возможностей


*Определение 3* В заданной байесовой игре, механизм является **воплощением доминантной стартегии** социального выбора функции $C$, если для любого вектора полезности $u$ , у игры есть равновесие в доминантной стратегии, и для любого равновесия $a^*$ выполняется $M(a^*) = C(u)$


*Определение 4* В заданной байесовой игре, механизм является воплощением *Байес-Нэшевой доминантной стартегии* социального выбора функции $C$, если для любого вектора полезности $u$ , у игры есть равновесие в доминантной стратегии, и для любого равновесия $a^*$ выполняется $M(a^*) = C(u)$

:::tip

    Дизайн механизмов широко распространен в организации деятельности. Например, применяется для оптимальной организации расписания в аэропортах.

:::


## Дизайн 

Описаны ключевые свойства награды в линейно упорядоченной в виде.

### Уровни наград

Одним из направлений исследования ценности трофея 

Как правило награды в рамках одного направления упорядочены по значимости $m > \dots > 1 > 0$. Таким образом, участник мероприятия может сопоставить вклад своего участия.

### Статус

Определения адаптированы работы [SOCIAL STATUS AND BADGE DESIGN](https://arxiv.org/pdf/1312.2299).

Постановка изучает как распределить награды среди $n$ участников, внесших вклады $b \in \mathrm{R}$ в дело таким образом, чтобы $\sum_{i=1}^n b_i \rightarrow \max $ 


*Определение 1*. Механизмом Бейджа называется функция $r(b_i,b_{-i})$, определенная на множестве $$




### Создание и разрушение

Система наград имеет правила, по которым  они вручаются




:::tip 

    Ценность награды должна сохраняться с течением времени. Для этого необходимо подкреплять ее ценность.

:::
