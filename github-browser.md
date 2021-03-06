
## ブラウザだけからGitHub Pagesでサイトを作って更新する方法
GitHub Pagesは無料で(markdownの)サイトを作れる便利なサービスだが、ネットで日本語の情報を探してもパソコンから操作する技術者向けの説明が多い。だから、私のようなスマホやタブレットだけでGitHub Pagesを使おうとする酔狂な人間は細かい点で苦労してしまった。そこでネットの日本語の情報では欠けている、ブラウザからGitHub Pagesを使う方法をここでまとめることにした。


ここでの目的はGitHub Pagesでmarkdownを用いたファイルを公開できるようになることです。
### GitHubにアカウントを作ってレジストリを作成するまで
ブラウザからGitHubにサイトを作成する方法を書いた便利な記事があるので、とりあえずはそっちを見てください。

**[自分で作ったWebページをインターネット上に公開しよう！](https://prog-8.com/docs/github-pages)**

とりあえず「アカウント名.github.io」のレジストリを作りましょう。ちなみに、レジストリは削除も名前の変更も後からsettingからできます。
ただし、レポジストリ作成時に「initialize the repository with a README」をチェックしておくと、markdownのREADMEのファイルを自動で作ってくれて、indexファイルに代わりに表紙のサイトになってくれる。	ここでの目的にはその方が都合が良い。
### レジストリ専用ページの使い方
レジストリを作成すると、その後にレジストリ専用のページが表示されるはずです。おそらく上部にある幾つかのタブからcodeが選択された状態になるはずです(押せば選択できます)。

ここからもさっきリンクした記事にファイルのアップロードの仕方が説明されているので、それを見てください。codeタグから「Create new file」ボタンを使えば、ブラウザから簡単にファイルを作成できます。この作業はこれからサイトを運営する上で何度も使うので絶対に覚えてください。READMEファイルがあるならそれでもいいのですが、ファイル名にmarkdown用の拡張子mdをつけた`index.md`を作っても構いません(表紙にはindexファイルが優先されます)。

ファイルの編集もいつでもできて、リンク記事の第六節にあるように、codeからファイル名を選んで鉛筆じるしを押すだけです。ファイルの削除も鉛筆じるしの隣のゴミ箱じるしを押すだけです。
### 設定から公開されたサイトを確認する

これまたリンクした記事の第五節を見てください。レジストリ専用ページのsettingタブはいろんな大事なことができるところです。公開サイトのアドレスの確認だけでなく、サイトのデザイン変更やレジストリの削除などもここから行なえます。

settingタグのGitHub Pagesの項目に公開サイトのアドレスが表示されるが、その下の方のTheme chooserにある「choose the theme」ボタンを押すと、デザイン変更画面になり上からテーマを選んで右のボタンで決定すれば良い。ここまでは他の記事でも説明されているのが、困ったことにテーマに表示される文字の変え方は日本語ではどこにも書いてなかった。自分は以下の英語の記事を参考にした。

[Getting Started with GitHub Pages](https://guides.github.com/features/pages/)

codeタグから`_config.yml`を選んで編集する際に、`title: `や`description: `の後に表示させたい文字を入れた行を加えてから緑のcommitボタンを押せば、デザインに反映されます。
### 表紙以外のページを作る
これも何故か情報がないが、「Create new file」ボタンからそのまま拡張子付きファイルを作成すれば新しいページが簡単に作れます。その際、その新しいページは表紙のURLの後ろに/ファイル名をつけたURLに表示されるので、表紙のページからリンクを貼ろう。

ここではmarkdownの説明はしないが、GitHubも基本は一緒の記法だが、オリジナルの記法もあるので以下のリンクで確かめておこう。

[Mastering Markdown](https://guides.github.com/features/mastering-markdown/)


### ディレクトリの作り方
幾つかのファイルをまとめられるディレクトリは簡単に作れる。ファイルの編集画面でファイル名を入力・編集できるが、そのファイル名の入力枠に適当なディレクトリ名を打ち込んだ後にスラッシュ(`/`)を入れると、自動的にその名のディレクトリが作成されます。後は自由にファイルを作ろう。ディレクトリに入ってるファイルも公開サイトに変換されます。


続く？
