### LinkedIn-contact-ETL-Pentaho-Practice
利用 Pentaho PDI 實作 LinkedIn 聯絡人資料的處理流程

#### 自主練習：LinkedIn 聯絡人數據過濾與格式轉換 (ETL)

#### 簡介
本專案為資料工程自主練習，旨在運用 **Pentaho Data Integration** 工具，將上千筆模擬的 LinkedIn 聯絡人原始資料（CSV 格式）進行資料清洗、欄位選取與格式轉化，最終輸出為結構化的 XML 檔案

#### 使用工具
* **ETL Tool**: Pentaho Data Integration (Spoon) 9.3.x
* **Data Source**: Simulated LinkedIn Connections Dataset (CSV)
* **Output Format**: XML

#### 檔案
* `linkedin_connections_1000.csv`: 原始數據集（包含 1000 筆模擬聯絡人資訊）
* `Contacts_Transformation.ktr`: Pentaho 轉換邏輯檔案
* `Contacts01Outputfile.xml`: 最終輸出檔案

#### ETL 流程說明
1. **Extract (讀取)**: 輸入 `CSV file input` 讀取原始 1000 筆聯絡人資料
2. **Transform (轉換)**:
   - 使用 `Select values` 篩選特定欄位
   - 自動化轉換欄位值以符合目標格式，確保資料一致性
3. **Load (寫入)**: 透過 `XML Output` 將處理後的資料流寫入目標檔案

#### 學習心得
透過此練習，我熟悉了 Pentaho 的操作介面，包括 **Design Tab** 中的 Step 配置與 **View Tab** 的流程管理，並了解資訊流在 ETL 過程中的傳遞邏輯