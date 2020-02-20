# MSU
описание тем исследовательских работ для студентов

### кодирование категориальных признаков
исследование различных спомобов кодирования категорий (отнестись к этому, как к простейшей реализации стекинга)
* http://contrib.scikit-learn.org/categorical-encoding/
* https://www.kaggle.com/mlisovyi/9-ways-to-treat-categorical-features-updated#
* https://www.kaggle.com/ogrellier/python-target-encoding-for-categorical-features#
* https://www.kaggle.com/vprokopev/mean-likelihood-encodings-a-comprehensive-study#
* https://github.com/DenisVorotyntsev/CategoricalEncodingBenchmark
*  Дьяконов А.Г. [Методы решения задач классификации с категориальными признаками](https://istina.msu.ru/download/9065306/1iEWo3:1Ms-LUCOUScMLKN_B5hxIE-38tE/) // Прикладная математика и информатика. Труды факультета Вычислительной математики и кибернетики МГУ имени М.В. Ломоносова 2014, № 46, с. 103-127.


### метрические алгоритмы / эффективные методы поиска ближайших соседей
* материалы из лекции
* сделать аналогичные эксперименты / критику работы (есть журнальный вариант) https://arxiv.org/abs/1708.04321

### случайные леса
* kernel + RF https://arxiv.org/pdf/1502.03836.pdf (ещё много чего есть). Если поискать, то
* * https://arxiv.org/pdf/1402.4293.pdf (тут ядра как в АПкРО)
* сравнение с Extra-Trees https://stats.stackexchange.com/questions/175523/difference-between-random-forest-and-extremely-randomized-trees
* просто взять все совр. реализации, хорошие реальные/модельные задачи + эксперименты/графики!

### важности признаков
* что быстее сходится (в RF, например) качество или важность
* (done) Strobl C., Boulesteix A.-L., Zeileis A., Hothorn T. Bias in random forest variable importance measures (2007). BMC Bioinformatics, 8(1), 25.

*Здесь отмечается смещение важностей в сторону признаков с большим числом категорий или масштаба. Для некоторых моделей  -зависимость от способа сэмплинга (с возвратом или без).*

* van der Laan MJ (2006) Statistical inference for variable importance. Int J Biostat. https://doi.org/10.2202/
1557-4679.1008

*(вроде) поправка идёй Бреймана*

* Gregorutti B, Michel B, Saint-Pierre P (2015) Grouped variable importance with random forests and application to multiple functional data analysis. Comput Stat Data Anal 90:15–35
* Gregorutti B, Michel B, Saint-Pierre P (2017) Correlation and variable importance in random forests. Stat
Comput 27(3):659–678

*(вроде) теория Бреймана для регрессий*

### оптимизация гиперпараметров
сделать обзор существующих методов / предложить быстрые (не обязательно для настройки ML-алгоритмов)
* Байесовский подход: [отсюда](https://github.com/WillKoehrsen/hyperparameter-optimization/blob/master/Introduction%20to%20Bayesian%20Optimization%20with%20Hyperopt.ipynb) ходить по ссылкам
* много современных исследований: https://sigopt.com/research
* хорошая обзорная работа https://app.sigopt.com/static/pdf/SigOpt_Bayesian_Optimization_Primer.pdf

### аугментация
в принципе, выигрышная тема
* для звука https://arxiv.org/pdf/1904.08779.pdf

### развитие ядерных методов
Если сделать по уму - они немного проигрывают DL:
* одна из последних классных реализаций https://arxiv.org/pdf/1705.10958.pdf

### весовые схемы, оценка меняющихся вероятностей
Решить задачу оценки вероятности p(t), сравнить метод весового оценивания с LSTM

### ансамбли алгоритмов
Сначала сделать обзор существующих обзор,
например, погуглив "Dietterich, T. G. (2000).  Ensemble methods in machine learning."
* оценивание распределения для каждого элемента метапризнаковой матрицы, генерация обучения для мета-алгоритма с помощью оценённого распределения

### дисбаланс
* https://arxiv.org/pdf/1901.05555.pdf - можно использовать и другой множетель для перевзвешивания (придумать!) / тут неплохой обзор подходов

### Иерерхические вложения
тут надо разбираться... :)
* https://arxiv.org/pdf/1511.06361.pdf
* https://homepages.inf.ed.ac.uk/rsarkar/papers/HyperbolicDelaunayFull.pdf
* https://arxiv.org/pdf/1705.08039.pdf
* http://hyperbolicdeeplearning.com/hyperbolic-neural-networks/
* https://arxiv.org/pdf/1805.09112.pdf
* https://arxiv.org/pdf/1804.01882.pdf

### "Regularization by noise"

### Векторные представления
Начать с обзора (см. перечень), вариант темы: сделать такое же для категорий / исследовать существующие
* Перечень всего-всего со словами https://github.com/Separius/awesome-sentence-embedding

### SNA
много тем
* для начала всё повторить и перерисовать...
* подборка ресурсов https://github.com/briatte/awesome-network-analysis
* тут есть неплохие ссылки https://habr.com/ru/company/dca/blog/265077/
* библиотека + ссылки - современные методы SNA https://github.com/benedekrozemberczki/karateclub

### графы
предложить новые подходы генерации графов, сделать эксперименты
* Есть хороший обзор:  https://arxiv.org/pdf/1910.00760v1.pdf
* **DL** графовые сети (обзор) https://arxiv.org/pdf/1901.00596.pdf

### нестандартная оптимизация
для начала просто разобраться - сделать обзо по нескольким статьям
* обзор по т.н. Quality-Diversity https://quality-diversity.github.io  https://gitlab.com/leo.cazenille/qdpy

### Дистилляция
классная идея в статье, почему-то никто не развил. Как минимум, сделать более интерпретируемые картинки (+ регуляризация как в distill.pub). Можно попробовать без диф. оптимизации сделать что-то подобное. По второй работе: можно ли базис совсем маленьким сделать???
* Tongzhou Wang, Jun-Yan Zhu, Antonio Torralba, Alexei A. Efros «Dataset Distillation» // https://arxiv.org/abs/1811.10959
* вторая работа Ilia Sucholutsky, Matthias Schonlau Soft-Label Dataset Distillation and Text Dataset Distillation // https://arxiv.org/pdf/1910.02551v2.pdf


# Интересные идеи
* Анализ ошибок известных алогритмов, здесь NER: https://arxiv.org/ftp/arxiv/papers/1910/1910.02403.pdf
* Генерация с помощью деревьев новых признаков - RuleFite: http://statweb.stanford.edu/~jhf/ftp/RuleFit.pdf

### Неевклидовы сети (просто почитать)
* Group Equivariant Convolutional Networks https://arxiv.org/abs/1602.07576
* 3D G-CNNs for Pulmonary Nodule Detection https://arxiv.org/abs/1804.04656
* Geodesic convolutional neural networks on Riemannian manifolds https://arxiv.org/abs/1501.06297
* Geometric deep learning: going beyond Euclidean data https://arxiv.org/abs/1611.08097
* Gauge Equivariant Convolutional Networks and the Icosahedral CNN https://arxiv.org/abs/1902.04615
* Fake News Detection on Social Media usingGeometric Deep Learning https://arxiv.org/abs/1902.06673
* книга Spectral Geometry of Shapes https://books.google.ru/books?hl=ru&lr=&id=j-O4DwAAQBAJ&oi=fnd
