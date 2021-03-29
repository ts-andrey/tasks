# Задание №2: Components

## Требования:

1. Создать компонент `BookComponent`. Используйте его в `AppComponent`. Модель книг `BookModel` описать интерфейсом:  
   • `name`: _string_;  
   • `description`: _string_;  
   • `price`: _number_;  
   • `category`: _enum_ (Создайте enum с несколькими категориями);  
   • `createDate`: _number_;  
   • `isAvailable`: _boolean_;
2. Вывести свойства `BookComponent` в его темплейте. 3. Добавить кнопку `Buy` в шаблон `BookComponent`. Реализовать обработчик события `onBuy` по нажатию на кнопку `Buy`, который должен добавлять книгу в корзину. `BookComponent` реализовать как презентационный компонент с `input` и `output`, без зависимостей. Если товара нет, кнопку `Buy` делать недоступной.
3. Создать компонент `CartComponent` и использовать в `AppComponent` темплейте. Создать `CartItemComponent` и использовать внутри `CartComponent`. Компонент `CartItemComponent` должен отображать приобретенную книгу и колличество единиц данного экземпляра. Реализовать возможности: изменить количество товара, удалить товар из корзины.
4. Для взаимодействия между компонентами использовать декораторы: `@Input()`, `@Output()`.
5. По возможности использовать `OnPush` стратегию для презентационных компонентов (`BookComponent`, `CartItemComponent`).
6. По возможности использовать два или более метода-хука жизненного цикла компонента.
7. Использовать различные DOM событие (`click`, `wheel`, `blur`...).
8. Добавить в разметку AppComponent элемент <h1 #appTitle></h1> с шаблонной переменной. Использовать `@ViewChild`, получить доступ к DOM-элементу темплейта, установить заголовок для приложения из класса.

## Рекомендации:

Не используйте для имен событий, которые генерят компоненты префикс `on`. Используйте его для нейминга обработчиков этих событий