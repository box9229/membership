簡易應用——Spring Boot會員管理系統
包含功能：

會員管理：主要為管理員提供添加查詢、狀態修改（這裡有正常、掛失、使用）、會員消費、會員註銷功能；
商品消費：提供添加、修改、購買、查詢記錄等功能；
禮品消費：禮品設置、數量修改、兌換記錄查詢等功能；
積分抽獎：通過管理員設置抽獎積分，然後隨時分配給成員；
生日提醒：通過富文本編輯器提供人性化的郵件提醒服務；
匯入資料庫檔案

在專案的路徑下可以找到檔案db_membership.sql，該檔案是MySQL的資料庫檔案檔案。通過MySQL匯入該檔案檔案庫生成資料庫db_membership 修改專案檔案
在專案路徑下的membership\src\main\resources有emailConfigproperties檔案，該檔案是用於郵箱傳輸的功能，需要進入自己的郵箱和密碼以及smtp，沒有填寫正確進入則不能正常使用郵箱的提醒功能 Mysql root 密碼
在專案路徑下membership\src\main\resources有application.properties檔案，該檔案是MYSQL，root, password, server.port=8080 等設置
提示：

本項目使用從Spring Boot1.5.9修改到Spring Boot2.0.0
改用自定義過濾器設置登錄
升級後部分修改：

加入Spring Security框架
部分方法不能使用，比如 findById 返回對象由實體對象改為可選對象
修改部分bug，如：會員狀態無法出現的情況
密碼均為123，登錄名為admin || 123

導入項目運行步驟可以去博客文章CSDN或cnblogs
https://www.cnblogs.com/lger/p/8366320.html
