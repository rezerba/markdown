#環境構築

- [テキストエディタを導入する](#sec1)
- [Package Controlをインストールする](#p2)
- [Markdownを使えるようにする](#p3)
- [実際に書いてみよう](#p4)

***


## <a id="sec1"></a> テキストエディタを導入する  
今回使用するのはSublime Textである。Versionが2, 3とあるが、今回はどちらを使用してもよい  

- [Sublime Text 2](http://www.sublimetext.com/2)
- [Sublime Text 3](http://www.sublimetext.com/3)

##<a id="p2"></a>Package Controlをインストールする  
下記のサイトに従ってPackage Controlをインストールしてください  

[恋に落ちる「Sublime Text」のインストール・日本語化](http://webmem.hatenablog.com/entry/sublime-text)

##<a id="p3"></a>Markdownを使えるようにする  
次にMarkdownを使えるようにするにあたり次のようなPackageをインストールしてください  

[マークダウンエディタとして使う方法](http://futago-life.com/sublime-text3-wiki/how-to/markdown)  
	上記のサイトから次のパッケージがインストールできます  

- OmniMarkupPreviewer  
- Monokai Extended  
- Markdown Extended  
- Trailing Space  
- Table Editor  

##<a id="p4"></a>実際に書いてみよう  
実際にMarkdownの記法を使ってみましょう  
参考:[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#headers)  



# 環境構築
OS毎にいくつかのインストール方法があるので、好きな方法で入れる。  

- [Windows](#p1)
- [Mac](#p2)
- [Linux](#p3)
- [インストール後](#p4)
- [GUIを使えるようにする](#p5)

---

## <a id="p1"></a> Windows
- [Git for Windows](https://git-for-windows.github.io)からインストーラーをダウンロードして、インストール
	- Bash OnlyがデフォルトなのでCommand Promptで使えるように選択しておいた方が良いらしい
	- その他設定はお好みで 
- [GitHub for Windows](http://windows.github.com)からインストーラーをダウンロードして、インストール

## <a id="p2"></a> Mac
- Xcode Command Line Toolsをインストール
- [Git](http://git-scm.com/downloads)からインストーラーをダウンロードして、インストール
- Homebrewを使用
```shell
$ brew install git
```

## <a id="p3"></a> Linux
自分のディストリビューションのパッケージ管理システムを使用してインストール。
#### Debian/Ubuntu
```shell
$ apt-get install git
```
#### Fedora
```shell
$ yum install git
```
#### Gentoo
```shell
$ emerge --ask --verbose dev-vcs/git
```
#### Arch Linux
```shell
$ pacman -S git
```
#### openSUSE
```shell
$ zypper install git
```
#### FreeBSD
```shell
$ cd /usr/ports/devel/git
$ make install
```
#### Solaris 11 Express
```shell
$ pkg install developer/versioning/git
```
#### OpenBSD
```shell
$ pkg_add git
```

## <a id="p4"></a> インストール後
コマンドライン上で以下を実行し、正しくversionが表示されればインストール完了。
```shell
$ git --version
```

#### ユーザ情報を設定
```shell
$ git config --global user.name "{user_name}"   # ユーザ名を登録
$ git config --global user.email "{email}"      # メールアドレスを登録
$ git config --global color.ui auto             # 出力をカラーリング(任意)

$ git config --list                             # 現在の設定を確認
```

##<a id="p5"></a> GUIを使えるようにする
gitをインストールするとgit gui/gitkというGUIツールが付いてくるが、これを使うくらいなら以下のクライアントを使ったほうが良いと思う。

- [SourceTree](https://ja.atlassian.com/software/sourcetree/overview)
- [GitHub Desktop](https://desktop.github.com)
- 他にもいろいろあるっぽい

