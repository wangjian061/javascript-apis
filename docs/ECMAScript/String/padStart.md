# padStart() <Badge text="ES7"/>

## 语法

```ts
padStart(length: number, fillStr?: string): string;
```

## 描述

用于将`fillStr`字符串填充到调用此方法的字符出的前面，使返回的字符串的长度等于`length`

- 当只传递`length`而不传递`fillStr`时，默认以`空字符串`填充

- 当`fillStr`的长度加上`原字符串`的长度大于`length`时，只保留最左侧的部分，其他部分会被截断

- 当`length`小于等于`原字符串`时，返回`原字符串`

## 示例

```js
const str = 'messi';

str.padStart(9, 'goat'); // 'goatmessi'
str.padStart(1, 'goat'); // 'messi'
str.padStart(6, 'goat'); // 'gmessi'
str.padStart(10); // '     messi'
```
