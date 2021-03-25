# MSU
описание тем исследовательских работ для студентов

### калибровка уверенности
все ссылки есть здесь -  https://dyakonov.org/2020/03/27/проблема-калибровки-уверенности/
Есть куча идей - как сделать ещё / лучше. Нет честного сравнения всего и обзора (можно и более полный обзор сделать).

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

* Sage, A. J., Genschel, U., & Nettleton, D. (2020). Tree aggregation for random forest class probability estimation. Statistical Analysis and Data Mining: The ASA Data Science Journal. doi:10.1002/sam.11446 

*Исследуются разные способы агрегации вероятнсотей - всё на R - можно переписать и сделать лучше*

* Обзор всех новых техник! Читать и разбираться!!! https://github.com/benedekrozemberczki/awesome-decision-tree-papers

### важности признаков
* что быстее сходится (в RF, например) качество или важность
* (done) Strobl C., Boulesteix A.-L., Zeileis A., Hothorn T. Bias in random forest variable importance measures (2007). BMC Bioinformatics, 8(1), 25.

*Здесь отмечается смещение важностей в сторону признаков с большим числом категорий или масштаба. Для некоторых моделей  -зависимость от способа сэмплинга (с возвратом или без).*

* van der Laan MJ (2006) Statistical inference for variable importance. Int J Biostat. https://doi.org/10.2202/
1557-4679.1008

*поправка идёй Бреймана - на самом деле, это теоретическая работа по мат. статистике*

* Gregorutti B, Michel B, Saint-Pierre P (2015) Grouped variable importance with random forests and application to multiple functional data analysis. Comput Stat Data Anal 90:15–35
* Gregorutti B, Michel B, Saint-Pierre P (2017) Correlation and variable importance in random forests. Stat
Comput 27(3):659–678

*(вроде) теория Бреймана для регрессий*

* Fisher A, Rudin C, Dominici F (2018) All models are wrong but many are useful: Variable importance for black-box, proprietary, or misspecified prediction models, using model class reliance.
arXiv:1801.01489v3

*(вроде) какое-то новое определение важности - теоретическая статья, много непонятного*

* Datta A, Sen S, Zick Y (2016) Algorithmic transparency via quantitative input influence: theory and experiments with learning systems. In: 2016 IEEE symposium on security and privacy (SP). IEEE, pp 598–617
* Kononenko I et al (2010) An efficient explanation of individual classifications using game theory. J Mach Learn Res 11(Jan):1–18
* Staniak M, Biecek P (2018) Explanations of model predictions with live and breakDown packages. arXiv:1804.01955

*(вроде) SHARP*

* G. Louppe,  L. Wehenkel,  A. Sutera,  and P. Geurts.  Understanding variable impor-tances in forests of randomized trees. InAdvances in Neural Information ProcessingSystems, pages 431–439, 2013.
* A.  Sutera,  G.  Louppe,  V.  A.  Huynh-Thu,  L.  Wehenkel,  and  P.  Geurts.   Context-dependent feature analysis with random forests.arXiv  preprint  arXiv:1605.03848,2016.

*(вроде) теоретическое исследование про категориальные признаки*

* Robin Genuer, Jean-Michel Poggi, Christine Tuleau-Malot. Variable selection using Random Forests.Pattern Recognition Letters, Elsevier, 2010, 31 (14), pp.2225-2236.

*Тут зависимость от параметров RF*

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
* обнаружение сообществ https://github.com/benedekrozemberczki/awesome-community-detection

### графы
предложить новые подходы генерации графов, сделать эксперименты
* Есть хороший обзор:  https://arxiv.org/pdf/1910.00760v1.pdf
* **DL** графовые сети (обзор) https://arxiv.org/pdf/1901.00596.pdf
* обзор много-чего по графам (современные статьи) https://github.com/benedekrozemberczki/awesome-graph-classification
* аномалии в графах https://github.com/bhatiasiddharth/MIDAS

### экваринтные сети
тут надо разбираться - слишком много материала
* https://github.com/Chen-Cai-OSU/awesome-equivariant-network
а тут топология:
* https://github.com/Chen-Cai-OSU/Topology-and-Learning

### нестандартная оптимизация
для начала просто разобраться - сделать обзо по нескольким статьям
* обзор по т.н. Quality-Diversity https://quality-diversity.github.io  https://gitlab.com/leo.cazenille/qdpy

### Дистилляция
классная идея в статье, почему-то никто не развил. Как минимум, сделать более интерпретируемые картинки (+ регуляризация как в distill.pub). Можно попробовать без диф. оптимизации сделать что-то подобное. По второй работе: можно ли базис совсем маленьким сделать???
* Tongzhou Wang, Jun-Yan Zhu, Antonio Torralba, Alexei A. Efros «Dataset Distillation» // https://arxiv.org/abs/1811.10959
* вторая работа Ilia Sucholutsky, Matthias Schonlau Soft-Label Dataset Distillation and Text Dataset Distillation // https://arxiv.org/pdf/1910.02551v2.pdf

### Извлечение признаков из деревьев и обучение на деревьях
* Оригинальная интересная идея Celine Vens, Fabrizio Costa Random Forest Based Feature Induction // https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.454.7215&rep=rep1&type=pdf
* Её современная модификация https://arxiv.org/pdf/2011.02829.pdf
* тут просто м.б. полезный код: https://github.com/yunchuankong/forgeNet/blob/master/forgeNet.py


# Semi-, Self-and Unsupervised
* Schmarje L. et al. A survey on Semi-, Self-and Unsupervised Techniques in Image Classification //arXiv preprint arXiv:2002.08721. – 2020. https://arxiv.org/pdf/2002.08721.pdf

Отличнейший обзор!
* [заметка в блоге](https://dyakonov.org/2020/06/03/%d1%81%d0%b0%d0%bc%d0%be%d0%be%d0%b1%d1%83%d1%87%d0%b5%d0%bd%d0%b8%d0%b5-self-supervision/)
можно сделать для неглубокого обучения (получится что-то типа стекинга)

# SVM-кластеризация
обзор и реализация известных подходов, например
* http://hanj.cs.illinois.edu/pdf/aistat13_qgu.pdf
* https://www.jmlr.org/papers/volume2/horn01a/horn01a.pdf
* https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-8-S7-S18

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

### Онлайн-обучение
* Bandit Algorithms Book https://tor-lattimore.com/downloads/book/book.pdf
* блог к BAB https://banditalgs.com/
* Regret Analysis of Stochastic andNonstochastic Multi-armedBandit Problems http://sbubeck.com/SurveyBCB12.pdf
* Some Notes on Multi-armed Bandits (2020) https://courses.cs.washington.edu/courses/cse599i/20wi/resources/bandit_notes.pdf
* http://sbubeck.com/BubeckLectureNotes.pdf
* Introduction to Online Optimization 2011 курс https://courses.cs.washington.edu/courses/cse599i/18wi/
* A Modern Introduction to Online Learning https://arxiv.org/pdf/1912.13213.pdf
* ECE 543:  Statistical Learning Theory https://courses.engr.illinois.edu/ece543/sp2019/SLT.pdf
* Avrin Blum http://www.cs.cmu.edu/~avrim/Papers/survey.pdf

### Оригинальное
* Поиск прорывных / пустых научных областей

Есть такое решение: https://foundation.mozilla.org/en/blog/open-source-tool-accelerate-scientific-knowledge-discovery/
Есть более обширная база: https://dblp.org
