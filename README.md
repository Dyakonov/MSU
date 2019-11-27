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


### эффективные методы поиска ближайших соседей
* материалы из лекции

### случайные леса
* kernel + RF https://arxiv.org/pdf/1502.03836.pdf (ещё много чего есть). Если поискать, то
* * https://arxiv.org/pdf/1402.4293.pdf (тут ядра как в АПкРО)
* сравнение с Extra-Trees https://stats.stackexchange.com/questions/175523/difference-between-random-forest-and-extremely-randomized-trees

### оптимизация гиперпараметров
сделать обзор существующих методов / предложить быстрые (не обязательно для настройки ML-алгоритмов)
* Байесовский подход: [отсюда](https://github.com/WillKoehrsen/hyperparameter-optimization/blob/master/Introduction%20to%20Bayesian%20Optimization%20with%20Hyperopt.ipynb) ходить по ссылкам
* много современных исследований: https://sigopt.com/research
* хорошая обзорная работа https://app.sigopt.com/static/pdf/SigOpt_Bayesian_Optimization_Primer.pdf

### генерация графов

предложить новые подходы, сделать эксперименты
* Есть хороший обзор:  https://arxiv.org/pdf/1910.00760v1.pdf

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


### Иерерхические вложения
тут надо разбираться... :)
* https://arxiv.org/pdf/1511.06361.pdf
* https://homepages.inf.ed.ac.uk/rsarkar/papers/HyperbolicDelaunayFull.pdf
* https://arxiv.org/pdf/1705.08039.pdf
* http://hyperbolicdeeplearning.com/hyperbolic-neural-networks/
* https://arxiv.org/pdf/1805.09112.pdf
* https://arxiv.org/pdf/1804.01882.pdf

### "Regularization by noise"

# Интересные идеи
* Анализ ошибок известных алогритмов, здесь NER: https://arxiv.org/ftp/arxiv/papers/1910/1910.02403.pdf
* Генерация с помощью деревьев новых признаков - RuleFite: http://statweb.stanford.edu/~jhf/ftp/RuleFit.pdf
