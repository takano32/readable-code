# 4. 美しさ


優れたソースコードは目に優しい

* 読み手が慣れているパターンを意識する
* 似ているコードは似ていると分かるようにする
* 関連するコードはひとつのブロックにする


## 4-1. なぜ美しさが大切なのか？

美しくないと理解に時間がかかる

[![Image from Gyazo](https://i.gyazo.com/a06385e78f963d2146074374712659c7.png)](https://gyazo.com/a06385e78f963d2146074374712659c7)

美しくした例

[![Image from Gyazo](https://i.gyazo.com/64ee47bc2ef8d3e71ad0b11cb413501f.png)](https://gyazo.com/64ee47bc2ef8d3e71ad0b11cb413501f)


**プログラミングのほとんどの時間はコードを読む時間**

## 4-2. 一貫性のある簡潔な改行位置

TcpConnectionSimulator クラスのコンストラクタには 4 つの仮引数

1. 接続速度(Kbps)
2. 平均遅延時間(ms)
3. 遅延「イライラ」時間(ms) 4. パケットロス率(%)

改行の位置が悪い例

[![Image from Gyazo](https://i.gyazo.com/602bcca8f4316e441710434795216664.png)](https://gyazo.com/602bcca8f4316e441710434795216664)


改行の位置が良い例


[![Image from Gyazo](https://i.gyazo.com/faf9e41053d3d8f91875e9e66f71c90d.png)](https://gyazo.com/faf9e41053d3d8f91875e9e66f71c90d)


さらにコメントの冗長性を取り除いた例

[![Image from Gyazo](https://i.gyazo.com/fe95a683f1e8806f02e0eb4c9bcec481.png)](https://gyazo.com/fe95a683f1e8806f02e0eb4c9bcec481)

## 4-3. メソッドを使った整列

同一の処理がまとめられていないと読みにくい


[![Image from Gyazo](https://i.gyazo.com/355b9cb87396a9d7787f71d9d7182813.png)](https://gyazo.com/355b9cb87396a9d7787f71d9d7182813)


ヘルパーメソッドを作成し処理をまとめて分かりやすくした例

[![Image from Gyazo](https://i.gyazo.com/f7ecb3a06e761ceef1537a0280b58fbd.png)](https://gyazo.com/f7ecb3a06e761ceef1537a0280b58fbd)

* 重複を排除したことでコードが簡潔になった。
* テストケースの大切な部分(名前やエラー文字列)が見やすくなった。以前 は、database_connection や error などのトークンに囲まれていて、コード を見て「飲み込む」のが難しかった。
* テストの追加が簡単になった。

**テストコードだからといって assert を連発すればよいというものではない**


## 4-4. 縦の線をまっすぐにする

先ほどの例

[![Image from Gyazo](https://i.gyazo.com/e54e57b195fce64397d04d7e6999fc62.png)](https://gyazo.com/e54e57b195fce64397d04d7e6999fc62)

表敬式のようにすると分かりやすい

[![Image from Gyazo](https://i.gyazo.com/eccc859452a4d3c8b1ac376f4eeb4333.png)](https://gyazo.com/eccc859452a4d3c8b1ac376f4eeb4333)

規則性をもたせると間違いも見つけやすい

[![Image from Gyazo](https://i.gyazo.com/fb7cf965a1ed6013efd54c4f855dffd6.png)](https://gyazo.com/fb7cf965a1ed6013efd54c4f855dffd6)

### 備考: プロダクトでの例

位置合わせ前

[![Image from Gyazo](https://i.gyazo.com/97664a7984773845a021a3d259625190.png)](https://gyazo.com/97664a7984773845a021a3d259625190)

位置合わせ後

[![Image from Gyazo](https://i.gyazo.com/e8b8681798d14ebc679db4d870683636.png)](https://gyazo.com/e8b8681798d14ebc679db4d870683636)

## 4-5. 一貫性と意味のある並び

## 4-6. 宣言をブロックにまとめる

## 4-7. 段落に分割する

## 4-8. 個人的な好みと一貫性

## 4-9. まとめ
