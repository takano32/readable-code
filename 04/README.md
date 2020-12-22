# 4. 美しさ


優れたソースコードは目に優しい

* 読み手が慣れているパターンを意識する
* 似ているコードは似ていると分かるようにする
* 関連するコードはひとつのブロックにする


## 4-1. なぜ美しさが大切なのか？

美しくないと理解に時間がかかる

[![Image from Gyazo](https://i.gyazo.com/d2bf9e179a784d8eba4215766cc177d2.png)](https://gyazo.com/d2bf9e179a784d8eba4215766cc177d2)

美しくした例

[![Image from Gyazo](https://i.gyazo.com/fa9a271a495c73992d545250c0b4a774.png)](https://gyazo.com/fa9a271a495c73992d545250c0b4a774)

**プログラミングのほとんどの時間はコードを読む時間**

## 4-2. 一貫性のある簡潔な改行位置

TcpConnectionSimulator クラスのコンストラクタには 4 つの仮引数

1. 接続速度(Kbps)
2. 平均遅延時間(ms)
3. 遅延「イライラ」時間(ms) 4. パケットロス率(%)

改行の位置が悪い例

[![Image from Gyazo](https://i.gyazo.com/83db06428fc113a6053d8d8f88726439.png)](https://gyazo.com/83db06428fc113a6053d8d8f88726439)

改行の位置が良い例

[![Image from Gyazo](https://i.gyazo.com/afb367e852addba72bab630f762408d8.png)](https://gyazo.com/afb367e852addba72bab630f762408d8)

さらにコメントの冗長性を取り除いた例

[![Image from Gyazo](https://i.gyazo.com/9874e93b2ae313872962991b5deb8a1e.png)](https://gyazo.com/9874e93b2ae313872962991b5deb8a1e)

## 4-3. メソッドを使った整列

同一の処理がまとめられていないと読みにくい


[![Image from Gyazo](https://i.gyazo.com/6a45835fec343e5ece8b090e819cdfb3.png)](https://gyazo.com/6a45835fec343e5ece8b090e819cdfb3)


ヘルパーメソッドを作成し処理をまとめて分かりやすくした例

[![Image from Gyazo](https://i.gyazo.com/855d0ab8977a80a3e3336d5aed9050f2.png)](https://gyazo.com/855d0ab8977a80a3e3336d5aed9050f2)

* 重複を排除したことでコードが簡潔になった。
* テストケースの大切な部分(名前やエラー文字列)が見やすくなった。以前 は、database_connection や error などのトークンに囲まれていて、コード を見て「飲み込む」のが難しかった。
* テストの追加が簡単になった。

**テストコードだからといって assert を連発すればよいというものではない**


## 4-4. 縦の線をまっすぐにする

先ほどの例に注目

[![Image from Gyazo](https://i.gyazo.com/ad559836e62f5ffca999e38b04dc7da4.png)](https://gyazo.com/ad559836e62f5ffca999e38b04dc7da4)

表敬式のようにすると分かりやすい

[![Image from Gyazo](https://i.gyazo.com/d7c9d20e10d6fbbdc1e91b2f7b21800d.png)](https://gyazo.com/d7c9d20e10d6fbbdc1e91b2f7b21800d)

規則性をもたせると間違いも見つけやすい

[![Image from Gyazo](https://i.gyazo.com/d40ecfc3ecc686641ed7af89db3de0fc.png)](https://gyazo.com/d40ecfc3ecc686641ed7af89db3de0fc)

### 備考: wget での例

[![Image from Gyazo](https://i.gyazo.com/9eb456c81df5cd98d9747d4bc869d601.png)](https://gyazo.com/9eb456c81df5cd98d9747d4bc869d601)

### 備考: プロダクトでの例

位置合わせ前

[![Image from Gyazo](https://i.gyazo.com/97664a7984773845a021a3d259625190.png)](https://gyazo.com/97664a7984773845a021a3d259625190)

位置合わせ後

[![Image from Gyazo](https://i.gyazo.com/e8b8681798d14ebc679db4d870683636.png)](https://gyazo.com/e8b8681798d14ebc679db4d870683636)

## 4-5. 一貫性と意味のある並び

フォームの例

* 対応する HTML フォームの <input> フィールドと同じ並び順
* 「最重要」なものから重要度順
* アルファベット順

改善前

[![Image from Gyazo](https://i.gyazo.com/6bef151b134dd938dbaad2cd8eb403bc.png)](https://gyazo.com/6bef151b134dd938dbaad2cd8eb403bc)

改善後

[![Image from Gyazo](https://i.gyazo.com/e544a015064c725697bb21433572354f.png)](https://gyazo.com/e544a015064c725697bb21433572354f)

## 4-6. 宣言をブロックにまとめる

## 4-7. 段落に分割する

## 4-8. 個人的な好みと一貫性

## 4-9. まとめ
