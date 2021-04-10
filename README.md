# msfs-hiddenui-enhance

## あらすじ

MSFSのマルチプレイ等で、他のプレイヤー名やAI機の機体番号を非表示にしたい場合は、
オプションの `SHOW TRAFFIC NAMEPLATES` をOFFにする必要があります。

しかしONとOFFの切り替えのためにはポーズが必要なので、
飛行しながらシームレスに切り替えることは現状ではできません。(※2021年4月時点)

そこで、飛行しながらでも簡単に切り替えるためのMODが公開されていたので、その導入方法のメモです。

そのままMODを導入するだけだとUIがだいぶ斬新になってしまうので、デフォルトっぽい見た目に戻すためのファイルも併せて公開します。

---

## 導入方法

1. 「[UI mods and tweaks (full pack)](https://flightsim.to/file/3530/ui-mods-and-tweaks-full-pack)」をダウンロード

2. 「[uimod]-mugz-hiddenui」「[uimod]-mugz-tinyplates」の2つをCommunityフォルダに入れる
> ※両方導入しないと正常に動作しない

3. (見た目を元通りのスタイルに戻したい場合は)下記のファイルを差し替え
> [uimod]-mugz-tinyplates\html_ui\mCSS\mugzIGMAT.css
* [差し替え用ファイル](https://raw.githubusercontent.com/berry1225/msfs-hiddenui-enhance/main/mugzIGMAT.css)
* * ※ `mugzIGMAT.css` として保存後に置換、もしくは内容を丸ごとコピーして元ファイルを全行書き換え

---

## 使い方

* オプションの `SHOW TRAFFIC NAMEPLATES` はON
* キーボードの `BackSpace` を押すと非表示、もう1回で再表示
* * `F12` や `NumLock` でも可能、ファイル弄ればキーアサイン変更もできるらしい

---

## メモ

* CSSなので頑張れば他要素も色々変えることができる
* フォントを変えようとしたら日本語が豆腐化、そもそもの指定も効いてない気がする
* * →webfont形式とかで読み込まないといけない？

---

## 各種環境
* 確認時のMSFSバージョン：v1.14.5.0
* 確認時のMODバージョン：v1.12.13.0
* 画面解像度：1920x1080 スケール100% (margin指定がpxなので、別環境だと影響出るかもしれない？)

---
