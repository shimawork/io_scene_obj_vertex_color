# 頂点カラーの.objファイルをBlenderのversion2.79にインポートするの備忘

## 本家はこちら

https://blender.stackexchange.com/questions/90890/how-to-display-and-use-vertex-color-from-obj-model

### でこのままだとimportするとなんちゃらエラー

    Traceback (most recent call last):
      File "/Applications/Blender/blender.app/Contents/Resources/2.79/scripts/addons/io_scene_obj/__init__.py", line 148, in execute
        return import_obj.load(context, **keywords)
    TypeError: load() got an unexpected keyword argument 'use_cycles'
    
    location: <unknown location>:-1







# で、__init__.pyの142行目をコメントアウト

### あとは普通にimport

FILE → import → Wavefront(.obj) →　インポートするobj選択

インポートされたオブジェクトを選択して３Dビューの左下のリスト

「Object Edit Mode」→「Vertex Paint」

へ変更です。

### コメントアウトしてしまったので、なにか他のobjフォーマット読み込めなくなってる可能性大ですよね。（バックアップは取りましょう）
