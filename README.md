# en-teamwork1

# перевод Георгий Попов Андреевич ( AR-15)

# card

### card
Создавайте макеты с разными стилями.

### Использование
Компонент «Карта» состоит из самой карты, тела карты и необязательного названия карты. Обычно карточки располагаются в столбцах сетки из компонента «Сетка».

### Класс :       Описание:

.uk-card       | Добавьте этот класс в элемент <div>, чтобы определить компонент Card.
          
.uk-card-body  | Добавьте этот класс к карточке, чтобы создать отступы между карточкой и ее содержимым.

.uk-card-title | Добавьте этот класс в заголовок, чтобы определить заголовок карты.

![image](https://github.com/user-attachments/assets/d4107ef1-1205-4958-bb65-6f5230014aa7)

 <div class="uk-card uk-card-body">
    <h3 class="uk-card-title"></h3>
</div>

По умолчанию карта пустая. Вот почему важно добавить класс-модификатор для стилизации. В нашем примере мы используем класс .uk-card-default.

# По умолчанию                                                   

 <div class="uk-card uk-card-default uk-card-body uk-width-1-2@m">
    <h3 class="uk-card-title">Default</h3>
    <p>Lorem ipsum <a href="#">dolor</a> sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
</div>

### Модификаторы стиля

UIkit включает в себя ряд модификаторов, которые можно использовать для придания карточкам определенного стиля.

### Класс :       Описание:

 .uk-card-default | Добавьте этот класс, чтобы создать поле с визуальным стилем.                        
                                                                                  
.uk-card-primary  | Добавьте этот класс, чтобы изменить карту и подчеркнуть ее основным цветом.         

.uk-card-secondary| Добавьте этот класс, чтобы изменить карточку и придать ей дополнительный цвет фона. 

# пример:

<div class="uk-card uk-card-default"></div>

<div class="uk-card uk-card-primary"></div>

<div class="uk-card uk-card-secondary"></div>

# По умолчанию       

![image](https://github.com/user-attachments/assets/18090a42-8e0b-4b81-a913-d5311a4dc5b1)

<div class="uk-child-width-1-3@m uk-grid-small uk-grid-match" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-body">
            <h3 class="uk-card-title">Default</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-primary uk-card-body">
            <h3 class="uk-card-title">Primary</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-secondary uk-card-body">
            <h3 class="uk-card-title">Secondary</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
    </div>
</div>

### Модификатор при наведении

Вы можете применять к картам разные модификаторы размера, которые уменьшат или увеличат их отступы.

### Класс :       Описание:
.uk-card-small    Добавьте этот класс, чтобы применить меньшие отступы.

.uk-card-large    Добавьте этот класс, чтобы применить больший отступ.

<div class="uk-card uk-card-small uk-card-default"></div>

<div class="uk-card uk-card-large uk-card-default"></div>

![image](https://github.com/user-attachments/assets/86e209ce-fbcc-4c93-a467-bd5e7099a487)

<div class="uk-child-width-1-2@s" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-small uk-card-body">
            <h3 class="uk-card-title">Small</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-large uk-card-body">
            <h3 class="uk-card-title">Large</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
        </div>
    </div>
</div>

### Верхний и нижний колонтитулы

Вы также можете разделить карточку на верхний и нижний колонтитулы — вокруг тела по умолчанию. Просто добавьте класс .uk-card-header или .uk-card-footer к элементу <div> внутри карточки.

<div class="uk-card">
    <div class="uk-card-header">
        <h3 class="uk-card-title"></h3>
    </div>
    <div class="uk-card-body"></div>
    <div class="uk-card-footer"></div>
</div>

![image](https://github.com/user-attachments/assets/68302dd4-7d83-40f4-bf6c-fae26e6c5aa8)

<div class="uk-card uk-card-default uk-width-1-2@m">
    <div class="uk-card-header">
        <div class="uk-grid-small uk-flex-middle" uk-grid>
            <div class="uk-width-auto">
                <img class="uk-border-circle" width="40" height="40" src="images/avatar.jpg" alt="Avatar">
            </div>
            <div class="uk-width-expand">
                <h3 class="uk-card-title uk-margin-remove-bottom">Title</h3>
                <p class="uk-text-meta uk-margin-remove-top"><time datetime="2016-04-01T19:00">April 01, 2016</time></p>
            </div>
        </div>
    </div>
    <div class="uk-card-body">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.</p>
    </div>
    <div class="uk-card-footer">
        <a href="#" class="uk-button uk-button-text">Read more</a>
    </div>
</div>

### СМИ

Чтобы отобразить изображение внутри карточки без каких-либо пробелов, добавьте один из следующих классов в <div> вокруг элемента <img>. Имейте в виду, что вам необходимо соответствующим образом изменить исходный порядок.

.uk-card-media-top      Этот класс указывает, что медиа-элемент выровнен по верху.

.uk-card-media-bottom	  Этот класс указывает, что медиа-элемент выровнен по нижнему краю.

.uk-card-media-left    Этот класс указывает, что медиа-элемент выровнен по левому краю.

.uk-card-media-right  Этот класс указывает, что медиа-элемент выровнен по правому краю.

<div class="uk-card uk-card-default">
    <div class="uk-card-media-top">
        <img src="" width="" height="" alt="">
    </div>
    <div class="uk-card-body"></div>
</div>

![image](https://github.com/user-attachments/assets/d09f2571-cdc6-4900-9f8d-2486c512bdcb)

<div class="uk-child-width-1-2@m" uk-grid>
    <div>
        <div class="uk-card uk-card-default">
            <div class="uk-card-media-top">
                <img src="images/light.jpg" width="1800" height="1200" alt="">
            </div>
            <div class="uk-card-body">
                <h3 class="uk-card-title">Media Top</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.</p>
            </div>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-default">
            <div class="uk-card-body">
                <h3 class="uk-card-title">Media Bottom</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.</p>
            </div>
            <div class="uk-card-media-bottom">
                <img src="images/light.jpg" width="1800" height="1200" alt="">
            </div>
        </div>
    </div>
</div>

### Значок
Чтобы разместить значок внутри карты, добавьте класс .uk-card-badge к элементу контейнера. Для стилизации значка вы можете использовать один из других компонентов, например Label.

<div class="uk-card uk-card-body">
    <div class="uk-card-badge uk-label"></div>
</div>

![image](https://github.com/user-attachments/assets/4e3c58e1-40cb-42c7-8fd6-fb54da53542c)

<div class="uk-card uk-card-default uk-card-body uk-width-1-2@m">
    <div class="uk-card-badge uk-label">Badge</div>
    <h3 class="uk-card-title">Title</h3>
    <p>Lorem ipsum color sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
</div>


______________________________________________________________________________________________________________
# перевод Болкаревой Анны
Cover(обложка)

Разверните изображения, видео, iframe'ы так, чтобы они занимали весь контейнер и поместите сверху свой контент.

#Usage (использование)

Чтобы изображение могло наложиться на родительский элемент, добавьте класс ".uk-cover-container" к родительскому элементу и "uk-cover" к картинке/фотографии.

" <div class="uk-cover-container">
    <img src="" alt="" uk-cover>
</div> "

!Заметка! Чтобы поместить контент на уже наложенный элемент(картинку), используйте Position component (компонент положения). Чтобы адаптировать видимость, добавьте ".uk-light" или ".uk-dark" из Inverse component(обратная составляющаяя).
Предпросмотр:

![image](https://github.com/user-attachments/assets/f3c1f647-5e63-4245-8016-eec20e082422)

<div class="uk-cover-container uk-height-medium">
    <img src="images/dark.jpg" alt="" uk-cover>
</div>


#Video (видео)

Чтобы создать видео, которое будет покрывать родительский контейнер, добавьте "uk-cover" атрибут к видео. Заверните элемент контейнера вокруг видео и добавьте класс ".uk-cover-container" чтобы закрепить контент.

Элемент обложки наследует все свойства из компонента видео , это значит, что видео лишены звука и проигрываются автоматически. Таким образом, они будут останавливаться в тот момент, когда будут покидать поле зрения и начинаться тогда, когда будут в него попадать.

<div class="uk-cover-container">
    <video uk-cover></video>
</div>

Предпросмотр:

![image](https://github.com/user-attachments/assets/6a4b1fa1-0d07-412f-8f28-8bb24f242eb0)


<div class="uk-cover-container uk-height-medium">
    <video src="https://yootheme.com/site/images/media/yootheme-pro.mp4" autoplay loop muted playsinline uk-cover></video>
</div>



#Iframe (личная подсказка:  iFrame — элемент HTML, позволяющий встраивать на веб-страницу документы, видео и интерактивные медиафайлы и прочие части содержимого из других источников)

чтобы добавить элемент обложки к iframe'у, нужно добавить атрибут "uk-cover" к iframe'у. После добавьте класс ".uk-cover-container" к элементу контейнера поверх iframe'а, чтобы закрепить контент.

<div class="uk-cover-container">
    <iframe src="" uk-cover></iframe>
</div>

предпросмотр: 

<div class="uk-cover-container uk-height-medium">
    <iframe src="https://www.youtube-nocookie.com/embed/c2pz2mlSfXA?autoplay=1&amp;controls=0&amp;showinfo=0&amp;rel=0&amp;loop=1&amp;modestbranding=1&amp;wmode=transparent" width="1920" height="1080" allowfullscreen uk-cover></iframe>
</div>


#Responsive height (Адаптивная высота) 

Чтобы добавить адаптивное поведение к изображению на обложке, вам нужно создать невидимый элемент "canvas"(холст) и присвоить ему значения ширины и высоты в соответствии с соотношением сторон, которое вы хотите, чтобы имела охватываемая область. Таким образом, он адаптирует адаптивное поведение изображения.

<div class="uk-cover-container">
    <canvas width="" height=""></canvas>
    <img src="" alt="" uk-cover>
</div>

предпросмотр

<div class="uk-cover-container">
    <canvas width="400" height="200"></canvas>
    <img src="images/dark.jpg" alt="" uk-cover>
</div>


#Viewport height (высота видового окна/экрана)

Добавление атрибута "uk-height-viewport" Из height component (компонента высоты) увеличит высоту родительского элемента, чтобы заполнить весь видовой экран


<div class="uk-cover-container" uk-height-viewport>
    <img src="" alt="" uk-cover>
</div>

#Component options (Параметры компонентов)

К атрибуту компонента можно применить любой из этих параметров. Разделяйте несколько параметров точкой с запятой

Опции|описания|значения|по умолчанию

automute|	Boolean(логический)|	true(правда)|	Пытается автоматизировать видео в iframe.

widt |   Number(номер)	|      Ширина элемента.

height|	Number(номер)	|	Высота элемента.

#Javascript

инициализация

Иконки 
 Размещайте масштабируемые векторные значки в любом месте вашего контента. 
UIkit поставляется с собственной системой значков SVG и обширной библиотекой, которая включает в себя растущее количество элегантных контурных значков. Этот компонент внедряет SVG-файлы на сайт, чтобы они принимали цвет и могли быть стилизованы с помощью CSS. 
  # Использование  
Обязательно подключите скрипт библиотеки значков,более подробную информацию смотрите в инструкции по установке. 
       <script src="uikit/dist/js/uikit-icons.min.js"></script> 
Чтобы применить компонент,добавьте uk-icon отнести к <span> или <a> элемент.Чтобы отобразить фактический значок,вам нужно добавить icon: NAME параметр для атрибута.И вуаля,ты имеешь векторный значок, который наследует цвет, как и ваш текст. 
    <span uk-icon="icon: check"></span> 
 
    <a href="" uk-icon="icon: heart"></a> 
Если icon единственная опция в значении атрибута, вы также можете использовать uk-icon="NAME"  
    <span uk-icon="heart"></span> 
<span class="uk-margin-small-right" uk-icon="check"></span> 
 
<a href="" uk-icon="heart"></a> 
  # Библиотека  
Вот обзор всех доступных на данный момент значков. Со временем мы будем добавлять в список новые значки. 
 Приложения 
 home 
 sign-out 
 user 
 users 
 lock 
 unlock 
 settings 
 cog 
 nut 
 comment 
 commenting 
 comments 
 hashtag 
 tag 
 cart 
 bag 
 credit-card 
 mail 
 receiver 
 print 
 search 
 location 
 bookmark 
 code 
 paint-bucket 
 camera 
 video-camera 
 bell 
 microphone 
 bolt 
 star 
 heart 
 happy 
 lifesaver 
 rss 
 social 
 git-branch 
 git-fork 
 world 
 calendar 
 clock 
 history 
 future 
 crosshairs 
 pencil 
 trash 
 move 
 link 
 link-external 
 eye 
 eye-slash 
 question 
 info 
 warning 
 image 
 thumbnails 
 table 
 list 
 menu 
 grid 
 more 
 more-vertical 
 plus 
 plus-circle 
 minus 
 minus-circle 
 close 
 check 
 ban 
 refresh 
 play 
 play-circle 
  Устройства 
 tv 
 desktop 
 laptop 
 tablet 
 phone 
 tablet-landscape 
 phone-landscape 
   Хранилище 
 file 
 file-text 
 file-pdf 
 copy 
 file-edit 
 folder 
 album 
 push 
 pull 
 server 
 database 
 cloud-upload 
 cloud-download 
 download 
 upload 
  Направление 
 reply 
 forward 
 expand 
 shrink 
 arrow-up-right 
 arrow-up 
 arrow-down 
 arrow-left 
 arrow-right 
 chevron-up 
 chevron-down 
 chevron-left 
 chevron-right 
 chevron-double-left 
 chevron-double-right 
 triangle-up 
 triangle-down 
 triangle-left 
 triangle-right 
   Редактор  
bold 
 italic 
 strikethrough 
 quote-right 
   Бренды 
 500px 
 android 
 android-robot 
 apple 
 behance 
 bluesky 
 discord 
 dribbble 
 etsy 
 facebook 
 flickr 
 foursquare 
 github 
 github-alt 
 gitter 
 google 
 instagram 
 joomla 
 linkedin 
 mastodon 
 microsoft 
 pinterest 
 reddit 
 signal 
 soundcloud 
 telegram 
 threads 
 tiktok 
 tripadvisor 
 tumblr 
 twitch 
 uikit 
 vimeo 
 whatsapp 
 wordpress 
 x 
 xing 
 yelp 
 yootheme 
 youtube 
  # Соотношение 
Добавьте ratio: 2 параметры для uk-icon атрибут, чтобы удвоить его размер — или любое другое число, в зависимости от того, насколько большим вы хотите, чтобы ваш значок был. 
  <span uk-icon="icon: check; ratio: 2"></span> 
  <span class="uk-margin-small-right" uk-icon="icon: check; ratio: 2"></span> 
  <span uk-icon="icon: check; ratio: 3.5"></span> 
  # Модификатор ссылки  
Чтобы сбросить стиль ссылки по умолчанию на более приглушенный цвет при использовании значка внутри привязки, добавьте .uk-icon-link сорт. 
 <a href="" class="uk-icon-link" uk-icon="heart"></a> 
<div> 
    <a href="#" class="uk-icon-link uk-margin-small-right" uk-icon="copy"></a> 
    <a href="#" class="uk-icon-link uk-margin-small-right" uk-icon="file-edit"></a> 
    <a href="#" class="uk-icon-link" uk-icon="trash"></a> 
</div> 
 # Модификатор биттона 
Используйте модификатор .uk-icon-button класс на <a> элемент для создания кнопки со значком, который можно использовать для значков социальных сетей. 
<a href="" class="uk-icon-button" uk-icon="instagram"></a> 
<div> 
    <a href="" class="uk-icon-button uk-margin-small-right" uk-icon="instagram"></a> 
    <a

    href="" class="uk-icon-button  uk-margin-small-right" uk-icon="facebook"></a> 
    <a href="" class="uk-icon-button" uk-icon="youtube"></a> 
</div> 
 # Модификатор изображения  
Вы также можете масштабировать любое фоновое изображение до размера значка. Просто добавьте .uk-icon-image класс и путь к фоновому изображению. 
<span class="uk-icon uk-icon-image" style="background-image: url(images/dark.jpg);"></span> 
 # Варианты компонентов  
Любой из этих параметров можно применить к атрибуту компонента. Разделяйте несколько вариантов точкой с запятой. Узнать больше. 
  Вариант Значение По умолчанию Описание 
icon Строка  Значок для отображения 
ratio Номер 1 Соотношение размеров значков. 
icon это Primary  Опция и ее ключ могут быть опущены, если это единственная опция в значении атрибута. 
<span uk-icon="heart"></span> 
  # JavaScript 
Узнайте больше о компонентах JavaScript. 
   Инициализация 
UIkit.icon(element, options); 
   Характеристики 
 svg 
Обещание JavaScript, которое будет разрешено с добавлением узла SVG. 
UIkit.icon(element).svg.then(function(svg) { svg.querySelector('path').style.stroke = 'red'; }) 
  # Доступность  
Установите соответствующие роли, состояния и свойства WAI-ARIA для компонента Icon. 
Если <a> используется элемент,установите aria-label собственность в <a> элемент, описывающий его значение. 
<a href="" uk-icon="icon: heart" aria-label="…"></a>
