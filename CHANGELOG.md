# CHANGELOG

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
