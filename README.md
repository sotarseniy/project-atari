# **Описание среды**
- В LostLuggage агент должен перемещаться в пространстве и находить потерянные багажи, выпавшие с самолёта.
- За каждый потерянный багаж агент теряет одну жизнь, всего жизней три.
- Цель агента - найти как можно больше багажей, избегая столкновений.

## **Действия**
- 0: NOOP (Ничего не делать)
- 1: UP (Вверх)
- 2: RIGHT (Вправо)
- 3: LEFT (Влево)
- 4: DOWN (Вниз)
- 5: UPRIGHT (Вверх-вправо)
- 6: UPLEFT (Вверх-влево)
- 7: DOWNRIGHT (Вниз-вправо)
- 8: DOWNLEFT (Вниз-влево)

## **Награды**

Один багаж - 3.

![lost-luggage](https://github.com/sotarseniy/project-atari-lost-luggage/blob/main/assets/lost_luggage.gif)

# **Алгоритмы**

## **Value Based**

Для реализации Value Based алгоритма можно реализовать Q-Learning алгоритм.

Q-Learning - алгоритм, обучающий агента принимать решения на значениях функции Q, представляющую собой ожидаемую награду за каждое действие action.

## **Policy Based (Policy Gradient)**

Алгоритм, который будет реализован, это REINFORCE (REward Increment = Nonnegative Factor * Offset Reinforcement * Characteristic Eligibility).

Алгоритм основан на принципе градиентного спуска и обновляет параметры стратегии агента таким образом, чтобы максимизировать накопление вознаграждения.