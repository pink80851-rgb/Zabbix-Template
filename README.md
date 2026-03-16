# Enterprise Zabbix Templates Collection

本倉庫收錄了針對企業基礎設施所開發的自定義 Zabbix 監控範本（YAML 格式）。涵蓋伺服器硬體、電力設備與存儲系統，實現對關鍵硬體指標的全面監控。

## 🛠 監控專案說明

### 🗄️ RAID 存儲監控 (Zabbix_RAID_template.yaml)
* **監控重點**: 硬體 RAID 卡狀態、磁碟健康度、重建進度。
* **解決問題**: 避免因硬碟損毀未及時發現而導致的數據丟失風險。

### 🔋 UPS 電力系統監控 (zbx_Ups_Webjson_template.yaml)
* **監控重點**: 透過 Web JSON 接口擷取 UPS 剩餘電量、負載百分比、輸入/輸出電壓。
* **實作特色**: 整合異質接口數據，將電力狀態視覺化，確保機房在斷電時能有充足的反應時間。

### 🖥 HP 伺服器硬體監控 (HP_templates.yaml)
* **監控重點**: 針對 HP 伺服器 iLO/SNMP 接口開發，監控風扇轉速、溫度、電源供應器 (PSU) 狀態。

## 🚀 核心優勢
- **自動化探索 (LLD)**: 部分 Template 整合了自動化探索邏輯，能自動識別磁碟數量與網路介面。
- **預警機制**: 內建多層級 Trigger（警告、嚴重、災難），確保維運人員能第一時間接收通知。
- **高度整合**: 所有範本均經過生產環境驗證，可直接導入 Zabbix 6.x 以上版本。

## 📂 目錄內容
- `Zabbix_RAID_template.yaml`: 磁碟陣列監控。
- `zbx_Ups_Webjson_template.yaml`: 不斷電系統監控解決方案。
- `HP_templates.yaml`: HP 伺服器專用硬體監控。
- `MESHA_export_templates.yaml`: 混合環境導出範本。

---
*專注於減少手動巡檢，實現 24/7 自動化硬體健康管理。*
