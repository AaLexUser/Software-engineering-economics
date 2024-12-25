# ЭПИ

- [Лабораторная работа 1](Lab1/Lab1_Юнусов_Лапин.pdf)
- [Лабораторная работа 2](Lab2/Lab2_Юнусов_Лапин.pdf)
- [Лабораторная работа 3](Lab3/Lab3_Юнусов_Лапин.pdf)

## Рубежка (По вопросам от Redgry)

> Мы решили произвести товар стоимость которого составляет 300к, система налогообложения общая у нас. Мы используем 2 компании для производства нашего товара. В одной 72к траты без НДС, во второй 48к с НДС. Сколько мы должны уплатить НДС за наш товар?

<details>
    <summary>Решение</summary>

Для расчёта НДС, который необходимо уплатить при продаже товара стоимостью 300 000 рублей на общей системе налогообложения, нужно учитывать как исходящий НДС (от продаж), так и входящий НДС (от расходов).

**Шаг 1: Определение исходящего НДС (от продажи)**

- **Продажная цена без НДС**: 300 000 рублей
- **Ставка НДС**: 20%
- **Исходящий НДС**: 300 000 × 20% = 60 000 рублей

**Шаг 2: Определение входящего НДС (от расходов)**

1. **Первая компания**:
   - **Расходы без НДС**: 72 000 рублей
   - **Входящий НДС**: 0 рублей (так как расходы без НДС)

2. **Вторая компания**:
   - **Расходы с НДС**: 48 000 рублей
   - **НДС включен в стоимость**: 
     - **База без НДС**: 48 000 ÷ 1.20 = 40 000 рублей
     - **Входящий НДС**: 48 000 - 40 000 = 8 000 рублей

- **Итого входящий НДС**: 0 + 8 000 = 8 000 рублей

**Шаг 3: Расчёт НДС к уплате**

- **НДС к уплате** = **Исходящий НДС** - **Входящий НДС** = 60 000 - 8 000 = **52 000 рублей**

### Ответ

$\fbox{52 000 рублей}$
</details>

> Трудоемкость разработки ПО составляет 300 попугаев в бэклоге. За спринт разработчики отрабатывают 50 попугаев. После первого спринта в бэклог было добавлено 20 попугаев, второго 40, третьего 70, а затем в каждый следующий спринт добавлялось по 10 попугаев. За сколько спринтов, в соответствии с улучшенной диаграммой сгорания, будет разработано ПО?

<details>
    <summary>Решение</summary>

Чтобы определить, за сколько спринтов будет разработано ПО с учетом добавления новых попугаев в бэклог после каждого спринта, рассмотрим процесс пошагово.

### Исходные данные

- **Начальный бэклог:** 300 попугаев
- **Скорость разработки:** 50 попугаев за спринт
- **Добавления в бэклог:**
  - После 1-го спринта: +20 попугаев
  - После 2-го спринта: +40 попугаев
  - После 3-го спринта: +70 попугаев
  - Начиная с 4-го спринта и далее: +10 попугаев после каждого спринта

### Пошаговый расчет

| Спринт | Начальный бэклог | Разработано | Остаток до добавления | Добавлено | Итоговый бэклог |
|--------|-------------------|-------------|------------------------|-----------|------------------|
| 1      | 300               | 50          | 250                    | +20       | 270              |
| 2      | 270               | 50          | 220                    | +40       | 260              |
| 3      | 260               | 50          | 210                    | +70       | 280              |
| 4      | 280               | 50          | 230                    | +10       | 240              |
| 5      | 240               | 50          | 190                    | +10       | 200              |
| 6      | 200               | 50          | 150                    | +10       | 160              |
| 7      | 160               | 50          | 110                    | +10       | 120              |
| 8      | 120               | 50          | 70                     | +10       | 80               |
| 9      | 80                | 50          | 30                     | +10       | 40               |
| 10     | 40                | 40          | 0                      | —         | 0                |

### Подробное объяснение

1. **Спринты 1-3:** На начальных этапах добавление попугаев увеличается значительными плюсами (20, 40, 70 попугаев соответственно).
2. **Спринты 4 и далее:** Добавление стабилизируется на уровне 10 попугаев за спринт.
3. **Итого:** К 10-му спринту весь бэклог будет успешно отработан, и ПО будет завершено.

### Ответ

$\fbox{10 спринтов}$

</details>
---

> Дана таблица со значениями.
Необходимо посчитать по методу PERT $E_{95\%}$

| Параметр   | Оптимистичное (O) | Пессимистичное (P) | Наиболее вероятное (M) |  
|------------|--------------------|---------------------|------------------------|
| **E1**     | 24                | 40                 | 24                    |
| **E2**     | 16                | 40                 | 12                    |
| **E3**     | 16                | 44                 | 14                    |

<details>
    <summary>Решение</summary>

---
$E_1 = \frac{24+40+4\cdot 24}{6}= \frac{80}{3}$

$E_2 = \frac{16+40+4\cdot 12}{6}= \frac{52}{3}$

$E_3 = \frac{16+44+4\cdot 14}{6}= \frac{58}{3}$

$E = \frac{80}{3} + \frac{52}{3} + \frac{58}{3} = \frac{190}{3}$

---
$СКО_1 = \frac{40-24}{6}=\frac{8}{3}$

$СКО_2 = \frac{40-16}{6}=4$

$СКО_3 = \frac{44-16}{6}=\frac{14}{3}$

$СКО = \sqrt{СКО_1^2 + СКО_2^2 + СКО_3^2} = \frac{2\sqrt{101}}{3}$

---

$E_{95\%} = E + 2\cdot СКО = \frac{190}{3} + 2\cdot \frac{2\sqrt{101}}{3} = 76.73$

### Ответ

$\fbox{77}$
</details>

---

> • Между Сторонами заключен договор, где Исполнитель обязан изготовить ПО, стоимость которого составляет `1 000 000 руб`. Заказчик заплатил задаток `200 000 руб`.

> • Договор может быть расторгнут за неисполнение любой из Сторон существенных условий Договора, если просрочка разработки ПО Исполнителем составило `20` и более календарных дней с возвратом обеспечительных обязательств.

> • В штрафных санкциях по договору за неисполнение обязательств Исполнителем предусмотрено пени за просрочку сдачи ПО за каждый календарный день просрочки на `0.5%` от суммы договора, но не более `10%` от суммы договора.

> • Расторжение договора не избавляет стороны от уплаты штрафов.

> • Какую сумму должен выплатить Исполнитель Заказчику, если Заказчик расторгает договор за неисполнение Исполнителя после `30 дня` просрочки обязательств?

<details>
    <summary>Решение</summary>
Разберёмся по шагам:

1) Базовая сумма договора: 1 000 000 руб.  
2) Задаток (или иное обеспечительное обязательство), уплаченный Заказчиком Исполнителю: 200 000 руб.  
3) Штрафные санкции по договору: 0,5 % в день от суммы договора за просрочку, но не более 10 % от суммы всего договора.  
   • 0,5 % от 1 000 000 руб. = 5 000 руб. в день  
   • За 30 дней просрочки «чистая» неустойка составила бы 30 × 5 000 = 150 000 руб.,  
     однако по условию договора максимум — 10 %, то есть 100 000 руб.  
4) Возможность расторжения при просрочке ≥ 20 дней с возвратом обеспечительных обязательств означает, что Исполнитель обязан вернуть задаток (200 000 руб.) и уплатить начисленную неустойку (100 000 руб.).  
5) Итого Исполнитель должен выплатить Заказчику:  
   $200 000 руб$. (возврат задатка)  
   $+ 100 000 руб$. (штраф за просрочку, ограниченный 10 %)  
   $= 300 000 руб$.
### Ответ

$\fbox{300 000 руб}$
</details>

> Зарплата после всех налогов `40002 руб`. Налог на Фонды = `28.5%`. Необходимо было посчитать сколько было изначально (с налогами).

<details>
    <summary>Решение</summary>

<details>
    <summary>Подробно:</summary>
Шаг 1. Определяем «грязную» заработную плату (базу для НДФЛ)
Чистая зарплата = 40002 руб

Чистая зарплата = Грязная зарплата × (1 – 13%)

40 002 = Грязная зарплата × 0,87

Отсюда
Грязная зарплата = 40 002 / 0,87 ≈ 45 979,31 руб.

Шаг 2. Рассчитываем страховые взносы (28.5% от «грязной»)

Взносы в фонды = 45 979,31 × 0,285 ≈ 13104,10 руб.

Грязная зарплата + Взносы в фонды = 45 979,3 + 13104,10 ≈ 59083,41 руб

Шаг 3. Рассчитываем НДС (20%)

НДС = 59083,41 × 0,2 ≈ 11816,68 руб

Итого:

Грязная зарплата + Взносы в фонды + НДС = 59083,41 + 11816,68 ≈ 70900 руб
</details>
<details>
    <summary>Коротко:</summary>
Изначально = (40002 / 0,87) × 1.285 × 1.2 = 70900 руб
</details>
### Ответ

$\fbox{70900 руб}$
</details>