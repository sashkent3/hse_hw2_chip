# Ссылка на Colab
https://colab.research.google.com/drive/1zt62_MEbPiSGCmoxVzBCBJIB_JuOjLSN?usp=sharing

# Fastqc
Отчёты fastqc в формате html находятся в папке fastqc. Судя по результатам анализа тримминг не требуется. В последовтельностях нет адаптеров, качество хорошее.
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/JMD_PerBaseSequenceQuality.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/JMD_PerSequenceGCContent.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/JMD_AdapterContent.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/TVN_PerBaseSequenceQuality.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/TVN_PerSequenceGCContent.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/TVN_AdapterContent.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/RYF_PerBaseSequenceQuality.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/RYF_PerSequenceGCContent.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/images/RYF_AdapterContent.png)

# Статистика по каждому из образцов

|Sample|Reads|Unique aligned|Non-unique aligned|Not aligned|
|------|-------|------|------|------|
|ENCFF190TVN|39640834|1327746 (3.35%)|3606424 (9.10%)|34706664 (87.55%)|
|ENCFF797JMD|24313947|791672 (3.26%)|2014290 (8.28%)|21507985 (88.46%)|
|ENCFF303RYF|12923893|437914 (3.39%)|1201362 (9.30%)|11284617 (87.32%)|

__Ответ на вопрос из ноутбука:__ большинство чтений (~88%) оказалось не выравнено из-за того, что выравнивание производилось всего на одну хромосому, а не на весь геном для экономии ресурсов.

# Диаграммы
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/venn/Intervene_venn-1.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/venn/Intervene_venn-2.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/venn/Intervene_venn-3.png)
![](https://raw.githubusercontent.com/sashkent3/hse_hw2_chip/main/venn/Intervene_venn-4.png)

__Ответ на вопрос из ноутбука:__ можно видеть, что общее число пиков в наших данных значительно меньше. Скорее всего это опять связано с тем, что мы рассматриваем только одну хромосому из всего генома. В то же время среди пиков, найденных в наших экспериментах, большинство отсуствует в эксперименты с encodeproject. Возможно это вызвано какой-то дополнительной предобработкой данных или отличающимися параметрами в процессе.
