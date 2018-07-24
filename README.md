# TWII_predict
以機器學習模型根據各種財經指數預測明天的台股加權指數漲跌

主程式檔：./TWII_Daily_predict/TWII_Daily_predict-v04.ipynb

版本：Draft(待系統架構師修正後提供正式版)

宣告：本程式作為「AI傳說對決——建構股市AI生態系」專案之AI模型封包pkl檔開發示範，開放版權可依自由軟體授權協定使用。

AI模型封包須包含以下三項資料：
1. 模型說明：適用投資標的、執行週期、是否可重新訓練及訓練所需資源、其他事項
2. 特徵項清單：依Yahoo Finace之[股票/指數/商品代碼]及[Open,High,Low,Close,Adj Close,Volume,Ratio漲跌幅]，列出模型預測所需輸入之特徵項名稱清單，平台將依此清單傳入變項值。
3. 模型檔：訓練好的模型依<<Sickit Learn>>的<<sklearn.externals>>模組<joblib.dump()>匯出檔案格式進行封裝，平台也將以該模組<joblib.load()>方法載入模型，以<model.predict()>方法使用該模型執行預測。

參考資料：http://scikit-learn.org/stable/modules/model_persistence.html
