# Cornixのキーマップ

## 特徴

- レイヤー1: 記号レイヤー
  - 各種括弧を左右対称に配置：`<>[](){}`
  - Vimの行頭・行末移動（`^` / `$`）を左右対称に配置し、直感的に操作できるようにしている
- レイヤー2: ショートカットレイヤー
  - `hjkl` があった位置に方向キーを配置し、Vim風に操作できる
  - IMEの切り替えを左右対称に配置し、間違えにくく、覚えやすいようにしている
  - `LCA(key)` (Ctrl + Alt + key)でアプリを切り替える
    - b: ブラウザ
    - t: ターミナル
    - m: 音楽
  - アプリ切り替えの設定: [dotfiles/home-manager/hotkey/app.nix](https://github.com/mizunofukusayou/dotfiles/blob/main/home-manager/hotkey/app.nix)
- レイヤー3: 数字レイヤー
  - なるべくホームポジションから手を動かさずに数字を入力できるように配置
- レイヤー4: マウスレイヤー
  - Vim風の移動では斜め移動が苦手だったので、`wasd` 風の操作にしている
- レイヤー8・9: ゲーム用レイヤー
  - `DF(8)` でゲームモードに切り替える
- 親指キーの活用
  - レイヤーごとに異なる親指キーを割り当て、無駄なく使用
  - 親指キーの組み合わせでレイヤー5まで移動可能
  - AIチャットやSNSなどで使いやすいように `Shift + Enter` を用意
- 小指への負担を軽減
  - 極力、外側のL字部分のキーを使用しないようにしている

## pdf出力の手順

- `Vial Web`上で、`File > Save current layout`をして`vil`ファイルを出力する
- [Cornixhub/キーマップ](https://cornixhub.com/keymap)に出力した`vil`ファイルをアップロードする
- `印刷`を押して、`pdfとして保存`する。

## png出力の手順

```bash
pdftoppm -png -r 300 layout.pdf layer
```
