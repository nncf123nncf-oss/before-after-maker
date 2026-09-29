# CHANGELOG

## 0.1.1 - 2026-09-29

iPhone・iPadでPNGが保存できなかった問題を修正。

- 公開後、iPhoneのChromeで「PNGで保存」を押しても何も起きないことが判明した。
  iOSは `a.download` を無視し、data URLへの遷移も止めるため、初回実装の保存方法が働かなかった。
  iOSのChromeも中身はSafariと同じなので、ブラウザを変えても同じ結果になる
- iPhone・iPadでは共有シート（`navigator.share`）から保存する経路に変更
- 共有シートが使えない場合は、できあがった画像を画面に出して長押しで保存できるようにした
- PC（Windows・Mac・Android）は従来どおりダウンロードのまま

## 0.1.0 - 2026-09-15

初回リリース。

- Before画像・After画像の2枚選択（`input[type=file]`）
- canvasへの左右連結描画（`drawImage` の中央基準クロップ）
- ラベル帯（Before＝グレー地に白文字／After＝青地に紺文字）と中央区切り線の描画
- ラベルの日本語（ビフォー/アフター）／英語（Before/After）切替
- 正方形（1080×1080）／横長（1080×608）の2比率切替
- `canvas.toDataURL('image/png')` によるPNG保存
- 写真未選択時の赤文字1行エラー表示
- 運営者表記フッタ
