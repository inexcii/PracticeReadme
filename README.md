### 課題
フォートビューワの中にユーザが選択した一枚フォートの内容に関してユーザが見なくても自動解析してくれる

### 解決
オンラインサービス「Imagga」のAPIを利用して実現できた

### アピールポイント
- CocoaPodsを利用してthird-party ライブラリを組み込む
- API通信は`Alamofire`で、画像の非同期処理は`AlamofireImage`で、JSONハンドリングは`SwiftyJSON`というライブラリを利用すること
- 画像認識はオンラインサービス[Imagga](https://imagga.com/)を利用すること

