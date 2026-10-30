# プライバシー / Privacy

## プライバシー

euno が読むもの、書くもの、送るもの。設定の「プライバシー」と同じ内容。

### 読むもの

| もの | 範囲 |
| --- | --- |
| ブリッジに入れたチャット | ユーザーとエージェントの発言 |
| 読まないもの | thinking、ツールの呼び出しと結果、添付 |
| 最近のチャット | タイトル、フォルダ、更新日時 |
| Claude、Codex、Cursor の保存場所 | 読み取りだけ |
| Claude、Codex、Cursor の設定 | euno の登録だけ |
| Claude、Codex、Cursor のウィンドウ | 前面のウィンドウのタイトルと URL |
| キー入力 | 右⌘の2回押しだけ |
| 実行中のプロセス | euno-mcp だけ |

### 書くもの

| もの | 範囲 |
| --- | --- |
| ブリッジの設定 | `~/Library/Application Support/euno` |
| 読んだ記録 | `~/Library/Application Support/euno`、本文なし |
| euno の設定 | `~/Library/Preferences` |
| Claude、Codex、Cursor の設定とスキル | 設定の「連携」でボタンを押したときだけ |

### 送るもの

| もの | 範囲 |
| --- | --- |
| 発言、読んだ記録、利用状況 | 送らない |
| アップデート | `updates.fenrirx.dev`、`github.com` |
| スキルの追加と更新 | npm、GitHub |
| ブリッジの名前（AI のボタンを押したとき） | チャットのタイトルとリポジトリの名前を、選んだ CLI で送る |
| メニューの「問題を報告…」 | バージョン、権限、連携の状態を入れた Issue を開く |

## Privacy

What euno reads, writes, and sends. This matches the Privacy page in Settings.

### Reads

| Item | Scope |
| --- | --- |
| Chats in a bridge | User and agent messages |
| Excluded content | Thinking, tool calls and results, attachments |
| Recent chats | Titles, folders, modification dates |
| Claude, Codex, and Cursor storage | Read-only |
| Claude, Codex, and Cursor settings | euno registration only |
| Claude, Codex, and Cursor windows | Frontmost window title and URL |
| Keyboard input | Double tap of the right ⌘ key only |
| Running processes | euno-mcp only |

### Writes

| Item | Scope |
| --- | --- |
| Bridge settings | `~/Library/Application Support/euno` |
| Read records | `~/Library/Application Support/euno`, without message text |
| euno settings | `~/Library/Preferences` |
| Claude, Codex, and Cursor settings and skills | Only when you click a button in Settings → Integrations |

### Sends

| Item | Scope |
| --- | --- |
| Messages, read records, usage data | Not sent |
| Updates | `updates.fenrirx.dev`, `github.com` |
| Skill installation and updates | npm, GitHub |
| Bridge naming, when you click the AI button | Chat titles and repository names are passed to the CLI you choose |
| Report a Problem… in the menu | Opens an issue form containing version, permission, and integration information |
