# Уравнение Кеплера

Этот репозиторий содержит решение задачи "21. Уравнение Кеплера" в рамках моей зачетной работы по дисциплине "Системы компьютерной математики".

## Описание задачи

### 21. Уравнение Кеплера
[Каханер–Моулер–Нэш]

*Уравнение Кеплера* для вычисления орбиты имеет вид

$$
    M=E-\varepsilon\sin E,
$$

где $M$ – средняя аномалия, $E$ – эксцентрическая аномалия, $\varepsilon$ – эксцентриситет орбиты.
Пусть $M=24.851090$, $\varepsilon=0.1$. 
  * Изобразите полученную орбиту.
  * С помощью функции `scipy.optimize.brentq` найдите $E$.
  * Вычислите $E$ с помощью формулы
  
  $$
    E = M + 2\sum_{m=1}^{\infty} \frac{1}{m} J_m(m\varepsilon) \sin(mM),
  $$
  
  где $J_m(x)$ – функция Бесселя $1$-го рода порядка $m$.
  * Найдите $E$ по предыдущей формуле, используя равенство
  
  $$
    J_m(m\varepsilon) = \sum_{n=0}^{\infty} \frac{(-1)^n (m\varepsilon/2)^{2n+m}}{n!(m+n)!}.
  $$

Проведите сравнение вычислительных затрат и точности результатов, полученных каждым из трех способов.

## Содержание репозитория

**kepler_equation_solution.ipynb**: Jupyter Notebook файл с решением задачи "21. Уравнение Кеплера". В нем представлен код на языке Python, который реализует различные методы решения уравнения Кеплера.
