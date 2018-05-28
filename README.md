# 練習リポジトリ
## 目標
- [ ] Gitの操作ができる
  - [ ] リポジトリをローカルに持ってくる: `git clone [リモートリポジトリのURL]`
  - [ ] branchの作成: `git branch [new branch]`
  - [ ] 変更ファイルをステージングエリアに移動: `git add [path/to/file]`
  - [ ] ステージングエリアの変更をツリーに移動: `git commit -m "write your changes"`
  - [ ] ツリーの変更をリモートリポジトリに反映: `git push`
  - [ ] Github上でpull requestを送る
- [ ] c#のコーディング、オブジェクト志向言語のコーディングを学ぶ

## 自分の作業ブランチを作成する
このセクションでは、githubからローカルにリポジトリを複製して、自分の作業ブランチを作成するところまで行う。  

### 手順
リモートリポジトリをローカルに持ってくるのは`git clone`コマンド。  
Githubのリポジトリ画面の右上のあたりに、`Clone or Download`ボタンがある。  
そこから、クローンするためのURLを取得できるので、コピーする。  
ターミナルから、今回のリポジトリを配置したいパスに移動し(`cd`コマンド)、`git clone https://github.com/y-kisse/lessons_with_csharp.git`を行う。  
例えば、`~/workspace/lessons_with_csharp/`となるように配置したい場合には、`cd ~/workspace`を実行して、カレントディレクトリを`~/workspace`にしてから、`git clone`を行う。  

リポジトリのクローンに成功したら、`git branch`コマンドを実行する。  
すると、現在のブランチが`master`であると表示されるはず。  
今回は`master`から派生した、`dev_arinaga`ブランチを作成する。  
`git branch dev_arinaga`でブランチを作成(この際の派生元ブランチは現在選択されている`master`ブランチとなる。)  
`git checkout dev_arinaga`で`dev_arinaga`ブランチに移動することができる。  

今回のセクションはここまで。  

## 最初のC#プロジェクトを作成