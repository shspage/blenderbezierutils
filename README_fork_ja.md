# [fork元](https://github.com/Shriinivas/blenderbezierutils) からの変更点
by [@shspage](https://github.com/shspage)


## ver.0.9.96+  -  2020.12.27

(fork元の変更を反映)

----

## ver.0.9.95+2  -  2020.12.17
### ハンドルスナップ機能に Vertex(頂点)モードを追加
パイメニューの項目 Selected Ends, Move Paths に、それぞれ _Vertexモード_ を追加しました。
Vertexモードでは、端点の移動先はベジェ曲線上の（数学的な）最近点ではなく、曲線をメッシュに変換した際に頂点になる点(※)のうちの最近点になります。

※：頂点の位置は曲線の解像度（BezierCurve > Shape > Resolution Preview）を元に決定しています。

----

## ver.0.9.95+1  -  2020.12.16
### ハンドルスナップ機能を追加  
選択されている _ベジェ曲線_ の端点を、最も近い _ベジェ曲線上_ に移動します。その際、ハンドルの角度を移動先での接線に合わせます。  
オブジェクトモードで(Flexi Edit Bezierツールで)端点を選択後、**Shift+S** で パイメニューが表示されますので、以下のいずれかを選んでください。

- **Selected Ends** : 選択端点を移動します。

- **Move Paths** : 端点を移動するとともに、移動分をパス全体に適用します。両方の端点が移動される場合、その他の点には移動分の平均が適用されます。

曲線上からズレるよ、という場合：曲線の解像度が不足しているかもしれません。BezierCurve > Shape > Resolution Preview の値を上げてみてください。

### retinaディスプレイ対応
文字サイズや線幅などの既定値に `bpy.context.preferences.system.ui_scale` を掛けています。
(対応としてこれが正解なのか確信なし。ご指摘頂けると助かります。)

----