# Arduino 環境構築（Windows）

## Arduino IDE のダウンロード・インストール

1. [公式サイト](https://www.arduino.cc/en/software/)から最新バージョン（v2.3.6）をダウンロード
   <br>windows Win 10 and newer,64 bits を選択
   <br>寄付してください系の勧誘は JUST DOWNLOAD を選択
2. ダウンロードされたファイルを開く
3. ライセンス契約書に同意
4. インストールオプション、パスを設定
   <br>基本初期のままで OK
5. インストールを押す

## Aruduino CLI のダウンロード

1. [公式サイト](https://arduino.github.io/arduino-cli/1.1/installation/#download)から Windows exe 64bit をダウンロード
2. ダウンロードされた zip ファイルを解凍
3. C:\Program Files\ArduinoCLI\を作成
4. arduino-cli.exe を C:\Program Files\ArduinoCLI\ に移動
   <br>自分で分かりやすい場所に配置して OK
5. スタート → 環境変数と検索 → システム環境変数を編集を選択
6. 環境変数を選択（下の方）
7. 〇〇のユーザー環境変数の PATH という変数をダブルクリック
8. 新規を押す
9. C:\Program Files\ArduinoCLI\ を入力（自分でパス指定した際はそのパス）
10. 「OK」 → 「OK」 → 「OK」で閉じる
11. コマンドプロンプトを開いて以下を実行してバージョンが出れば OK

```bash
arduino-cli version
```

## VS Code での設定

- Arduino Community Edition という拡張機能をインストール
- Arduino Community Edition の設定を開く
- 以下の 3 点を変更

```json
{
  "arduino.clearOutputOnBuild": true,
  "arduino.enableUSBDetection": true,
  "arduino.useArduinoCli": true
}
```
