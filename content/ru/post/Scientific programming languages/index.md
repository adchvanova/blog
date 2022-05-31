---
title: Научные языки программирования
subtitle: О научных языках программирования.

# Summary for listings and search engines
summary: Что такое языки программирования

# Link this post with a project
projects: []

# Date published
date: '2022-05-24T00:00:00Z'

# Date updated
lastmod: '2022-05-24T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin
 

tags:
  - Academic


categories:
  - Demo

---
## Научные языки программирования и среды.
По мере того, как компьютеры становятся все более распространенными в физических исследованиях (и научных исследованиях в целом), вопрос о том, какие языки программирования использовать, становится все более важным. Факторы, которые особенно влияют на важность этого вопроса:

    возрастающая сложность программируемых задач;
    возрастающая сложность и разнообразие программируемых машин;
    все более широкое использование графической визуализации и взаимодействия с научными программами; а также
    растущее число языков программирования, доступных для программирования.
    
    С и С++
C — интересный выбор в качестве научного языка. Он чрезвычайно гибкий и доступен практически на каждой машине, известной человеку. Кроме того, один из лучших компиляторов C (gcc) доступен бесплатно. Почти все пакеты визуализации и пользовательского интерфейса поддерживают язык C. C часто преподается как первый или второй язык на факультетах информатики университетов.

Давняя претензия к C заключается в том, что он производит более медленный код, чем эквивалентный Fortran. В настоящее время скорость компьютеров удваивается каждый год или около того, и компиляторы C, похоже, не так уж плохи по сравнению с Fortran (типичный код C работает на 50–100% быстрее, чем эквивалентный Fortran, в зависимости от приложения). В свете этого я думаю, что трудно отказаться от C из-за скорости кода, который он производит.

Тем не менее, я не думаю, что это хороший научный язык программирования. Язык C довольно близок к аппаратному обеспечению, и при написании приложения довольно легко допустить большие ошибки. Эти ошибки часто не проявляются в небольших тестовых примерах, поскольку они связаны с проблемами управления памятью и т.п. Кроме того, программирование больших приложений на C требует определенной степени профессионализма, что означает достаточно глубокое знание языка. Таким образом, это плохой язык для основного научного программирования; как правило, только создатель программы или люди с реальным опытом в области компьютерного программирования смогут понять большое приложение на C, если оно не будет написано очень тщательно.

Я считаю, что эти комментарии применимы и к кодированию на C++. Опасения по поводу удобочитаемости и профессионализма применимы здесь, возможно, даже в большей степени, чем к «просто C». Преимущество C++ состоит в том, что он является самым популярным объектно-ориентированным языком, но он также признан довольно загадочным. Опять же, необходима определенная степень профессионализма, чтобы запрограммировать приложение на C++, понятное другим. Пакеты, которые автоматически генерируют код C++ из заданного пользователем псевдокода, помогают облегчить проблему, но тогда мы сталкиваемся с просьбой ко всем пользователям использовать один и тот же генератор C++, что является еще одной проблемой того же масштаба.

Вышеуказанные два являются «традиционными» вариантами. Теперь я перехожу к более новым языкам, менее известным в научном сообществе.
питон
Python — это объектно-ориентированный расширяемый интерпретируемый язык. Он работает практически на всех системах Unix, а также на платформах DOS/Windows и на Mac. Это бесплатно и поставляется с полным исходным кодом. Начать использовать Python очень просто — на простом уровне он напоминает Basic и может использоваться в интерактивном режиме так же, как и Basic. Однако он поддерживает объектные методы и хорошо "масштабируется". Масштабирование указывает на относительную сложность написания небольших и больших приложений. Средства объекта помогают и поощряют писать приложение небольшими частями. Эти маленькие части могут быть объединены в большую программу, а маленькие части могут также использоваться в других приложениях.

Еще одним преимуществом Python является его расширяемость. Можно написать библиотеку объектов на C, C++ или родном Python, которую затем можно динамически или статически связать с основной системой Python и использовать в программах Python. Это можно использовать для создания программируемого приложения, такого как пакет для построения графиков данных. Можно добавить в интерпретатор пакет, содержащий команды для настройки ваших графиков и фактического построения данных. Этому интерпретатору Python+графики можно дать другое имя, например "pygraph", и вызвать его как команду. Интерпретатор будет обрабатывать графические команды и выполнять их. Однако в то же время вы можете использовать любую другую допустимую команду Python в качестве команды для этой графической программы! Таким образом, один графический входной файл для этой программы мог сначала вычислить результат, а затем обработать его и построить его.

Переход от этого к системам пакетов Python+, таким как программы анализа данных или программы управления экспериментами, довольно очевиден. Это также может в некоторой степени решить упомянутую выше дилемму об использовании C++. Профессиональный программист может создать четко определенный пакет библиотеки с четко определенным интерфейсом на C++, который может быть включен в программы Python для использования. Поскольку Python почти так же читаем, как и Fortran, «нормальный человек» (то есть тот, кто не является профессиональным программистом) может использовать эту библиотеку в своих программах. И профессионалы, которым нужны мощь и эффективность C или C+