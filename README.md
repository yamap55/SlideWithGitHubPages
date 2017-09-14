# SlideWithGitHubPages
Markdownでスライド書いて、自分のGitHubで管理して、自分のGitHub Pagesで表示します。

## Description
- Slideを作る際に、Markdownで書いて自分のGitHubで管理するして、自分のGitHub Pagesで表示できます
  - reveal.js version 3.5.0を使用（[index.html](https://raw.githubusercontent.com/hakimel/reveal.js/a6ecbfa73272977d04e107f878a6afbfd17c6869/index.html)でリクエストパラメーターで渡されたスライドを表示できるようにしただけ）
- 通常、reveal.jsを使用する場合、毎回HTML部が必要となりますが、リクエストパラメーターでMarkdownのパスを指定すればスライドが表示されるようにしています

## Demo
- http://yamap55.github.io/SlideWithGitHubPages/index.html?slide=example/slide1.md
- http://yamap55.github.io/SlideWithGitHubPages/index.html?slide=example/slide2.md

## Usage
### initialize
- git clone or fork
- プロジェクトのsettings
- [GitHub Pagesとして公開](https://www.google.com/search?q=github+pages)
- 以下にアクセス
  - http://${userId}.github.io/${repositoryName}/index.html?slide=example/slide1.md

### add slide
- Markdownでスライドを書く
  - 書き方は[検索](https://www.google.com/search?q=revelal.js+markdown)するか、[サンプル](https://raw.githubusercontent.com/yamap55/SlideWithGitHubPages/master/example/slide1.md)見てください。
- GitHubにpush
- 以下にアクセス
  - http://${userId}.github.io/${repositoryName}/index.html?slide=${markdownPath}

### print-pdf
- URL末尾に「&print-pdf」を付与して表示。
  - 例 : http://yamap55.github.io/SlideWithGitHubPages/index.html?slide=example/slide1.md&print-pdf
- ブラウザの印刷設定
- PDFに保存、横向き、背景のグラフィックにチェック
- 保存

## Notes
- GitHub Pagesなので更新が遅い場合があります
  - ブラウザにキャッシュされている場合もある（キャッシュクリアや別ブラウザ、シークレットモードなどで確認）
- 古いブラウザは考慮していません
- オフラインでは見れません
