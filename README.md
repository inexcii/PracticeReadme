
# SDK導入ガイド

- [Objective-C言語で作成されたアプリの場合](#objective-c言語で作成されたアプリの場合)
- [Swift言語で作成されたアプリの場合](#swift言語で作成されたアプリの場合)


## Objective-C言語で作成されたアプリの場合

1. SDK(UAEInStreamAds.frameworkファイル)をプロジェクトに追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/add_drag_and_drop.png)
1. 「Copy items if needed」をチェックして「Finish」ボタンを押す
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/add_options.png)
1. SDKがリンクされたことを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/link_confirm.png)
	- リンクされていない場合に手動で追加する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/link_no_sdk_add.png)
	- ローカルディスクにあるSDKを選択して「Open」ボタンを押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/link_no_sdk_confirm.png)
1. 「Build Phases」タグでBundle Resourcesを追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/bundle_add.png)
	- プロジェクトに追加したSDKを選択して「Add」ボタンを押す　　　　　　　　　　　　　
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/bundle_choose.png)
	- SDKがBundleに追加されたことを確認する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/bundle_confirm.png)
1. SDKが 「Build Settings」タグの _Header Search Paths_ 設定で `$(PROJECT_DIR)/UAEInStreamAds.framework/Headers` を指定する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/path_settings.png)
1. SDKクラスをソースコードにインポートしてビルドが通ることを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/objc/class_import_success.png)


## Swift言語で作成されたアプリの場合

1. SDK(UAEInStreamAds.frameworkファイル)をプロジェクトに追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/1_1_add_drag_and_drop.png)
	- 「Copy items if needed」をチェックして「Finish」ボタンを押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/1_2_add_options.png)
1. SDKがリンクされたことを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/2_1_link_confirm.png)
	- リンクされていない場合に手動で追加する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/2_2_link_no_sdk_add.png)
	- ローカルディスクにあるSDKを選択して「Open」ボタンを押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/2_3_link_no_sdk_confirm.png)
1. SDKが「General」タグの _Embedded Binaries_ で設定されたことを確認して、なかった場合に追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/3_1_binaries_add.png)
	- 追加されたことを確認する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/3_2_binaries_confirm.png)
1. 「Build Phases」タグでBundle Resourcesを追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/4_1_bundle_add.png)
	- プロジェクトに追加したSDKを選択して「Add」ボタンを押す　　　　　　　　　　　　　
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/4_2_bundle_choose.png)
	- SDKがBundleに追加されたことを確認する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/4_3_bundle_confirm.png)
1. SDKが「Build Settings」タグの _Header Search Paths_ 設定で `$(PROJECT_DIR)/UAEInStreamAds.framework/Headers` を指定する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/5_1_path_settings.png)
1. Umbrella Headerファイルの新規作成と設定
	- Xcodeでプロジェクトファイルを右クリックして、「New File」を選択する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/6_1_header_file_new.png)
	- _iOS_ タグの下にある _Header File_ タイプを選択して「Next」ボタンを押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/6_2_header_file_choose.png)
	- ファイル名は `{プロジェクト名}-Bridging-Header.h` にして、「Create」ボタンを押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/6_3_header_file_naming.png)
	- 「Build Settings」タグの _Objective-C Bridging Header_ 設定で先ほど作成したHeaderファイル名を入力する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/6_4_header_settings.png)
	- Headerファイルを開いて組み込むSDKのクラスをインポートする
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/6_5_header_import.png)
1. 実装クラスでSDKを利用してビルドが通ることを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmeImages/swift/7_1_class_import_success.png)
