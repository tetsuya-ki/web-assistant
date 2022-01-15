# Web Assistant

* Phil Nsah氏の"Speech to text in the browser"をもとに作成しました
* 機能
  * Discordに投稿中/しないボタン
    * 「Discordに投稿中」と表示されている状態で、後述のWebhook URLが入力されていれば、それを使ってDiscordに音声認識結果を投稿します
  * 音声認識に使う言語を選択
    * 日本語、英語から選ぶことができます
    * 変更した場合、一度音声認識を停止することを推奨します
  * 音声継続ON/OFFチェックボタン
    * 音声を継続して認識させるかどうか(デフォルトはONです)
    * 変更した場合、一度音声認識を停止することを推奨します
  * 結果編集ON/OFFボタン
    * 音声認識の結果が編集できるかどうか(デフォルトはOFFです)
    * 別に送信されるわけでもないので編集しても意味ないですが、音声認識の結果をちょろっと変えたいときに便利です
* 入力項目説明
  * 名前
    * 音声認識の左側にカッコ付きで記載されます
    * Discordに投稿する場合の名前にも使用されます
  * Webhook URL
    * Discordの[Webhook URL](https://support.discord.com/hc/ja/articles/228383668-%E3%82%BF%E3%82%A4%E3%83%88%E3%83%AB-Webhooks%E3%81%B8%E3%81%AE%E5%BA%8F%E7%AB%A0)を設定してください
    * Webhook URLが設定されていない場合に、投稿するボタンが設定されていても、実際には投稿されません(ブラウザのコンソールログにその旨表示されます)
  * bot_name
    * Discordに投稿する際の名前
  * bot_avatar_url
    * Discordに投稿する際使用するアイコン画像のURL

## Experiments

* Speech to text in the browser
  * [Speech to text in the browser with the Web Speech API](https://www.twilio.com/blog/speech-recognition-browser-web-speech-api)
  * [Browser speech recognition demo](https://browser-recognition.glitch.me/)
  * [Remix the speech recognition demo on Glitch](https://glitch.com/~browser-recognition)
  * [Source code](./speech-recognition)
