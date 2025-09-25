# English part



# Getting Started

Welcome to your new project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`package.json` | project metadata and configuration
`readme.md` | this getting started guide


## Next Steps

- Open a new terminal and run `cds watch`
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start adding content, for example, a [db/schema.cds](db/schema.cds).


## Learn More

Learn more at https://cap.cloud.sap/docs/get-started/.


#

## Japanese part

これはCAPで簡単にHANA Cloudに対しデータベース及び内部のテーブルを作成し、ODataとして公開するためのCAPプロジェクトのテンプレートです。
SAP Business Application StudioもしくはSAP Build Codeでの使用を想定しています。

# 使用方法
※BAS/Build Codeにこのプロジェクトをインポートしていることが前提です。インポートするまでは下記ブログを参照してください。

詳しくはこちらのブログでも解説しています。

1.まず、開発するプロジェクト名（このプロジェクトでは＝データベースの名称）を決めてください。ややこしくしないために半角小文字と数字だけを使用してください。
　以下の例ではtestdb1としています。
2.BAS/Build Code上でターミナルを開き、projectsディレクトリの下に移動します。projectsディレクトリにはインポートしたDBTemplateというディレクトリが存在するはずです。
3.DBTemplateディレクトリを丸ごと別名でコピーします。
　cp -rf ./DBTemplate ./testdb1
4.3で作成したディレクトリに移動し、以下のコマンドでプロジェクトのファイル中で使用しているxxxxxxxxという文字列をプロジェクト名に全て置換します。
　cd testdb1
  grep -rlI 'xxxxxxxx' /path/to/dir | xargs sed -i -e 's/xxxxxxxx/testdb1/g'
5.BAS上にてFile->Open Workspace from 
ワークスペースに読み込ませます。


ダウンロードしたDB