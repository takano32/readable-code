# 4. 美しさ


優れたソースコードは目に優しい

* 読み手が慣れているパターンを意識する
* 似ているコードは似ていると分かるようにする
* 関連するコードはひとつのブロックにする


## 4-1. なぜ美しさが大切なのか？

美しくないと理解に時間がかかる

[![Image from Gyazo](https://i.gyazo.com/a06385e78f963d2146074374712659c7.png)](https://gyazo.com/a06385e78f963d2146074374712659c7)

[![Image from Gyazo](https://i.gyazo.com/92aa95e6dc262fd7123174d63dfc9d61.png)](https://gyazo.com/92aa95e6dc262fd7123174d63dfc9d61)

正解

[![Image from Gyazo](https://i.gyazo.com/b41f4838595044c20284f0e489da5ab1.png)](https://gyazo.com/b41f4838595044c20284f0e489da5ab1)

**プログラミングのほとんどの時間はコードを読む時間**

## 4-2. 一貫性のある簡潔な改行位置

TcpConnectionSimulator クラスのコンストラクタには 4 つの仮引数

1. 接続速度(Kbps)
2. 平均遅延時間(ms)
3. 遅延「イライラ」時間(ms) 4. パケットロス率(%)

改行の位置が悪い例

[![Image from Gyazo](https://i.gyazo.com/ccac44551deb21c0f29de02673b57223.png)](https://gyazo.com/ccac44551deb21c0f29de02673b57223)

改行の位置が良い例

[![Image from Gyazo](https://i.gyazo.com/bad34611acebf0f89d7b45b2318262c4.png)](https://gyazo.com/bad34611acebf0f89d7b45b2318262c4)

さらにコメントの冗長性を取り除いた例

[![Image from Gyazo](https://i.gyazo.com/7ea5033bff19df871f74b748c94de7b1.png)](https://gyazo.com/7ea5033bff19df871f74b748c94de7b1)

## 4-3. メソッドを使った整列

同一の処理がまとめられていないと読みにくい

[![Image from Gyazo](https://i.gyazo.com/9e232bd0217885e77d654e10f5966f55.png)](https://gyazo.com/9e232bd0217885e77d654e10f5966f55)

ヘルパーメソッドを作成して分かりやすくした例

[![Image from Gyazo](https://i.gyazo.com/223d3c2868fd938927f06fbd7ec82bd4.png)](https://gyazo.com/223d3c2868fd938927f06fbd7ec82bd4)


* 重複を排除したことでコードが簡潔になった。
* テストケースの大切な部分(名前やエラー文字列)が見やすくなった。以前 は、database_connection や error などのトークンに囲まれていて、コード を見て「飲み込む」のが難しかった。
* テストの追加が簡単になった。

**テストコードだからといって assert を連発すればよいというものではない**


## 4-4. 縦の線をまっすぐにする

先ほどの例

[![Image from Gyazo](https://i.gyazo.com/e54e57b195fce64397d04d7e6999fc62.png)](https://gyazo.com/e54e57b195fce64397d04d7e6999fc62)

表敬式のようにすると分かりやすい

[![Image from Gyazo](https://i.gyazo.com/c6c41ec4c3c17e3f098512189b12e678.png)](https://gyazo.com/c6c41ec4c3c17e3f098512189b12e678)

規則性をもたせると間違いも見つけやすい

[![Image from Gyazo](https://i.gyazo.com/d7405adb4f0951a4b4b0f2690f227ab7.png)](https://gyazo.com/d7405adb4f0951a4b4b0f2690f227ab7)

### 備考: プロダクトでの例

位置合わせ前

[![Image from Gyazo](https://i.gyazo.com/6b28664f58fe08e20679a499ba4aae67.png)](https://gyazo.com/6b28664f58fe08e20679a499ba4aae67)

位置合わせ後

[![Image from Gyazo](https://i.gyazo.com/a9a395cdfef93487b179d6ef2efd402e.png)](https://gyazo.com/a9a395cdfef93487b179d6ef2efd402e)


## 4-5. 一貫性と意味のある並び

## 4-6. 宣言をブロックにまとめる

## 4-7. 段落に分割する

## 4-8. 個人的な好みと一貫性

## 4-9. まとめ
