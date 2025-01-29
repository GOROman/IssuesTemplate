name: バグ報告 / サポート依頼
description: バグの報告やサポートを求める際のテンプレート
title: "[Bug] 簡潔なタイトルを記入"
labels: ["bug", "support"]
assignees: []

body:

- type: markdown
  attributes:
  value: |
  **以下の内容を簡潔に記入してください。** - **長文説明やお気持ち表明は不要** です。 - **再現に必要充分な情報** を提供してください。

- type: textarea
  id: environment
  attributes:
  label: ハード及びソフトの構成
  description: 例: OS のバージョン、ハードウェア (ESP32S3 など)、関連ソフトウェア
  placeholder: | - OS: Ubuntu 22.04 - ハードウェア: ESP32S3 - ソフトウェア: xxx v1.2.3
  validations:
  required: true

- type: textarea
  id: steps-to-reproduce
  attributes:
  label: 実施した内容
  description: 実施した手順を簡潔に箇条書きで記載
  placeholder: | 1. xxx を実行 2. yyy を設定 3. zzz を試す
  validations:
  required: true

- type: textarea
  id: actual-result
  attributes:
  label: 得られた結果
  description: 実際に発生した問題やエラーメッセージを記載
  placeholder: | - xxx というエラーが発生 - 期待通りに動作しない
  validations:
  required: true

- type: textarea
  id: expected-result
  attributes:
  label: 期待した結果
  description: 本来どうなるべきだったかを記載
  placeholder: | - xxx が動作する - yyy になる
  validations:
  required: true

- type: textarea
  id: additional-info
  attributes:
  label: その他の補足情報 (必要な場合のみ)
  description: 再現に必要なログやスクリーンショットがあれば添付
  placeholder: | - エラーログ:
  `      Error: xxx failed due to yyy
     ` - スクリーンショット:
  (ここに画像をドラッグ&ドロップ)
  validations:
  required: false
