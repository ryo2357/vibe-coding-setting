# vibe-coding-setting

GitHub Copilot で Vibe Cording を行うための設定を管理するためのリポジトリ

## リポジトリの構成

- `plain`
  MCP を追加しない運用

- `serena`
  Serena MCP を追加した運用

- `develop`
  検証中の運用

## フォルダ内容

- `.github`
  GitHub Copilot 関連の設定を管理します。

- `.vscode/`  
  `.github`内のファイルを参照する VSCode の設定を管理

- `root_files`
  プロジェクトルートに配置するファイル群
  主に`AGENTS.md`

## 使用方法

### 新規プロジェクトへの導入

1. 導入したいプロジェクトのルートディレクトリに移動します。

   ```bash
   cd /path/to/your/new-project
   ```

2. このリポジトリをクローンします。

   ```bash
   git clone git@github.com:ryo2357/vibe-coding-setting.git
   ```

3. 必要なフォルダやファイルをプロジェクトにコピーします。

   ```bash
   cp -r vibe-coding-setting/<select configuration>/.docs ./
   cp -r vibe-coding-setting/<select configuration>/.github ./
   cp -r vibe-coding-setting/<select configuration>/.vscode ./
   cp -r vibe-coding-setting/<select configuration>/root_files/* ./
   ```

4. クローンしたリポジトリを削除します（オプション）。

   ```bash
   rm -rf vibe-coding-setting/
   ```

5. プロジェクトに合わせて設定をカスタマイズします。
