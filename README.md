# **Описание среды**
- В LostLuggage агент должен перемещаться в пространстве и находить потерянные багажи, выпавшие с самолёта.
- За каждый потерянный багаж агент теряет одну жизнь, всего жизней три.
- Цель агента - найти как можно больше багажей, избегая столкновений.
![](https://github.com/sotarseniy/project-atari-lost-luggage/tree/main/assets/lost_luggage.gif)

## **Действия**
- 0: NOOP
- 1: UP
- 2: RIGHT
- 3: LEFT
- 4: DOWN
- 5: UPRIGHT
- 6: UPLEFT
- 7: DOWNRIGHT
- 8: DOWNLEFT

## **Награды**

Один багаж - 3.

# **Алгоритмы**

## **Value Based**

Для реализации Value Based алгоритма можно реализовать Q-Learning алгоритм.

Q-Learning - алгоритм, обучающий агента принимать решения на значениях функции Q, представляющую собой ожидаемую награду за каждое действие action.

## **Policy Based (Policy Gradient)**

Алгоритм, который будет реализован, это REINFORCE (REward Increment = Nonnegative Factor * Offset Reinforcement * Characteristic Eligibility).

Алгоритм основан на принципе градиентного спуска и обновляет параметры стратегии агента таким образом, чтобы максимизировать накопление вознаграждения.