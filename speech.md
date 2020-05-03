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

- [ ] Bo Li, et al **Towards Fast and Accurate Streaming End-to-End ASR** https://arxiv.org/abs/2004.11544

Вроде практическая доработка LAS, но не вникал

- [ ] Takato Fujimoto **Semi-Supervised Learning Based on Hierarchical Generative Models for End-to-End Speech Synthesis**

вызов - сделать TTS для японского языка (non-alphabetic languages)
обычно для таких моделей нужны grapheme-to-phoneme conversion model
variational auto-encoder (VAE) -> semi-supervised learning.
TTS + латентные переменные позволяют контролировать атрибуты речи:
* GMVAE-Tacotron [13]
* Capacitron [14]
* controllable TTS system based on semi-supervised generative models [15]
нет кода
https://ieeexplore.ieee.org/document/9054466

- [ ] Tomoki Hayashi **Espnet-TTS: Unified, Reproducible, and Integratable Open Source End-to-End Text-to-Speech Toolkit**
e2e-TTS toolkit "ESPnet-TTS"
поддержка Tacotron 2, Transformer TTS, FastSpeech
+ предтренированные модели!
есть код! есть примеры!
https://arxiv.org/pdf/1910.10909.pdf
https://espnet.github.io/icassp2020-tts/

- [ ] Tae-Ho Kim **Emotional Voice Conversion Using Multitask Learning with Text-To-Speech**
Voice conversion (VC) - Изменение голоса, сохраняя лингвистический контент
обычно seq2seq, Но есть потери
здесь multitask learning + TTS (т.е. не звук -> звук)
т.е. модель, которая делает и TTS и VC
есть обзор про VC - там ссыка на аналог Cycle-GAN
кода и примеров ПОКА нет
https://arxiv.org/pdf/1911.06149.pdf

- [ ] Zhen Zeng **Aligntts: Efficient Feed-Forward Text-to-Speech System Without Explicit Alignment**
главное достижение - скорость (чуть-чуть выше и качество)
но нет кода и примеров
https://arxiv.org/abs/2003.01950


- [ ] Se-Yun Um **Emotional Speech Synthesis with Rich and Granularized Control**
отмечается, что хорошо, когда есть датасет с разметкой эмоций
Но в этой работе контролируется ещё и интенчивность эмоции
используется GST-Tacotron
нет кода и примеров
https://arxiv.org/abs/1911.01635


- [ ] Erica Cooper **Zero-Shot Multi-Speaker Text-To-Speech with State-Of-The-Art Neural Speaker Embeddings**
как раз нужная задача!
Есть всё - и код и примеры!
https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9054535
https://nii-yamagishilab.github.io/samples-multi-speaker-tacotron/
https://github.com/nii-yamagishilab/multi-speaker-tacotron



- [ ] Rafael Valle **Mellotron: Multispeaker Expressive Voice Synthesis by Conditioning on Rhythm, Pitch and Global Style Tokens**
https://nv-adlr.github.io/Mellotron 


### предобработка
- [ ] Improving Audio Quality in Duo with WaveNetEQ https://ai.googleblog.com/2020/04/improving-audio-quality-in-duo-with.html

### распознавание
- [ ] Tae Jin Park, Kyu J. Han, Jing Huang, Xiaodong He, Bowen Zhou, Panayiotis Georgiou, Shrikanth Narayanan **Speaker Diarization with Lexical Information** https://arxiv.org/abs/2004.06756




