# claude-config

Configuration files for Claude Code

- 参考: [Claude Code のカスタムコマンドを Git や Dropbox で共有する｜まくろぐ](https://maku.blog/p/xpwvvfz/)

## セットアップ方法

`agents`、`commands` ディレクトリを Claude Code の設定ディレクトリにリンクして使用してください。

### Windows (ジャンクションを使用)

PowerShell を開き、以下のコマンドを実行してください：

```powershell
cd claude-config
cmd /c mklink /J "$HOME\.claude\commands\maku" "$PWD\commands"
cmd /c mklink /J "$HOME\.claude\agents\maku" "$PWD\agents"
```

### macOS / Linux (シンボリックリンクを使用)

ターミナルで以下のコマンドを実行してください：

```bash
cd claude-config
ln -s $PWD/commands ~/.claude/commands/maku
ln -s $PWD/agents ~/.claude/agents/maku
```

`$THIS_REPO` はこのリポジトリを `git clone` したパスに置き換えてください。

### 動作確認

Claude Code を起動して、`/maku:hello` というスラッシュコマンドを起動できるようになっていることを確認します。

```
> /maku:hello

⏺ てすと、てすと
```
