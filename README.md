nendSDK-cocos2d-x Sample Project
==================
## Overview
cocos2d-xでNendSDKを利用するサンプルプロジェクトになります。  

## Requirement

* cocos2d-x-3.6

* nendSDK Cocos2d-x module ver1.2.0

## Usage
nendの管理画面からcocos2d-xモジュール 3.x用をダウンロードし、以下の手順でプロジェクトにSDKとモジュールの追加及び設定を行ってください。

### iOS  

### 1 NendSDK の組み込み
[組込み方法](https://github.com/fan-ADN/nendSDK-cocos2d-x/wiki/組込み方法) で以下の内容に読み替えてください。

1. プロジェクトに NendSDK 追加  
FinderでCocosNendSample/proj.ios_mac/ios のディレクトリに、NendModuleに内包しているNendSDKのNendAdフォルダごと追加します。  
2. 必須フレームワークの追加を行う  
本サンプルではこの手順は不要です。

### 2 cocos2d-x モジュールの組み込み
[組込み方法](https://github.com/fan-ADN/nendSDK-cocos2d-x/wiki/組込み方法) の説明に従って行ってください。


### 3 XcodeでプロジェクトをCleanしてRunする。

### Android  
事前にEclipse環境でcocos2d-x-3.6のセットアップが完了している必要があります。

1. Eclipse > File > Import > Android / Existing Android Code Into Workspace  
ダウンロードしたCocosNendSampleのproj.androidをインポートする。

2. インポートしたCocosNendSampleを右クリック > Properties > Android > Library  
参照がエラーになっているcocos2dxの項目を一旦Removeする。  
Add...をクリックし、Eclipseにインポート済みのlibcocos2dxを選択する。  

### 1 SDK の組み込み
1. jar ファイルの追加  と 2. Google Play services の追加  
[組込み方法](https://github.com/fan-ADN/nendSDK-cocos2d-x/wiki/組込み方法) の説明に従って行ってください。  
この時点で、google-play-services_libとlibcocos2dxのLibraryプロジェクトへの参照が有効になっている必要があります。

3. マニフェスト設定を行う  
本サンプルではこの手順は不要です。

### 2 cocos2d-x モジュールの組み込み
[組込み方法](https://github.com/fan-ADN/nendSDK-cocos2d-x/wiki/組込み方法/) の説明に従って行ってください。

### 3 ビルドの設定変更 と 4 AppActivity.java の編集
本サンプルではこの手順は不要です。


### EclipseでプロジェクトをCleanしてRunする。  
   または、ターミナルからproj.androidディレクトリに移動し、
   ```
   $ cocos compile -p android
   ```
   を実行後、EclipseでプロジェクトをCleanしてRunする。
