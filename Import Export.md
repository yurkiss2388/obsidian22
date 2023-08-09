Позволяет решить проблему модульности кода , создание отдельных модулей которые содержат в себе определенные наборы данных и функций, которые можно подключить и с ними работать

```js
export const checkLS = () => {
	if(localStorage.getItem('w')) return true;
	return false;
}

export const showMessage = text => {
	return '{text}! Message not found';
}

%%добавим к export import%%

import {checkLS, showMessage} from './cookies.js';
if (!checkLS()) console.log(showMessage('Problem'));
```
можно разбивать на множество модулей и использовать их где-то ещё 