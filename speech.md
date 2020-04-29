# Работа со звуком / речью - статьи todo
ссылки на ресурсы для проработки

### синтез речи
- [ ] Guangzhi Sun **FULLY-HIERARCHICAL FINE-GRAINED PROSODY MODELING FOR INTERPRETABLE SPEECH SYNTHESIS** https://arxiv.org/pdf/2002.03785.pdf
- [ ] Guangzhi Sun **Generating diverse and natural text-to-speech samples using a quantized fine-grained VAE and auto-regressive prosody prior**  https://arxiv.org/abs/2002.03788

- [x] Soumi Maiti, Erik Marchi, Alistair Conkie **Generating Multilingual Voices Using Speaker Space Translation Based on Bilingual Speaker Data** https://arxiv.org/abs/2004.04972

Рассматривается задача, когда произносятся фразы на двух языках, есть двуязычные спикеры, а есть одноязычные. Надо синтезировать голос одноязычного спикера на чужом языке. Используют Такотрон, добавляют представления спикера - 2LSTM+Lin+Softmax (обучаемся отличать спикеров). Новизна в том, что обычно такие представления спикеров рассматривали для одноязычных. Представления для спикер-язык образуют кластеры, переход к другому языку - смещение в нужный кластер.

- [x] BookTubeSpeech https://users.wpi.edu/~jrwhitehill/BookTubeSpeech/

Датасет разных спикеров, взятый с ютуба. Но очень большие файлы... хорош для академических исследований "представлений спикеров".

- [x] Ann Clifton **The Spotify Podcasts Dataset**

Датасет подкастов, транскрибация с помощью Гугла (в том числе на уровне слова),  47,000 часов.

### предобработка
- [ ] Improving Audio Quality in Duo with WaveNetEQ https://ai.googleblog.com/2020/04/improving-audio-quality-in-duo-with.html

### распознавание
- [ ] Tae Jin Park, Kyu J. Han, Jing Huang, Xiaodong He, Bowen Zhou, Panayiotis Georgiou, Shrikanth Narayanan **Speaker Diarization with Lexical Information** https://arxiv.org/abs/2004.06756




