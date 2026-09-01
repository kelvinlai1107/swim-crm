# 游泳學院 CRM

游泳學院學員管理系統，含續報作業分析功能。

## 部署

此系統部署於 GitHub Pages，需使用公司 Microsoft 帳號登入。

## 權限設定

- **管理員**：可存取所有功能
- **門市老師**：只能存取續報作業

## 設定方式

在 `index.html` 找到以下區段並填入 Azure AD 資訊：

```javascript
var MSAL_CLIENT_ID = "YOUR_CLIENT_ID_HERE";
var MSAL_TENANT_ID = "YOUR_TENANT_ID_HERE";
```

並設定各帳號的存取權限：

```javascript
var ADMIN_EMAILS = ["kelvin@yourdomain.com"];
var STORE_EMAILS = ["teacher1@yourdomain.com"];
```
