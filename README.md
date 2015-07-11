# forge_form

## これは何？

- formのaction, method, パラメータを設定できます
- 自分で作ったサイトに対してのCSRF及び連打対策の確認を想定したものです

## 使い方

- add input? にnameを記述しaddボタンを押下でinput要素(type=file)を配置出来ます
- add hidden? にnameとvalueを記述しaddボタンを押下でパラメータを設定出来ます
- intervalに実行間隔を設定出来ます(ms)
- exec-cntに実行回数の指定が出来ます(最大100回まで※default)
 - exec-cntのMAX値はFF.Config.MAX\_EXEC\_CNT の値を変えれば変更可能です

## 例

- intervalの間隔でexec-cnt数、action_url先にパラメータを送信します
- デフォルトはintervalが1、exec-cntが1なので
  - 1ms後に1回だけaction_url先にパラメータを送信します
- intervalに100、exec-cntを10に設定すると
  - 100ms間隔で10回、action_url先にパラメータを送信します

## License

* MIT License

### ツールの使用は用量・用法を守って自己責任でお願いします