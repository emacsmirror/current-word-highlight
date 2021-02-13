# current-word-highlight-mode.el

## TODO
- [x] face指定がうまくいってない。deffaceで定義したものを使いたい。add-text-propertyがよくない感じか？
- [x] faceを消すとき、undoの履歴に残ってしまう -> overlayを使うことによりクリア
- [x] なんか遅い
- [x] 初回の実行が失敗する(最初にdelete-overlayするが、最初はないので)
- [x] 日本語入力のときおかしい。2語分先を差している？重要な目的の一つなのに…。
- [x] カーソル外のwordのときは、表示しないようにした。
- [x] ~括弧にカーソルが当たったときにsexpを選択するようになっていない。(easy-mark-word)と揃えたい → 次のwordを示すように。一応移動先の情報としては正しい。選択のときに一致しないが。問題はeasy-mark-wordをほかからうまく利用する方法がわからないためだ。これができればもっと統一された機能になる。このハイライトはeasy-mark-wordと深く結びついている。~
- [ ] もっといいword指定のやり方はないのか？最初のforward-wordなどださい。easy-mark-wordができれば…
- [ ] カーソルが消えずに残ってしまうときがある。とくにmagitを開いたときに発生するような。magitがすべてハイライトされ、元に戻ると消えないoverlayが発生している。割と致命的。
- [ ] カーソル外のwordのとき、前後のwordをハイライトするようにする。(現在は何もハイライトしないようにしている)
