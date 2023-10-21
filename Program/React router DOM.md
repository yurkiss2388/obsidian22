---
aliases: 
- 
---

2023-08-20 12:42
Tags: 

___

# React router DOM

это библиотека для маршрутизации в реакт 
пример использования 
```js
import {
  createBrowserRouter,
  RouterProvider,
} from "react-router-dom";
function App() {
  const router = createBrowserRouter([
    {
      path: "/",
      element: <IndexLayout />,
      children: [
        {
          path: "userPages",
          element: <UserPages />,
        },
        {
          path: "productPage",
          element: <ProductPage />,
        },
        {
          path: "exp",
          element: <div> это пиздец</div>,
        },
      ],
    },
  
  ]);
  return (
    <div className="App container">
      <RouterProvider router={router} />
    </div>
  );
}
export default App;
```

## layout
это оболочка для контента реакт приложения 
хранит в себе повторяющееся элементы такие  как Header Footer Navigasion 

Корневой роут это роут который используется для  layout
Дочерний роут  - это роут который используется для конкретной страницы 

## outlet
контент страницы передаётся через тег outlet .
При вызове заменяется полем element из массива children 


___

## Zero-Links
-

___

## Links
-

## Source

