# GitHub 創建新倉庫

Tags: Github

### 建立新的GitHub repository

1. 建立路徑
    
    ```bash
    mkdir new_project
    cd new_project
    ```
    
2.  初始化一個新的 Git repository
    
    ```bash
    git init
    ```
    
3. 創建README.md
    
    ```bash
    echo "Hello World" >> README.md
    ```
    
4. 保存變更到local git repository
    
    ```bash
    git commit -m "commit"
    ```
    
    ‘-m’ 表達短句子無需打開編輯器(vim)
    
5. 在GitHub 中新增repository 並獲得Git repository的SSH URL
    1. 
    
    ![https://docs.github.com/assets/cb-34248/mw-1440/images/help/repository/repo-create-global-nav-update.webp](https://docs.github.com/assets/cb-34248/mw-1440/images/help/repository/repo-create-global-nav-update.webp)
    
    ![https://docs.github.com/assets/cb-61138/mw-1440/images/help/repository/create-repository-name.webp](https://docs.github.com/assets/cb-61138/mw-1440/images/help/repository/create-repository-name.webp)
    
    ![https://docs.github.com/assets/cb-48149/mw-1440/images/help/repository/copy-remote-repository-url-quick-setup.webp](https://docs.github.com/assets/cb-48149/mw-1440/images/help/repository/copy-remote-repository-url-quick-setup.webp)
    
6. 把remote 設置為Git repository 的 URL **`origin`** 作為remote的別名
    
    ```bash
    git remote add origin **SSH_URL**
    ```
    
7. 把當前 branch 命名為 main
    
    ```bash
    git branch -M main
    ```
    
    • **`-M`** 選項表示強制重新命名分支，即使新名稱的分支已經存在。
    
8. 把 main 上傳(push) 到Git repository
    
    ```bash
    git push -u origin main
    ```