
# SDKをアプリに導入

## Objective-C言語で作成したプロジェクト

1. SDK(UAEInStreamAds.frameworkファイル)をプロジェクトに追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/add_drag_and_drop.png)
1. 「Copy items if needed」をチェックして「Finish」を押す
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/add_options.png)
1. FrameworkがLinkされたことを確認する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/link_confirm.png)
	- Linkされていない場合手動で追加する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/link_no_sdk_add.png)
	- ローカルディスクにあるFrameworkを選択して「Open」を押す
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/link_no_sdk_confirm.png)
1. 「Build Phases」でBundle Resourcesを追加する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/bundle_add.png)
	- プロジェクトに追加したFrameworkを選択して「Add」を押す 
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/bundle_choose.png)
	- FrameworkがBundleに追加されたことを確認する
	![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/bundle_confirm.png)
1. Frameworkの「Header Search Paths」を設定する
![image](https://github.com/inexcii/PracticeReadme/blob/master/ReadmePics/path_settings.png)



## Swift言語で作成したプロジェクト


