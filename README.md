# RPHackathon
## ディレクトリ構成

- `.devcontainer`: VS CodeのDevContainerの設定ファイルが含まれています。
  - `Dockerfile`: DevContainerで使用するDockerfileです。
  - `devcontainer.json`: DevContainerの設定ファイルです。
- `.streamlit`: Streamlitの設定ファイルが含まれています。
- `.env.template`: 環境変数のテンプレートファイルです。
- `.gitignore`: Gitレポジトリの管理対象から外すファイルの設定が記述されています。
- `requirements.txt`: 必要なPythonパッケージが記載されています。

## 使い方

### 環境変数の設定

1. `.env.template`をコピーして`.env`ファイルを作成します。
2. `.env`ファイルに必要な環境変数の値を設定します。以下の環境変数が利用可能です：
   - `OPENAI_API_KEY`: OpenAI APIのAPIキー
   - `ANTHROPIC_API_KEY`: Anthropic APIのAPIキー
   - `GOOGLE_API_KEY`: Google APIのAPIキー


このプロジェクトを動作させるための手順を以下に示します。

python3.11 -m venv venv
source venv/bin/activate #Mac/Linux    
venv\Scripts\activate #Windows
pip install -r requirements.txt
python app.py
