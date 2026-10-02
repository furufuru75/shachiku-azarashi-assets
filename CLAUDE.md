# 社畜アザラシ

Instagram / Threads `@shachiku_azarashi` の素材リポジトリ。

- リポジトリ直下の `NN_YYYY-MM-DD_(AM|PM).png`: 1日2回投稿する1枚絵
- `channel/voice.md`: キャラクターと口調の設定。コピー・台本・返信を書く前に必ず読む
- `.claude/skills/yt-*`: [youtube-agent-skill](https://github.com/Jakeschincariol/youtube-agent-skill)（MIT, `a2feb21`）を取り込んだもの。
  元の `~/.claude/youtube/voice.md` を `channel/voice.md` に読み替えてある

## 日本語で使うときの注意

スキル同梱の Python ツール（`hookscore.py`, `title.py`, `deadair.py`, `chapters.py`）は英語の単語を前提にした判定なので、
日本語の文に対する点数は意味をなさない。実行して点数を出したり、それを根拠にしたりしないこと。
代わりに `channel/voice.md` の「型」と「使わない言葉」に照らして候補を比べる。
`retention.py`（視聴維持率 CSV の分析）は言語に関係なく使える。
`swipe.py` の「チャンネル中央値の何倍伸びたか」の順位は使えるが、タイトルからフックの型を当てる部分は英語前提なので無視する。

出力は日本語で書く。
