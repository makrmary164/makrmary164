\documentclass[a4paper, 12pt]{article} % тип документа

%%%Библиотеки
    %\usepackage[warn]{mathtext}	
    \usepackage[T2A]{fontenc}   %Кодировка
    \usepackage[utf8]{inputenc} %Кодировка исходного текста
    \usepackage[english, russian]{babel} %Локализация и переносы
    \usepackage{caption}
    \usepackage{listings}
    \usepackage{amsmath, amsfonts, amssymb, amsthm, mathtools}
    \usepackage[warn]{mathtext}
    \usepackage[mathscr]{eucal}
    \usepackage{wasysym}
    \usepackage{graphicx} %Вставка картинок правильная
    \usepackage{pgfplots}
    \usepackage{indentfirst}
    \usepackage{float}    %Плавающие картинки
    \usepackage{wrapfig}  %Обтекание фигур (таблиц, картинок и прочего)
    \usepackage{fancyhdr} %Загрузим пакет
    \usepackage{lscape}
    \usepackage{xcolor}
    \usepackage[normalem]{ulem}
    
    \usepackage{titlesec}
    \titlelabel{\thetitle.\quad}

    \usepackage{hyperref}

%%%Конец библиотек

%%%Настройка ссылок
    \hypersetup
    {
        colorlinks = true,
        linkcolor  = blue,
        filecolor  = magenta,
        urlcolor   = blue
    }
%%%Конец настройки ссылок


%%%Настройка колонтитулы
    \pagestyle{fancy}
    \fancyhead{}
    \fancyhead[L]{2.1.3}
    \fancyhead[R]{Макрушина Мария, группа Б06-205}
    \fancyfoot[C]{\thepage}
%%%конец настройки колонтитулы



\begin{document}
                        %%%%Начало документа%%%%


%%%Начало титульника
\begin{titlepage}

    \newpage
    \begin{center}
        \normalsize Московский физико-технический институт \\(госудраственный университет)
    \end{center}

    \vspace{6em}

    \begin{center}
        \Large Лабораторная работа по общему курсу физики\\Термодинамика и молекулярная физика
    \end{center}

    \vspace{1em}

    \begin{center}
        \Large \textbf{2.1.3. Определение $C_p/C_v$ по скорости звука в газе}
    \end{center}

    \vspace{2em}

    \begin{center}
        \large Макрушина Мария Алексеевна\\
        Группа Б06-205
    \end{center}

    \vspace{\fill}

    \begin{center}
    Долгопрудный \\2021
    \end{center}
    
\end{titlepage}
%%%Конец Титульника



%%%Настройка оглавления и нумерации страниц
    \thispagestyle{empty}
    \newpage
    \tableofcontents
    \newpage
    \setcounter{page}{1}
%%%Настройка оглавления и нумерации страниц


                    %%%%%%Начало работы с текстом%%%%%%
                    
\textbf{Цель работы:} измерение частоты
    колебаний
    и длины волны при
    резонансе звуковых
    колебаний в газе, заполняющем трубу; определение показателя адиабаты с помощью уравнения состояния идеального газа.\\

\textbf{Используемое оборудование:} звуковой генератор ГЗ; электронный
    осциллограф ЭО; микрофон; телефон; раздвижная труба; теплоизолированная труба, обогреваемая водой из термостата; баллон
    со сжатым углекислым газом; газгольдер.
                    
\section{Теоретическое введение}

Cкорость распространения звуковой волны в газах зависит от показателя адиабаты $\gamma$. На измерении скорости звука основан один из наиболее  точных методов определения показателя  адиабаты.
        
        Скорость звука в газах определяется формулой:
        $$c=\sqrt{\gamma\frac{RT}{\mu}},$$
        где $R$ - газовая постоянная, $T$ - температура газа, а $\mu$ его молярная масса. Выразим показатель адиабаты:
        $$\gamma=\frac{\mu}{RT} c^2$$
        
        Звуковая волна, распространяющаяся вдоль трубы, испытывает многократные отражения от торцов. Звуковые колебания в трубе являются наложением всех отраженных волн и, вообще говоря, очень сложны. Картина упрощается, если длина трубы L равна целому числу полуволн, то есть когда
        $$L=n\frac{\lambda}{2},$$
        где $\lambda$ — длина волны звука в трубе, а $n$ — любое целое число.
        
        Скорость звука c связана с его частотой $f$ и длиной волны $\lambda$ соотношением:
        $$c=\lambda f.$$
        
        Подбор условий, при которых возникает резонанс, можно производить двояко:
        
        1) При неизменной частоте $f$ звукового генератора (а следовательно, и неизменной длине звуковой волны $\lambda$) можно изменять длину трубы $L$. Для этого применяется раздвижная труба. Длина раздвижной трубы постепенно увеличивается, и наблюдается ряд последовательных резонансов. Для $k$-ого резонанса имеем:
        $$L_{n+k}=n\frac{\lambda}{2} + k\frac{\lambda}{2},$$
        т. е. $\lambda/2$ равно угловому коэффициенту графика, изображающего зависимость длины трубы $L$ от номера резонанса $k$.
        
        2) При постоянной длине трубы можно изменять частоту звуковых
        колебаний. В этом случае следует плавно изменять частоту $f$ звукового генератора, а следовательно, и длину звуковой волны $\lambda$.
        Для $k$-ого резонанса получим:
        $$L = (n+k)\frac{\lambda_{k+1}}{2}$$
        $$f_{k+1} = \frac{c}{\lambda_{k+1}}=\frac{c}{2L}(n+k)=f_1 + \frac{c}{2L}k.$$
        
        Скорость звука, деленная на $2L$, определяется, таким образом,
        по угловому коэффициенту графика зависимости частоты от номера
        резонанса.

\section{Эксперементальная установка}

\begin{figure}[h]
    \center{\includegraphics[scale = 1]{0}}
\end{figure}

    Соответственно двум методам измерения скорости звука в работе имеются две установки (рис. 1 и 2). В обеих установках звуковые колебания в трубе возбуждаются телефоном Т и улавливаются микрофоном М. Мембрана телефона приводится в движение переменным током звуковой частоты; в качестве источника переменной ЭДС используется звуковой генератор ГЗ. Возникающий в микрофоне сигнал наблюдается на осциллографе ЭО.

    Микрофон и телефон присоединены к установке через тонкие резиновые трубки. Такая связь достаточна для возбуждения и обнаружения звуковых колебаний в трубе и в то же время мало возмущает эти колебания: при расчетах оба торца трубы можно считать неподвижными, а влиянием соединительных отверстий пренебречь.

    Первая установка (рис. 1) содержит раздвижную трубу с миллиметровой шкалой. Через патрубок (на рисунке не показан) труба может наполняться воздухом или углекислым газом из газгольдера. На этой установке производятся измерения $\gamma$ для воздуха и для $CO_2$.
    
    Вторая установка (рис. 2) содержит теплоизолированную трубу постоянной длины. Воздух в трубе нагревается водой из термостата. Температура газа принимается равной температуре омывающей трубу воды. На этой установке измеряется зависимость скорости звука от температуры.
    
\section{Ход работы}

Исходя из примерного значения скорости звука ($ \approx 270$ м/c), предварительно рассчитаем, в каком диапазоне частот следует вести измерения, чтобы при удлинении трубы можно было наблюдать 4 резонанса:
$L = \frac{n\lambda}{2}$, $L + \Delta L = \frac{(n+4)\lambda}{2}$. Поскольку $\Delta L \leq 23$ см, то $\lambda \leq 11.5$ см. Следовательно $f \geq 2400$ Гц. 
        
        Проведём измерения на первой установке для $CO_2$.
        Плавно изменяя длину трубы, последовательно зафиксируем все доступные для наблюдения точки резонанса. Измерения проводятся для нескольких частот.
        \begin{center}
        \begin{tabular}{|l|l|l|l|l|l|l|l|l|l|}
            \hline
            $f$, Гц & \multicolumn{2}{|c|}{2492} & \multicolumn{2}{|c|}{2751}&  \multicolumn{2}{|c|}{3016} & \multicolumn{2}{|c|}{3265}
            \\
            \hline
            $k$ &  $l_1$, см& $l_2$, см & $l_1$, см & $l_2$, см & $l_1$, см & $l_2$, см & $l_1$, см & $l_2$, см
            \\
            
            \hline
            0 & 0 & 0 & 0,2 & 0,2 & 0,9 & 0,9 & 1,0 & 1,0
            \\
            \hline
            1 & 5,0 & 5,8 & 6,0 & 6,0 & 6,2 &  6,1 & 5,5 & 5,3
            \\
            \hline
            2 & 11,0 & 10,8 & 10,5 & 10,3 & 11,5 & 11,5 & 9,7 & 9,4
            \\
            \hline
            3 & 17,0 & 17,1 & 16,0 & 15,5 & 17,2 & 17,2 & 11,4 & 11,5
            \\
            \hline
            4 & 23,0 & 22,9 & 19,5 & 20,0 & 22,5 & 22,5 & 18,8 & 18,5
            \\
            \hline
        \end{tabular}
        \end{center}
        $l_1$ соответсвует значение на размеченной подвижной части трубы укорачиванию длины, а $l_2$ удлинению.
        Изобразим полученные результаты на графике, откладывая по оси абсцисс номер $k$ последовательного резонанса, а по оси ординат — соответствующее удлинение трубы
        $\Delta l$. Угловой коэффициент прямой определяет длину полуволны.
        
\begin{center}
    \begin{tabular}{lr}
            \begin{tikzpicture}[scale = 0.8]
            \begin{axis}[
            axis lines = left,
            legend style={at={(1,0.3)}},
            xlabel = {$k$},
            ylabel = {$\Delta l, {см} $
            },
            xmin=0, xmax=5,
            ymin=0, ymax=24,
            ymajorgrids = true,
            xmajorgrids = true,
            minor tick num = 4
            ]
            \addplot+[only marks ] plot[error bars/.cd, y dir=both, y explicit]
            coordinates {
                (0,0) +- (0.1,0.1)
                (1, 5) +- (0.1,0.1)
                (2, 11) +- (0.1,0.1)
                (3, 17) +- (0.1,0.1)
                (4, 23) +- (0.1,0.1)
                (0,0) +- (0.1,0.1)
                (1, 5.8) +- (0.1,0.1)
                (2, 10.8) +- (0.1,0.1)
                (3, 17.1) +- (0.1,0.1)
                (4, 22.9) +- (0.1,0.1)
            };
            \addplot[red, domain=0:4.5] {-0.25+5.755*x};
            
            \legend{
                $$f = 2492 {Гц}, y = -0.25+5.755x$$
            };
             \end{axis}
            \end{tikzpicture}	
            &
            
            \begin{tikzpicture}[scale = 0.8]
            \begin{axis}[
            axis lines = left,
            legend style={at={(1,0.3)}},
            xlabel = {$k$},
            ylabel = {$\Delta l, {см} $
            },
            xmin=0, xmax=5,
            ymin=0, ymax=24,
            ymajorgrids = true,
            xmajorgrids = true,
            minor tick num = 4
            ]
            \addplot+[only marks ] plot[error bars/.cd, y dir=both, y explicit]
            coordinates {
                (0,0) +- (0.1,0.1)
                (1, 5.8) +- (0.1,0.1)
                (2, 10.3) +- (0.1,0.1)
                (3, 15.8) +- (0.1,0.1)
                (4, 19.8) +- (0.1,0.1)
                (0,0) +- (0.1,0.1)
                (1, 5.8) +- (0.1,0.1)
                (2, 10.1) +- (0.1,0.1)
                (3, 15.3) +- (0.1,0.1)
                (4, 19.8)	+- (0.1,0.1)
            };
            \addplot [red, domain=0:4.5]{0.45+4.885*x};
            
            \legend{
                $$f = 2751{Гц},y=0.45+4.885x$$
            };
                        \end{axis}
            \end{tikzpicture}
            \\	
            
            \begin{tikzpicture}[scale = 0.8]
            \begin{axis}[
            axis lines = left,
            legend style={at={(1,0.3)}},
            xlabel = {$k$},
            ylabel = {$\Delta l, {см} $
            },
            xmin=0, xmax=5,
            ymin=0, ymax=24,
            ymajorgrids = true,
            xmajorgrids = true,
            minor tick num = 4
            ]
            
            \addplot+[only marks ] plot[error bars/.cd, y dir=both, y explicit]
            coordinates {
                (0,0) +- (0.1,0.1)
                (1, 5.3) +- (0.1,0.1)
                (2, 10.6) +- (0.1,0.1)
                (3, 16.3) +- (0.1,0.1)
                (4, 21.6) +- (0.1,0.1)
                (0,0) +- (0.1,0.1)
                (1, 5.2) +- (0.1,0.1)
                (2, 12.5) +- (0.1,0.1)
                (3, 16.3) +- (0.1,0.1)
                (4, 21.6) +- (0.1,0.1)
            };
            \addplot[red, domain=0:4.5] {0.20+5.425*x};
            \legend{
                $$f = 3016 {Гц},y = 0.20+5.425x$$
            };
            \end{axis}
            \end{tikzpicture}
            
            &
            
            \begin{tikzpicture}[scale = 0.8]
            \begin{axis}[
            axis lines = left,
            legend style={at={(1,0.3)}},
            xlabel = {$k$},
            ylabel = {$\Delta l, {см} $
            },
            xmin=0, xmax=5,
            ymin=0, ymax=24,
            ymajorgrids = true,
            xmajorgrids = true,
            minor tick num = 4
            ]
            
            \addplot+[only marks ] plot[error bars/.cd, y dir=both, y explicit]
            coordinates {
                (0,0) +- (0.1,0.1)
                (1, 4.5) +- (0.1,0.1)
                (2, 8.7) +- (0.1,0.1)
                (3, 10.4) +- (0.1,0.1)
                (4, 17.5) +- (0.1,0.1)
                (0,0) +- (0.1,0.1)
                (1, 4.3) +- (0.1,0.1)
                (2, 8.4) +- (0.1,0.1)
                (3, 10.5) +- (0.1,0.1)
                (4, 17.5) +- (0.1,0.1)
            };
            \addplot [red, domain=0:4.5] {-0.06+4.135*x};
            \legend{
                $$f = 3265 {Гц}, y = -0.06+4.135x$$
            };
            \end{axis}
            \end{tikzpicture}
            
            \\
    \end{tabular}
\end{center}
        
        Вычислим с помощью полученных графиков скорость звука в углекислом газе и рассчитаем погрешности.
        
        Погрешность $\sigma_{c}$ отдельного измерения определяется следующей формулой:
        $$ \sigma_{c} =c \sqrt{\Big(\frac{\sigma_{\lambda}}{\lambda}\Big)^2+ \Big(\frac{\sigma_{f}}{f}\Big)^2}.$$
        
        Результаты представлены в таблице:
        \begin{center}
        \begin{tabular}{|l|l|l|l|l|}
            \hline
            $f$, Гц & 2488 & 2749 & 3013 & 3262
            \\
            
            \hline
            $\lambda,{\text{м}} \cdot 10^{-2} $ & 5,755 & 4,885 & 5,425 & 4,135
            \\
            \hline
            $c,\frac{\text{м}}{\text{с}}$ & 286,829 & 268,773 & 327,236 & 270,016 
            \\
            \hline
            $\sigma_{\lambda},{\text{м}} \cdot 10^{-2} $ & 0,022 & 0,022 & 0,022 & 0,022
            \\
            \hline
            $\sigma_{f},{\text{Гц}}$ & 5 & 5 & 5 & 5 
            \\
            \hline
            $\sigma_{c},\frac{\text{м}}{\text{с}}$ & 1,238 & 1,305 & 1,436 & 1,495
            \\
            \hline
        \end{tabular}
        \end{center}
        Можно заметить, что значения скоростей звука при различных частотах не совпадают.
        Усреднив полученные значения найдём окончательное значение скорости звука в углекислом газе. 
        $$\overline{c} = 288,2 \:\frac{\text{м}}{\text{с}}$$
        $$c_{сл} = \sqrt{\frac{\sum_{i=1}^{5} (c_{i}-\overline{c})^2}{4}} = 27,2 \: \frac{\text{м}}{\text{с}}.$$
        
        $$ c_{кос} = \sqrt{\frac{\sum_{i=1}^{5} (\sigma_{c_{кос}})^2}{5^2}} = 0,69 \; \frac{\text{м}}{\text{с}}.$$
        
        Общая погрешность: $$\sigma_{c} = \sqrt{(c_{\text{сл}})^2+(c_{кос})^2} = 27,2\frac{\text{м}}{\text{с}}.$$
        Итак, $$c = 288,2 \pm 27,2 \; \frac{\text{м}}{\text{с}}.$$
        Теоретическое значение скорости при температуре $t = 24,1 ^\circ C$ равно $$с_{т} = 273,6 \: \frac{\text{м}}{\text{с}}.$$
        В пределах погрешности эксперементальное значение совпадает с теоретическим.
        Однако стоит сказать пару слов о таком сильном разбросе для $c$. Это может быть связано с тем, что подвижную часть цилиндра двигали не достаточно медленно.
        
        Проведём измерения на второй установке. Данные представлены в таблице.
        
        $f_1$ - соотвествует значениям при увеличении частоты на трубу, $f_2$ - при уменьшении. Видно, что данные воспроизводятся при обратном ходе.		

\begin{figure}
    \begin{center}
        \includegraphics[scale = 0.9]{1}
    \end{center}
\end{figure}

\begin{figure}
    \begin{center}
        \includegraphics[scale = 0.9]{2}
    \end{center}
\end{figure}
    
        Полученные результаты изобразим на графике, откладывая
        по оси абсцисс номер резонанса $k$, а по оси ординат — разность между частотой последующих резонансов и частотой первого резонанса: $\Delta f_k = f_{k+1}-f_1.$ Угловой
        коэффициент прямой определяет величину $c/2L$.
        
\begin{figure}
    \begin{center}
        \includegraphics[scale = 0.5]{3}
    \end{center}
\end{figure}

\begin{figure}
    \begin{center}
        \includegraphics[scale = 0.5]{4}
    \end{center}
\end{figure}

\begin{figure}
    \begin{center}
        \includegraphics[scale = 0.5]{5}
    \end{center}
\end{figure}

\begin{figure}
    \begin{center}
        \includegraphics[scale = 0.5]{6}
    \end{center}
\end{figure}

    Вычислим с помощью полученных графиков скорость звука в воздухе и рассчитаем погрешности. Погрешность $\sigma_{c}$ отдельного измерения определяется следующей формулой:
    $$ \sigma_{c} =c \sqrt{\Big(\frac{\sigma_{L}}{L}\Big)^2+ \Big(\frac{\sigma_{A}}{A}\Big)^2},$$
    где $A$ - коэффициент наклона прямой на графике.
    Результаты представлены в таблице:
    \begin{center}
    \begin{tabular}{|l|l|l|l|l|l|}
        \hline
        $t$, $^\circ$ C & 22,0 & 32,5 & 44 & 51,1 & 59,6
        \\
        
        \hline
        $A,\text{Гц}$ & 216,7 & 219,0 & 223,0 & 226,0 & 228,0
        \\
        \hline
        $c,\frac{\text{м}}{\text{с}}$ & 345,6 & 350,4 & 356,8 & 361,6 & 364,8
        \\
        \hline
        $\sigma_{\text{A}},{\text{Гц}} $ & 1,1 & 1,1 & 1,1 & 1,1 & 1,1
        \\
        \hline
        $\sigma_{L},{\text{м}} \cdot 10^{-3} $ & 1 & 1 & 1 & 1 & 1 
        \\
        \hline
        $\sigma_{c},\frac{\text{м}}{\text{с}}$ & 1,814 & 1,855 & 1,815 & 1,816 & 1,821
        \\
        \hline
        $\gamma$ & 1,413 & 1,403 & 1,401 & 1,408 & 1,396
        \\
        \hline
        $\sigma_{\gamma}$ & 0,014 & 0,014 & 0,014 & 0,014 & 0,014
        \\
        \hline
    \end{tabular}
    \end{center}

    По полученным данным расчитаем $\gamma$.
    $$\overline{\gamma} = 1,402$$
    $$\gamma_{сл} = \sqrt{\frac{\sum_{i=1}^{5} (\gamma_{i}-\overline{\gamma})^2}{4}} = 0,019 .$$
    
    Косвенная погрешность определения $\gamma$ мала, так как $\frac{2\sigma_c}{4c} \approx 0,25 \%.$
    
    Итак, $$\gamma = 1,402 \pm 0,019,$$ 
    
    что в пределах погрешности совпадает  с теоретическим значением $\gamma = 1,4.$
    
    \section{Заключение}
    
    Если обратить внимание на полученные значения для $c$, то можно усомниться в справедливости формулы $c^2 = \frac{\gamma R T}{\mu}$ и начать предпологать, что показатель адиабаты является функцией от температуры $\gamma = \gamma(T)$. Однако причина точно не в активировавшихся степенях свободы (температуры очень малы), а в том, что  измерения производились не во время достижения термодинамического равновесия и нужно было ждать приличное время (около 5 минут) после того как на термостате установится необходимая температура, для того чтобы система пришла в пригодное состояние для измерений.


\section{Список используемой литературы}

$\bullet$ Гладун А. Д. Лабораторный практикум по общей физике. Термодинамика и молекулярная физика\\

$\bullet$ Сивухин Д. В. Общий курс физики. Термодинамика и молекулярная физика. Том 2\\

$\bullet$ \href{https://mipt.ru/education/chair/physics/S_II/lab/}{Описание лабораторных работ на кафедре общей физики МФТИ}

\end{document}
