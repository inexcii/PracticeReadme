
# SDK導入ガイド

## Objective-C言語で作成されたアプリの場合

1. SDK(UAEInStreamAds.frameworkファイル)をプロジェクトに追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/add_drag_and_drop.png)
1. 「Copy items if needed」をチェックして「Finish」を押す
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/add_options.png)
1. SDKがLinkされたことを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/link_confirm.png)
	- Linkされていない場合手動で追加する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/link_no_sdk_add.png)
	- ローカルディスクにあるSDKを選択して「Open」を押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/link_no_sdk_confirm.png)
1. 「Build Phases」でBundle Resourcesを追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/bundle_add.png)
	- プロジェクトに追加したSDKを選択して「Add」を押す　　　　　　　　　　　　　
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/bundle_choose.png)
	- SDKがBundleに追加されたことを確認する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/bundle_confirm.png)
1. SDKの「Header Search Paths」設定で `$(PROJECT_DIR)/UAEInStreamAds.framework/Headers` を指定する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/path_settings.png)
1. SDKクラスをソースコードにインポートしてビルドが通ることを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/class_import_success.png)


## Swift言語で作成されたアプリの場合


