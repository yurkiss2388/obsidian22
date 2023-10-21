[[Итератор]] по массиву , возвращает новый элемент.
```jsx
const pizzaCard = [
    {
      title: 'С креветками и трюфелями',
      description: 'Домашнаяя паста феттуччине, сливочный соус, креветки, трюфельное масло, черный перец, пармезан.350 г',
      price: '600'
    },
    {
      title: 'С креветками ',
      description: 'Домашнаяя паста',
      price: '700'
    },
  ]

const array = [
'1 строка', '2 строка'
]
{pizzaCards.map((item, key) => <PizzaCard
          key={key}
          title={item.title}
          description={item.description}
          price={item.price}
          getPivo={item.getPivo}
        />)}
{array.map((item, key) => <Btn
          text= {item}
        />)}
```
описание:
item - название элемента который получается при итерации массива   