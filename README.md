# 頂点カラーの.objファイルをBlenderのversion2.79にインポートするの備忘

## 本家はこちら

https://blender.stackexchange.com/questions/90890/how-to-display-and-use-vertex-color-from-obj-model

### でこのままだとimportするとなんちゃらエラー




# __init__.pyの142行目をコメントアウト




### あとは普通にimport

FILE → import → Wavefront(.obj) →　インポートするobj選択

インポートされたオブジェクトを選択して３Dビューの左下のリスト

「Object Edit Mode」→「Vertex Paint」

へ変更です。

### コメントアウトしてしまったので、なにか他のobjフォーマット読み込めなくなってる可能性大ですよね。（バックアップは取りましょう）
