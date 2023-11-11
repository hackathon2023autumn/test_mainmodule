# sub module を持つ main module のリポジトリの混乱を防止する

- sub module の更新が未完了なのに main module を更新すると混乱する。それを GitHub Actions と Branch Protection で防ぐ。
- GitHub Actions の yml ファイルに sub module の更新状態をチェックするスクリプトを書き、GitHub の main module リポジトリの settings->branches->Protection Rules で require pull request と status check を有効にする。
