# hse_hw2_chip
### _Сушкова Дарья Сергеевна, подгруппа 2._
Homework 2 bioinformatics.
### Общая информация
Показатель | Значение 
--- | --- 
Клеточная линия | HepG2 
Гистоновая метка | H3K4me1 
ID эксперимента | ENCSR000APV 
ID Реплики 1 | ENCFF000BEX 
ID Реплики 2 | ENCFF000BEY 
ID контроля | ENCFF474ZPM 
Хромосома выравнивания | chr15 
ID bed narrowPeak | ENCFF532AGT 
Версия | GRCh38 
### [Ссылка на Google Colab](https://colab.research.google.com/drive/17GHH--RrzdSspmII-bscAv8RBvqHVSId?usp=sharing)
### FastQC
_Примечание:_ файлы $.html$ с выдачей также прредставлены в репозитории в папке $FastQC.$   
ENCFF000BEX | ENCFF000BEY | ENCFF474ZPM  
--- | --- | ---  
![image](https://user-images.githubusercontent.com/89806836/220106897-95369cea-59ea-461f-a62c-2197f30f7625.png) | ![image](https://user-images.githubusercontent.com/89806836/220109391-d3683ef3-2fd3-4aa4-bb28-d78f8b30b2da.png) | ![image](https://user-images.githubusercontent.com/89806836/220109544-85db3c6d-8a0e-4fa2-b371-75efbe8abf39.png)
![image](https://user-images.githubusercontent.com/89806836/220109674-24b8230a-f2ab-45bf-adce-1ba65daa7bb1.png) | ![image](https://user-images.githubusercontent.com/89806836/220109774-39cddfa9-e8f7-4a38-847b-eacf1bb42a41.png) | ![image](https://user-images.githubusercontent.com/89806836/220109839-1705fb9d-7491-4208-9ba3-6bba1e9d42df.png) 
![image](https://user-images.githubusercontent.com/89806836/220110310-b3a961ea-f11c-4403-9406-369c91798c3b.png) | ![image](https://user-images.githubusercontent.com/89806836/220110405-8bcf3afb-64ea-4b5c-ab7b-ca06819642c0.png) | ![image](https://user-images.githubusercontent.com/89806836/220110492-54a74c05-2432-4067-9cee-7257947618ed.png)
![image](https://user-images.githubusercontent.com/89806836/220110701-8f02f7ac-dabb-4b26-9c9a-6dfa0b5ecd24.png) | ![image](https://user-images.githubusercontent.com/89806836/220110777-03375332-b0d5-41e3-b785-42ec74840b0e.png) | ![image](https://user-images.githubusercontent.com/89806836/220110871-487d76c5-38d8-4f9e-94c6-f6d7cf177229.png) 
![image](https://user-images.githubusercontent.com/89806836/220111005-4ac13735-ed43-4d40-99b0-09267e76bff5.png) | ![image](https://user-images.githubusercontent.com/89806836/220111109-f6204ea9-b5b6-4267-8508-8b02553d75bf.png) | ![image](https://user-images.githubusercontent.com/89806836/220111201-7acb1f90-204f-4ce0-8ee6-527fadad4e31.png)
![image](https://user-images.githubusercontent.com/89806836/220111296-d9079029-88a4-4b20-af61-08a1a16fedbe.png) | ![image](https://user-images.githubusercontent.com/89806836/220111371-e6f182cd-5f52-4fa6-8894-207f34dd57c6.png) | ![image](https://user-images.githubusercontent.com/89806836/220111414-a91f5eb1-4b84-4141-b435-5d8dc85b0141.png)   

_Вывод:_ сама выдача $FastQC$ показала хорошее качество для всех графиков анализа (везде зеленые галочки). Наиболее важным параметром является $Per\ base\ sequence\ quality,$ который показывает хорошее качество чтений, все в зеленой области. В принципе, результаты для двух реплик практически идентичны, результаты для контроля тоже не особо отличаются. Так как качество хорошее, то фильтрация и подрезание чтений не производились.
### Таблица со статистикой
Образец | Кол-во чтений | Уникальные чтения | Неуникальные чтения | Не выравнявшиеся чтения 
--- | --- | --- | --- | --- 
ENCFF000BEX | 31037661 | 1187419 (3.83%) | 4335277 (13.97%) | 25514965 (82.21%) 
ENCFF000BEY | 31263991 | 1194821 (3.82%) | 4505886 (14.41%) | 25563284 (81.77%) 
ENCFF474ZPM | 21261022 | 744559 (3.50%) | 2002990 (9.42%) | 18513473 (87.08%) 
    
_Вывод:_ процент выравниваний получился таким (процент НЕ выравнявшихся чтений намного больше для всех образцов $>80$), потому что выравнивание производилось только на одну хромосому (еще и сравнительно небольшую в целях экономии памяти), то есть рассматривается далеко не весь геном.   
### Диаграммы Венна
_Примечание:_ $.pdf$ файлы хранятся в репозитории в папке $Intervene\ Venn$ для каждой реплики соответственно.
#### Реплика 1
AGT&BEX | BEX&AGT 
--- | --- 
![image](https://user-images.githubusercontent.com/89806836/220063010-c3edae49-d01d-451d-b7e9-e117c8a9c7bc.png) | ![image](https://user-images.githubusercontent.com/89806836/220063335-7167fe79-9823-4279-9360-5b668f8d1046.png) 
#### Реплика 2
AGT&BEY | BEY&AGT 
--- | --- 
![image](https://user-images.githubusercontent.com/89806836/220085145-85667f3a-9bbb-4f23-839c-6981a62f84cc.png) | ![image](https://user-images.githubusercontent.com/89806836/220085247-a7bb2495-736f-476c-847d-a14a43bee377.png) 
   
_Выводы:_ из диаграмм Венна видно, что количество наших $MACS2$ пиков меньше, чем количество пиков, приведенных в $ENCODE$ для рассматриваемого эксперимента. Это связано с тем, что для наших реплик выравнивание производилось на одну хромосому, а в $ENCODE$ - на всех. Различие в количестве пересечений связано с условным порядком указания файлов в параметрах операции $intervene\ venn$ (сначала за "опорный" берется $ENCODE$, а за второстепенный наш, потом наоборот) хотя относительно общего количества пиков в файлах разница небольшая. Предположу, что теоретически это различие связано опять же с выравниванием на одну хромосому.
### Бонусная часть
#### Общая информация
Показатель | Значение 
--- | --- 
ID bam (Реплика 1) | ENCFF401IDX 
ID bam (Реплика 2) | ENCFF995WXM 
ID bigWig (Реплика 1) | ENCFF900MSU 
ID bigWig (Реплика 2) | ENCFF637SSH   
Версия | hg19 
#### Ngs-plot
ENCFF900MSU | ENCFF637SSH 
--- | --- 
![result1](https://user-images.githubusercontent.com/89806836/220156055-2691b8d5-4e15-42a2-a2e9-674fa5422704.png) | ![result2](https://user-images.githubusercontent.com/89806836/220156120-a9e39ff1-c69d-4e1e-83b4-d815cff2c243.png) 
   
_Вывод:_ для обеих реплик результаты получились практически идентичны (только небольшая разница в числовых метках шкалы количества чтений). До $TSS$ наблюдается рост сигнала метки, в $TSS$ - резкое падение и такое же резкое возрастание, постепенное уменьшение до $TES$ и слабое увеличение после $TES.$ На картинке, данной в условиях ДЗ, для гистоновой метки $H3K4me1$ характерен постепенный рост после $TES$, это соответствует построенным графикам $ngs-plot.$
