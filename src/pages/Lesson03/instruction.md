おのうえさんは 200 人分の男女の身長と体重のデータを持っています。
(出典：[日本人 20 歳の身長と体重サンプルデータ - Excel VBA 数学教室](https://excelmath.atelierkobato.com/height/))

データは `input` として以下のように与えられます。

```json
[
  { "name": "宇内 歓行", "gender": "男性", "y": 183.87, "x": 85.54 },
  { "name": "大小原 康幸", "gender": "男性", "y": 179.54, "x": 80.94 },
  { "name": "朝永 孝幸", "gender": "男性", "y": 173.62, "x": 72.99 },
  { "name": "瀬治山 啓之", "gender": "男性", "y": 167.83, "x": 62.86 },
  ：
]

```

おのうえさんはこの中から男性のデータのみを散布図で表示したいと思っています。

おのうえさんはうまくデータを変換することができませんでした。
おのうえさんを助けるために、`src/pages/Lesson03/index.js` を開き `input` から `gender` が男性の要素のみを取り出した配列を返す関数 `convertData` を実装してください。

```javascript
const convertData = (input) => {
  return []; // ここを作りましょう！
};
```
