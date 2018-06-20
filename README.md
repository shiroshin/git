gitのあれこれ
# add
git add [ファイル名]<br>
ワイルドカード使用可能<br>
## ファイル形式指定

git add *.md<br>

複数指定も可能<br>
git add *.md *.c *.java<br>

## ディレクトリ指定
git add [ディレクトリ名]<br>

複数指定可能
git add docs iib<br>

.を指定するとカレントディレクトリ以下のすべての変更がaddされる  
git add .  

## オプション
### -A --all  
git管理内のすべての変更がaddされる．カレントディレクトリが先頭のディレクトリでなくても良い.  
新規追加，削除したファイルもすべてaddされる．  
git add -A  
git add --all  

### -u --update
既にgit内にあるファイルのみで，変更があった場合のみaddする．  
git add -u  
git add --update  

### -p --patch
ファイルすべてをaddするのではなく，ファイル内でaddしたい部分を自分で選択しながらaddすることができる．  
addするか尋ねられるときがある，yでaddし，nでaddしない  ．
git add -p -A  
git add . --patch  

### -n --dry-run
**このオプションを付けて実行しても実際にはaddされない**  
どのファイルがaddされるか一覧で見ることができる  
git add -n -A  
git add . --dry-run  
### -f --force
.gitigonoreにかかれている管理対象外のファイルも強制的にaddする．  
オプションの前後のどちらかにどのファイルをaddするか記述が必要．  

git add -f -A
git add . --force

# clone
現在いるディレクトリにリポジトリをcloneする<br>
git clone [リポジトリ名]<br>
ディレクトリを指定したい場合<br>
git clone [リポジトリ名] [ディレクトリ名]<br>
特定のブランチだけを取ってくる<br>
git clone -b [ブランチ] --single-branch [リポジトリ名]


