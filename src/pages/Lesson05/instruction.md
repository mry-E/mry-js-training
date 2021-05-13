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

`y` は身長、 `x` は体重を表しています。

おのうえさんは、身長のヒストグラムを表示したいと思いました。
そのためには、それぞれの人の身長を小数点以下で四捨五入し、その値の人が何人いるかの頻度を数える必要があります。
また、それぞれの身長の中で男女を色分けして内訳を表したいと思っています。

目的のヒストグラムを表示するために以下のような集計データを作る必要があります。

```json
[
  ：
  { "bin": "155", "男性": 0, "女性": 3 },
  { "bin": "156", "男性": 0, "女性": 9 },
  { "bin": "157", "男性": 4, "女性": 5 },
  { "bin": "158", "男性": 1, "女性": 4 },
  { "bin": "159", "男性": 0, "女性": 6 },
  { "bin": "160", "男性": 2, "女性": 2 },
  { "bin": "161", "男性": 4, "女性": 8 },
  { "bin": "162", "男性": 1, "女性": 7 },
  { "bin": "163", "男性": 4, "女性": 5 },
  { "bin": "164", "男性": 2, "女性": 5 },
  ：
]
```

各要素の `bin` には身長の値を表す文字列が、`男性` と `女性` にはこの身長の値に該当する男女それぞれの人数が格納されています。

おのうえさんはうまくデータを変換することができませんでした。
おのうえさんを助けるために、`src/pages/Lesson05/index.js` を開き `input` のデータを目的の形式に変換する `convertData` を実装してください。

```javascript
const convertData = (input) => {
  return []; // ここを作りましょう！
};
```