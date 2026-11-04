# CIF Completer

A single-file, browser-based tool that completes the `?` placeholders of a SHELXL-refined CIF with values from the diffractometer software's output, and builds Word tables for a paper's SI.
Everything runs in the browser; there is nothing to install.

**Use it:** [https://ken1yama.github.io/cif-completer/](https://ken1yama.github.io/cif-completer/) (Japanese / English switch at the top right)

## What it does

1. **Complete the CIF** – only items whose value is `?` are filled; existing values are never changed. A list shows which item was filled from which file.
   - Rigaku: `.cif_od` (or a `.cif` exported from CrysAlisPro)
   - Bruker: `.pcf` (XPREP), plus `.p4p` (colour / habit / size) and SADABS `.abs` (Tmin/Tmax) – the `.p4p` and `.abs` readers are **experimental**
   - Other makers: any CIF-format file
   - Crystal habit / colour, molecular graphics and publication-material software can be entered by hand.
2. **Edit** the result directly on the page.
3. **Check** with [checkCIF](https://checkcif.iucr.org/) (link button).
4. **Word tables** (.docx, Times New Roman): crystal data, atomic coordinates, bond lengths and angles, anisotropic displacement parameters, hydrogen coordinates, torsion angles and hydrogen bonds. Choose which tables to include.

Always run checkCIF on the final file.

## Run locally

Open `index.html` in a browser. It is a single self-contained file.

---

# CIF Completer（日本語）

SHELXL で精密化した CIF の `?` を、測定ソフトが出力したファイルの値で補完し、論文SI向けの Word の表を作るブラウザ用ツールです。インストール不要で、すべてブラウザ内で動きます。

使う: [https://ken1yama.github.io/cif-completer/](https://ken1yama.github.io/cif-completer/)（右上で日本語 / English を切り替え）

- 値が `?` の項目だけを埋めます。すでに入っている値は変更しません。
- Rigaku は `.cif_od`、Bruker は `.pcf`（加えて `.p4p`、`.abs` は試験的対応）、他社装置は CIF 形式のファイルを読み込めます。
- 補完後の内容は画面上で直接編集でき、checkCIF のページへのリンクがあります。
- 結晶データ、原子座標、結合長・結合角、異方性変位パラメータなどの表を .docx で出力できます。

## License

MIT © 2026 Ken-ichi Yamashita
