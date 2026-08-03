# Cornixのキーマップ

## pdf出力の手順

- `Vial Web`上で、`File > Save current layout`をして`vil`ファイルを出力する
- [Cornixhub/キーマップ](https://cornixhub.com/keymap)に出力した`vil`ファイルをアップロードする
- `印刷`を押して、`pdfとして保存`する。

## png出力の手順

```bash
pdftoppm -png -r 300 layout.pdf layer
```
