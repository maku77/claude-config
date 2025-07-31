# claude-config

Configuration files for Claude Code

- 参考: [Claude Code のカスタムコマンドを Git や Dropbox で共有する｜まくろぐ](https://maku.blog/p/xpwvvfz/)

## セットアップ方法

`commands` ディレクトリを Claude Code の設定ディレクトリにリンクして使用してください。

### Windows (ジャンクションを使用)

PowerShell を開き、以下のコマンドを実行してください：

```powershell
cmd /c mklink /J "$HOME\.claude\commands\maku" "$THIS_REPO\commands"
```

### macOS / Linux (シンボリックリンクを使用)

ターミナルで以下のコマンドを実行してください：

```bash
ln -s $THIS_REPO/commands ~/.claude/commands/maku
```

`$THIS_REPO` はこのリポジトリを `git clone` したパスに置き換えてください。

### 動作確認

Claude Code を起動して、`/maku:hello` というスラッシュコマンドを起動できるようになっていることを確認します。

```
> /maku:hello

⏺ てすと、てすと
```

