# Распознавание образов

## **Цель работы:**

Обучить нейронную сеть Хопфилда распознавать образ.

## Задание для выполнения работы:

<aside>
💡 Задание: обучить нейронную сеть Хопфилда распознавать образ, вариант которой приведен в табл. 1.

</aside>

Предположим, мы имеем определённое количество начальных образов – изображений. Нам предлагают видоизменённый образ, и задача наша состоит в распознании одного из эталонных шаблонов.

В целом, для реализации вам понадобится две библиотеки – `matplotlib` и `numpy`.
1. Сначала необходимо сгенерировать матрицу с “эталонным” образом (размер матрицы от 4 до 14) согласно варианту, которая будет состоять из значений 1 и -1.  Таких матриц должно быть 3 штуки. Не делайте размеры матриц слишком большими. Рекомендуется использовать np.array().
2. Визуализировать эталонные изображения. Для визуализации двумерного массива чисел можно использовать imshow или plt.matshow().
3. Создать набор данных с шумами для тестирования. Для этого необходимо зашумить эталонные изображения, внеся в них в случайных местах – шум (изменить значение пикселя в случайных местах изображения). Вывести зашумлённые изображения. Описать процесс зашумления, при этом в алгоритме зашумления необходимо предусмотреть возможность использовать разный процент зашумления.
4. Выполнить обучение сети. Можно использовать библиотеку numpy и внешнее произведение векторов. В результате вычисляется матрица весовых коэффициентов.
5. Выполнить предсказание. Для проверки качества обучения модели подаются тестовые изображения (зашумлённые), которые умножаются на матрицу весовых коэффициентов и выполняется предсказание, то есть происходит распознавание образа.
6. Вывести эталонное изображение, зашумлённое изображение и предсказанное изображение и количество пикселей, которые были неверно распознаны (отличие предсказанного изображения от эталонного).
7. Вывести изображения, которые сеть не смогла распознать.
8. Вычислить ошибку восстановления – отношение несовпадений предсказанного результата с эталонным и несовпадений тестовой матрицы с эталонной.
9. Построить график зависимости ошибки восстановления от степени зашумления изображений.

## Вариант
Любые три дорожных знака
