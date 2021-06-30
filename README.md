# Кому он нужен с точки зрения волновой графа

--------------------------------------------------------------------------------
*Russian Verstion*
*You will find the English version below, after the Russian version*

--------------------------------------------------------------------------------

Это репозиторий с данными для построения волнового графа с корневым утверждением:

### "Отравление Навального - это операция спецслужб России"

*Замечание 1: Смотрите внизу статьи краткое пояснение, что такое волновой граф и волновой анализ, лежащий в основе построения волнового графа*

*Замечание 2: Это репозитория с данными. Скрипты и подробное пояснение, как ими пользоваться и как строится волновой граф находятся в репозитории https://github.com/nihole/wikigraph*.

# Идея

Мы описываем волновые цепочки, состоящие из аргументов за и против в YAML файле в соответствии с правилами [волнового анализа](https://habr.com/ru/post/506670/). В этом же файле, для каждого утверждения (утверждение соответствует вершине графа) мы приводим ссылку на статью с цитатами, фактами, логическим обоснованием, подтверждающими данное утверждение. Далее, скриптом мы создаем сам граф (wikigraph) на основе данных из этого YAML файла.

# Цели

Важно понимать, что волновой анализ не пытается ничего доказать или опровергнуть, и тем более не является инструментом для того, чтобы утвердить определенную, ограниченную точку зрения и заклеймить противоположную. Прелесть этого подхода заключается в том, что он дает возможность рассмотреть все возможные значимые утверждения и логические цепочки, как за, так и против. Информация открыта, и каждый может принять участие в построении и анализе волнового графа.

Вы можете форкнуть данный репозиторий, изменить YAML файл (изменив логику) или любую статью с аргументацией, создать новый граф и сделать pull request. Это инициирует дискуссию и, если ваше изменение выглядит разумно, оно будет добавлено.

Цель волнового анализа заключается не только в протоколировании и формализации дискуссии, но, что на мой взгляд, более интересно, в том, чтобы понять, почему вы или ваш оппонент имеет ту или иную картину мира. 

# Результаты

Мы можем строить граф целиком или разбить его на подграфы. Каждая вершина графа может быть использована как корневое утверждение для другого графа. На данный момент по исследуемой теме построено 2 подграфа:

- [kremlin.svg](https://github.com/nihole/wg_navalny/blob/main/graphs/kremlin/kremlin_navalny.svg). Этот граф представляет позицию власти по поводу отравления Навального (соответсвующий YAML файл - [kremlin.yml](https://github.com/nihole/wg_navalny/blob/main/yaml/kremlin/kremlin_navalny.yml)). Вы можете скопировать svg файл к себе и открыть в любом браузере или кликнуть на приведенный линк и открыть его на github. Если вы открыли его на github обязательно выберете 'raw' в меню над картинкой и после этого уменьшите масштаб.

  После этого тексты нод становятся кликабельными, что позволит вам легко попадать в статьи, соответсвующие вершинам графа.

- ['nw_1.svg'](https://github.com/nihole/wg_navalny/blob/main/graphs/nw_1/nw_1.svg). Это волновой анализ только одного из утверждений власти: 'Кому он нужен?' (Путин) (соответствующий YAML файл - [nw_1.yml](https://github.com/nihole/wg_navalny/blob/main/yaml/nw_1/nw_1.yml)). Так же как и в предыдущем случае, нажмите 'Raw' и уменьшите масштаб.

Фактически, это запротоколированная логика Кремля со ссылками на соответствующие статьи. Здесь нет критики.

Далее, я взял лишь один аргумент и проанализировал его. 

Всю логику рассуждений и аргументацию вы найдете в [викиграфах](https://github.com/nihole/wg_navalny), поэтому я только хочу поделиться теми выводами, которые мы можем сделать. 

# Опорные точки

Так нужен или нет? Почему некоторые считают, что у власти были причины для попытки устранения Навального, а другие твердо уверены, что "да кому он нужен"?

Давайте рассмотрим выводы, которые можно сделать с помощью волнового анализа.

Итак, есть несколько ключевых моментов:

- Уровень веры в то, что говорит Путин

  Логика простая - это самая короткая логическая цепочка. Если вы верите, что Путин говорит правду, то для вас граф разрешился. 

- Уровень веры в то, что говорит Навальный

  Здесь у нас симметричная ситуация. Думаю, что есть люди, которые просто верят, поэтому здесь тоже короткая волна. Если уровень веры словам Навального и / или его соратникам высокий, то понятно, что Навальный в вашем мировосприятии очень даже нужен.

Если вы все же не настолько внушаемы, то дальше логика следующая:

- Если вы верите, что Навальный является сильной политической фигурой, а власть слаба (сейчас или в перспективе), то вы однозначно считаете, что Навальный "нужен". Это в принципе довольно банальное утверждение. Интересным является то, почему люди считают Навального "сильным" или "слабым" (и тоже самое по отношению к власти), но об этом чуть позже.

- Но, если вы считаете Навального ничтожным, а власть сильной, то это не приводит однозначно к выводу, что власть не причастна к тому, что произошло с Алексеем. К этому обязательно нужно добавить еще адекватность и компетентность. Это относится к функционированию власти в том, что касается

  - информации
  - аналитики
  - управления

  Если хоть в одном из этих компонентов есть изъян, тогда вы не можете доверять власти. Так, предположим, что Навальный не представлял угрозу Кремлю, но информация была искажена, или аналитика была ошибочной, или решение принималось на местечковом уровне... Поэтому здесь мы имеем следующую важную опорную точку - уровень **адекватности власти**.

  Сюда же можно отнести и уровень **компетентности спецслужб**. В действительности, это очень важная опорная точка для изначального вопроса ("был ли Алексей отравлен спецслужбами России?").

  Все, что касается **личностных качеств Путина** - также безусловно здесь.

Но и это еще не все. Предположим, что власть сильна, Навальный и его сторонники слабы, и все находится под контролем власти. Но

- Почему бы не перестраховаться? Здесь выходит на свет вопрос о цене. Сколько придется "заплатить" за устранение, если операция сорвется, и история станет достоянием общественности. Как оценить риски и выгоду? Здесь порождаются волны, которые заканчиваются все в тех же опорных точках, связанных с адекватностью, компетентностью и личностными качествами.

Далее, давайте посмотрим, куда уходят волны, связанные с "силой" Навального и власти.

- Почему люди по-разному оценивают силу влияния Навального? Мы видим, что волны упираются в следующие циклы или опорные точки:

  - Несколько волн уходит в оценку Навального как личности (хороший-плохой) и доверия к нему
  - Соцопросы и доверие соцопросам
  - Поддержка Навального: митинги, выходы на улицу, дотации - много / мало людей; кто поддерживает - враги России / истинные патриоты, спецслужбы Запада / неравнодушные граждане
  - Деятельность ФБК (и другие проекты, связанные с Навальным): оценка значимости и правдивости расследований
  - Навальный, как политик: программа - есть / нет, хорошая / плохая

  Т.к. часть из этих вопросов чисто оценочная, а другая не имеет четких критериев оценки, то каждый может "подогнать" ответ под свои субъективные ожидания, что сводится к тому, что именно **эмоциональное отношение к Навальному и членам его команды** является ключевым. 

  Но есть утверждение, которое стоит особняком, и оно порождает несколько важных волн, а именно

  - Вопросы, связанные с тем, способен ли электорат Навального ("хомячки") в действительности противостоять власти. Вы можете симпатизировать Навальному и считать, что он обладает достаточной поддержкой, но способны ли "хомячки" к противостоянию с реальностью? В действительности, соответствующие волны уходят в вопросы, связанные с философией и психологией. 

- Теперь поговорим о том, что лежит в основе нашего представления о силе / слабости власти? В принципе, обычно здесь присутствует консенсус. Власть централизована и выглядит сильной, но, все же мы можем отметить несколько волн:

  - Динамика уровня поддержки
  - Мы не можем говорить о провластных структурах, как едином органе, власть неоднородна. Для некоторых групп расследования Навального могли быть вполне болезненны - так это или нет?
  - Пример Белоруссии выявил потенциальные риски для власти (что бы было, если бы в Белоруссии был бы лидер уровня Навального?) - так это или нет?
  - Здоровье Путина 

# Выводы

Итак, мы видим, что анализ лишь одного высказывания породил десятки волн с порядка сотней утверждений (и этот граф еще не завершен). Но как происходит обычная дискуссия? Обычно мы способны обсудить лишь несколько утверждений, "попрыгать" по логическим цепочкам (волнам), потоптаться где-то у вершины или в середине графа. Но это не имеет большого смысла, если это, конечно, не телевизионное шоу со вполне понятными целями. Как в физике граничные условия определяют решение дифференциального уравнения, так и наша реальность проявляется в той или иной интерпретации в зависимости от того, какие значения принимают наши опорные точки. Во время дискуссии нужно стремиться двигаться вниз по волне, в сторону иррациональных границ, формирующих нашу реальность (или реальность наших оппонентов). Если хотите переубедить, то именно эти точки должны быть атакованы.

В контексте данной статьи наиболее значимыми (но не единственными) опорными точками являются: 

- Отношение к личности Путина
- Отношение к личности Навального и его окружению
- Оценка уровня управления, аналитики, качества работы с информацией власти и спецслужб
- И вечные вопросы о том, что является истинными человеческими ценностями, реальной силой в мире людей - идея, мораль, страх... и можно ли, например, обладать действительной властью, избегая насилия...

#Дополнение. Несколько слов о том, что такое Волновой Анализ

О том, что такое волновой граф и волновой анализ, лежащий в его основе можно прочитать [на Хабре](https://habr.com/ru/post/506670/).

Если коротко, то волновой граф - это представление информации в логической зависимости, изображаемой в виде графа. При этом каждая вершина графа - это в общем случае статья (например, в вики), а каждое ребро отображает зависимость между этими утверждениями, и эта зависимость может быть двух видов: дополнение  и опровержение разной силы, что порождает 3 вида зависимости:

- **прямое опровержение** (сильная зависимость)
  На графе представлен в виде сплошной линии со стрелкой. Если стрелка направлена от A к B, это значит, что B опровергает A. "Прямое" значит, что это сильное опровержение, то есть, если верно B, то A - ложь. 
- **косвенное опровержение** (косвенная зависимость)
  На графе представлен в виде пунктирной линии со стрелкой. Если стрелка направлена от A к B, это значит, что B опровергает A. "Косвенное" значит, что это слабое опровержение, то есть, если верно B, то вероятность того, что A  ложь увеличивается. 
- дополнение
  На графе обозначается красным цветом и сплошной линией с стрелками в обе стороны. Логически это отрицания, то есть, если B ложь, то А - истина, а если В правда, то А - ложь. 

Краткое пояснение, терминологию и детальный пример можно найти [здесь](https://github.com/nihole/wikigraph)


--------------------------------------------------------------------------------

*English version*

--------------------------------------------------------------------------------

# wg_navalny

This is a wikigraph data repository. 

Wikigraph is a graph created based on principles of Wave Analysis. Refer to https://github.com/nihole/wikigraph/ for details.

# What is investigated

The statement under investgation is

**"Was Alexei Navalny poisoned by the Russian special services or not?"**

So the root node's statement is 

**"This (poisoning) was an operation by the Russian special services."**

# Folders structure

- **yaml**. This is where the YAML files are located, describing the logical chains (waves) 
  - **kremlin**. This data is related to the Kremlin's line of defense. This is the point of view offered and cultivated by the Russian authorities
  - **nw_1**. We took only one statement of Russian authorities and analyzed it using wave analysis. nw_1 stands for negative wave 1 and is related to node with id = '--1--' and the statement "Who needs him?" (Putin)
  - **draft**. These are just experimental graphs. Pay no attention to it
- **graphs**. This folder is used for graphs. These graphs are created from previously discussed YAML files (refer to https://github.com/nihole/wikigraph/ for details) 
  - **kremlin**. Graph [kremlin_navalny.svg](https://github.com/nihole/wg_nav/blob/main/graphs/kremlin/kremlin_navalny.svg) is created from [kremlin_navalny.yml](https://github.com/nihole/wg_nav/blob/main/yaml/kremlin/kremlin_navalny.yml) YAML file
  - **nw_1**. Graph [nw_1.svg](https://github.com/nihole/wg_nav/blob/main/graphs/nw_1/nw_1.svg) is created from [nw_1.yml](https://github.com/nihole/wg_nav/blob/main/yaml/nw_1/nw_1.yml) YAML file

# Results

This analysis is still ongoing. At the moment we have two more or less complete subtrees associated with:

- Kremlin point o view (Kremlin defense)

<img src="https://github.com/nihole/wg_nav/blob/main/graphs/kremlin/kremlin_navalny.svg" alt="Kremlin deffense">

- Analysing of only one statement in this Kremlin defence: "Who needs him?" (Putin)

<img src="https://github.com/nihole/wg_nav/blob/main/graphs/nw_1/nw_1.svg" alt="Who needs him?">

Click on the images above and select "Raw" on the right side of the panel above the image (without this, the node links won't work). Then, by navigating to the nodes of the graph and clicking on the links, you will open wiki articles related to node descriptions.
