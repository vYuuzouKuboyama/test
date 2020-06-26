<html>
	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width">
		<link rel="stylesheet" href="../resources/css/default.css"></link>
	</head>
	<body>
		<div>
			<h1>はじめに</h1>
			<p>
				本手順は、SJFの開発環境を構築するまでの手順となります。<br>
				以下に記載された各事項を実施ください。<br>
				<br>
				　<a href="#1">１．Git for Windowsのインストール</a><br>
				　<a href="#2">２．GitHub上のSJFリポジトリのクローン</a><br>
				　<a href="#3">３．JDKのインストール</a><br>
				　<a href="#4">４．Apache Mavenのインストール</a><br>
				　<a href="#5">５．Eclipseのインストール</a><br>
				　<a href="#6">６．EclipseへのSJFパッケージのインポート</a><br>
				<br>
			</p>
		</div>
		<div>
			<h1>
				<a name="1">
					１．Git for Windowsのインストール
				</a>
			</h1>
			<p>
				【前提】<br>
				　○　バージョンは最新のバージョンを使用するものとする。<br>
				　○　インストール手順は<a href="https://weblabo.oscasierra.net/install-maven-36-windows/" target="_blank">こちらのリンク先</a>の手順に従うものとする。<br> 
				<br>
				【手順】<br>
				　①　<a href="https://gitforwindows.org/" target="_blank">こちらのリンク先</a>より、Git for Windowsのインストーラーをダウンロードする。<br>
				　②　①でダウンロードしたインストーラーを実行し、インストーラーに従ってインストールする。<br>
				　　　インストール先フォルダは、特に理由がない限りはデフォルトにする。<br>
				　③　Windowsスタートメニューより、「Git Bash」を起動する。<br>
				　④　Git Bashのコンソールで「git --version」と入力しEnterキーを押下する。<br>
				　　　バージョンが「2.27.0」であることを確認する。<br>
				<br>
				　　　　OIR-47943643+veriuser@oir-47943643 MINGW64 ~<br>
				　　　　$ git --version<br>
				　　　　git version 2.27.0.windows.1<br>
				<br>
				　以　上<br>
				<br>
			</p>
		</div>
		<div>
			<h1>
				<a name="2">
					２．GitHub上のSJFリポジトリのクローン
				</a>
			</h1>
			<p>
				【手順】<br>
				　①　Windowsスタートメニューより、「Git Bash」を起動する。<br>
				　②　Git Bashのコンソールで、cdコマンドでリポジトリのクローン先のフォルダに移動する。<br>
				　　　（以下コマンドの場合、Cドライブのsjfフォルダ配下に移動）<br>
				<br>
				　　　　OIR-47943643+veriuser@oir-47943643 MINGW64 ~<br>
				　　　　$ cd /C/sjf<br>
				<br>
				　③　Git Bashのコンソールで、「git clone https://github.com/Veriserve/selenium-java-framework.git」と入力し、Enterキーを押下する。<br>
				　　　実行途中でGitHubアカウント・パスワードの入力を求められるので、自身のアカウント情報を入力する。<br>
				<br>
				　　　　OIR-47943643+veriuser@oir-47943643 MINGW64 /C/sjf<br>
				　　　　$ git clone https://github.com/Veriserve/selenium-java-framework.git　　　　　　Cloning into 'selenium-java-framework'...<br>
				　　　　remote: Enumerating objects: 542, done.<br>
				　　　　remote: Counting objects: 100% (542/542), done.<br> 
				　　　　remote: Compressing objects: 100% (300/300), done.<br>
				　　　　remote: Total 542 (delta 225), reused 536 (delta 220), pack-reused 0<br>
				　　　　Receiving objects: 100% (542/542), 13.35 MiB | 4.63 MiB/s, done.<br>
				　　　　Resolving deltas: 100% (225/225), done.<br>
				　　　　Updating files: 100% (73/73), done.<br>
				<br>
				　以　上<br>
				<br>
			</p>
		</div>
		<div>
			<h1>
				<a name="3">
					３．JDKのインストール
				</a>
			</h1>
			<p>
				【前提】<br>
				　○　バージョンは「Java SE 8 Update 221」を使用する<br>
				　　　（個別に入手すること。）<br>
				<br>
				【手順】<br>
				　①　JDKのインストーラーを実行し、インストーラーに従ってインストールする。<br>
				　　　インストール先フォルダは、特に理由がない限りはデフォルトにする。<br>
				<br>
				　以　上<br>
				<br>
			</p>
			<h1>
				<a name="4">
					４．Apache Mavenのインストール
				</a>
			</h1>
			<p>
				【前提】<br>
				　○　バージョンは「apache-maven-3.6.1」を使用し、Teamsのフォルダにインストーラーをあらかじめ用意しておくものとする。<br>
				　○　インストール手順は<a href="https://weblabo.oscasierra.net/install-maven-36-windows/" target="_blank">こちらのリンク先</a>の手順に従うものとする。<br>
				<br>
				【手順】<br>
				　①　<a href="https://weblabo.oscasierra.net/install-maven-36-windows/" target="_blank">こちらのリンク先</a>の手順１～４の手順に従ってインストール・インストール確認する。<br>
				<br>
				　以　上<br>
				<br>
			</p>
			<h1>
				<a name="5">
					５．Eclipseのインストール
				</a>
			</h1>
			<p>
				【前提】<br>
				　○　バージョンは最新のバージョンを使用するものとする。<br>
				　○　インストール手順は<a href="https://proengineer.internous.co.jp/content/columnfeature/7853" target="_blank">こちらのリンク先</a>の手順に従うものとする。<br>
				<br>
				【手順】<br>
				　①　<a href="https://proengineer.internous.co.jp/content/columnfeature/7853#section201" target="_blank">こちらのリンク先</a>の手順に従ってインストールする。<br>
				　　　　2. Eclipseのダウンロードとインストール方法<br>
				　　　　3. Eclipseの日本語化<br>
				<br>
				　以　上<br>
				<br>
			</p>
			<h1>
				<a name="6">
					６．EclipseへのSJFパッケージのインポート
				</a>
			</h1>
			<p>
				【手順】<br>
				　①　Eclipseを起動する。<br>
				　②　メニューバーより「ファイル」→「インポート」を選択<br>
				　③　「一般」→「フォルダーまたはアーカイブからプロジェクト」を選択し、「次へ」をクリック<br>
				　④　「インポート・ソース」に、GitHub上のSJFリポジトリのクローンの手順でクローンしたフォルダ配下の<br>
				　　　「seleniumu-java-framework」フォルダを入力し、「完了」ボタンをクリックする。<br>
				　　　C:\sjf\selenium-java-framework<br>
				<br>
				【動作確認_SJFデモのデバッグ実行】<br>
				　①　「src/test/java」→「testClass」→「SampleTestClass.java」を選択。<br>
				　②　38行目の「test_01」を右クリックし、「実行」→「JUnit」を選択。<br>
				　　　ChromeでベリサーブのHPが表示され、各種ページが自動的に遷移されることを確認する。<br>
				<br>
				　以　上<br>
				<br>
			</p>
		</div>
	</body>
</html>