# AGENTS.md

- 所有回應一律使用繁體中文。
- 專案語言為 Python；目前僅有 `README.md` + Python `.gitignore`，無既有原始碼、測試、lint、CI。
- 一律使用 conda 管理 Python 套件，環境名稱為 `iem_python`。
  - 安裝：`conda install -n iem_python <pkg>`；執行：`conda run -n iem_python python <file>`。
  - 需新套件時優先用 conda 安裝，不要混用 pip／venv／poetry／uv；除非 conda 無此套件才經使用者同意使用 pip。
- 執行前先確認環境存在：`conda env list`；若 `iem_python` 不存在則停下詢問，勿自行新建或切換環境。
- 無測試框架與 lint 設定；完成前至少以 `conda run -n iem_python python <file>` 驗證；新增檔案放 repo 根目錄，勿自行搭建 monorepo、打包或 CI。
