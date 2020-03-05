# ShadowsocksX-NG

* `系统要求：macOS 10.5 及以上`
* `軟體版本：ShadowsocksX-NG-R8 1.4.4`
* `設備要求：MacBook / iMac / Mac Pro`

登入帳號，用戶中心底部[下载](http://1mix.org/user)並安装完成後，打開dmg文件，然後將其拖動到右側的Applications安裝。

![&#x5C07;&#x5176;&#x62D6;&#x52D5;&#x5230;&#x53F3;&#x5074;&#x7684;Applications&#x5B89;&#x88DD;&#x3002;](../../.gitbook/assets/e9ae1547179960.jpg)

安裝完成後，從LaunchPad或應用程序中打開，系統右上角會出現小飛機標誌。

![](../../.gitbook/assets/c_mac_2.png)

如提示不安全，请到系统偏好设置打开程式

![](../../.gitbook/assets/c_mac_3.png)

點擊小飛機打開菜單——服務器——編輯訂閱：

![&#x7DE8;&#x8F2F;&#x8A02;&#x95B1;](../../.gitbook/assets/c_mac_4.png)

點擊+號後填入訂閱地址後手動更新訂閱

![](../../.gitbook/assets/c_mac_5.png)

右上角会显示「成功更新订阅」

服務器添加成功後，選擇代理方式為繞過中國IP。或者也可以選擇PAC自動模式，前提是先點擊GFW List更新PAC，更新成功後，設置為PAC自動模式。

![](../../.gitbook/assets/80c71547179962.jpg)

選擇一個節點

![](../../.gitbook/assets/c_mac_6.png)

即可正常使用

{% hint style="info" %}
手動新增伺服器方式，不建議新手使用!
{% endhint %}

點擊小飛機打開菜單——服務器——服務器設置：

![](../../.gitbook/assets/0e8a1547179961.jpg)

在接下來的窗口中，點擊左下側的 + 號，然後在右側設置服務器參數，下圖紅框內容為必填項。

![](../../.gitbook/assets/0b521547179961.jpg)

地址：即網站服務器的IP地址，填好IP地址後，在後面的小框內填入服務端口。  
加密方法：與服務端設置的Stream Cipher參數保持一致。  
密碼：填入服務端設置的密碼。  
協議：與服務端設置的Protocol參數保持一致。  
混淆：與服務端設置的obfs參數保持一致。  
混淆參數：一般默認為空。

{% hint style="info" %}
相關數據請登入網站後查看節點列表
{% endhint %}

{% hint style="success" %}
Happy End 您可以愉快的使用了！
{% endhint %}

### 新版macOS 無法更新訂閱 問題解決辦法

新版mac系統因為新增 App Transport Security \(ATS\)機制關係，HTTP都轉向TLS1.2協議進行傳輸會導致原來請求更新訂閱網址，非HTTPS訪問是禁止的，照下面操作方法修改APP即可正常更新訂閱 \(本教學由1MiX撰寫真正實力技術派，轉貼請註明\)。

![](../../.gitbook/assets/ying-mu-kuai-zhao-20190713-shang-wu-12.25.10.png)

到 應用程式 找到 ShadowsocksX-NG-R8 應用程式，右鍵 &gt; 顯示套件內容  或 齒輪 &gt; 顯示套件內容

![&#x96D9;&#x64CA;&#x9032;&#x5165; Contents &#x6587;&#x4EF6;&#x593E;](../../.gitbook/assets/ying-mu-kuai-zhao-20190713-shang-wu-12.25.31.png)

[點此下載](http://1mix.org/ssr-download/Info.zip) Info.plist 文件壓縮檔 

![](../../.gitbook/assets/ying-mu-kuai-zhao-20190713-shang-wu-12.26.05.png)

打開下載下來的壓縮檔，將Info.plist 檔案拖曳進去，**取代**

重新打開app 即更新訂閱成功

### 閃退開不起來 解決辦法

一般開啟來程式及閃退，是因為之前有使用過，設定不良導致

在 Finder 中，選擇「前往 > 移至資料夾」。

在「移至資料夾」對話框中，鍵入 ~/Library

按一下「前往」。

刪除
/Users/{Your user name}/Library/Preferences/com.qiuyuzhou.ShadowsocksX-NG.plist
重新安裝一次軟體 即可

另外也可以檢查是否有殘餘資料夾
/Users/{Your user name}/.ShadowsocksX 
