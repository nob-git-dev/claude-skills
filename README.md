# claude-skills

Claude Code 向けスキル・エージェント・フックのコレクション。

各スキルセットは独立したサブディレクトリに収録されています。
特定のスキルだけ取得したい場合は [sparse-checkout](#sparse-checkout) を利用できます。

---

## スキル一覧

| ディレクトリ | 内容 |
|---|---|
| [sdlc-skills/](sdlc-skills/) | 仕様書（SPEC.md）を中心に SDLC プロセスを規律正しく進めるスキルセット |

---

## インストール（全スキル）

```bash
git clone https://github.com/nob-git-dev/claude-skills.git
cd claude-skills/<スキル名>
./scripts/install.sh
```

## Sparse-checkout（特定スキルだけ取得）

```bash
git clone --no-checkout https://github.com/nob-git-dev/claude-skills.git
cd claude-skills
git sparse-checkout init --cone
git sparse-checkout set sdlc-skills
git checkout main
cd sdlc-skills
./scripts/install.sh
```

---

## ライセンス

各スキルセットのディレクトリ内の LICENSE ファイルを参照してください。
