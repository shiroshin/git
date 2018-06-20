# git
gitのあれこれ
## add
git add [ファイル名]<br>
ワイルドカード使用可能<br>
### ファイル形式指定

git add *.md<br>

複数指定も可能<br>
git add *.md *.c *.java<br>

### ディレクトリ指定
git add [ディレクトリ名]<br>

複数指定可能
git add docs iib<br>

.を指定するとカレントディレクトリ以下のすべての変更がaddされる
git add .  

### オプション
#### -A --all  
git管理内のすべての変更がaddされる．カレントディレクトリが先頭のディレクトリでなくても良い．  新規追加，削除したファイルもすべてaddされる  
git add -A
git add --all


## clone
現在いるディレクトリにリポジトリをcloneする<br>
git clone [リポジトリ名]<br>
ディレクトリを指定したい場合<br>
git clone [リポジトリ名] [ディレクトリ名]<br>
特定のブランチだけを取ってくる<br>
git clone -b [ブランチ] --single-branch [リポジトリ名]


