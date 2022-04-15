# InteractiveValueResources
・Resources、css、js　フォルダはリソースファイルです。
・InteractiveValueAndCubism-qua2-0414.zip　はリソースファイルを作成するために使用したプロジェクトを圧縮した物です。

説明文------------
・webpackというnpmのライブラリを用いて、複数のtypescriptファイルを一つのjavascriptファイルに変換した「js/SectionOmote.js]をquartricsに取り込んで使っています。そのため実際のプロジェクトは上記の「InteractiveValueAndCubism-qua2-0414.zip」を展開してもらえば見れると思います（展開した　src/templates/index.html と src/indexApp/SectionOmote.ts がプログラムの開始位置です）。
（webpack参考：https://ics.media/entry/16329/）

・qualtrics上の埋め込みJavadcriptでは、githubからjsファイルをダウンロードして実行するという処理をしています。「js/SectionOmote.js」が主にqualtricsにダウンロードしているJavascriptの本体です。他の画像ファイルとjsonファイルもgithub上においてあり、qualtricsで取り込んで利用しています。これはwebpackによる変換後のjsファイルを直接qualtricsに貼り付けても無効なJavascriptとして認識されるためです
（参考：https://kscscr.com/archives/jspsych-qualtrics-r.html#:~:text=%E3%82%A2%E3%83%89%E3%83%AC%E3%82%B9/%E3%83%95%E3%82%A9%E3%83%AB%E3%83%80%E5%90%8D/%22%22%3B-,var%20requiredResources%20%3D%20%5B,%C2%A0%C2%A0%C2%A0%C2%A0%7D,-if%20）。

・ただgithubのjsファイルは直接実行できないので「jsdeliver」というものでurlを変換しています（参考：https://rs-techdev.com/archives/4318）
