---
title: Вложенные компоненты
---

Весьма нерационально размещать целое приложение в единственном компоненте. Лучше импортировать компоненты из других файлов и вставлять их в разметку как обычные HTML элементы.

Добавьте тег `<script>` в котором будет импортироваться файл `Nested.svelte`...

```html
<script>
	import Nested from './Nested.svelte';
</script>
```

...и вставьте его в разметку:

```html
<p>Просто строка текста</p>
<Nested/>
```

Обратите внимание, что в файле`Nested.svelte` тоже есть элемент `<p>`, но стили из `App.svelte` никак на него не влияют.