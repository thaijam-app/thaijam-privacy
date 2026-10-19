# Android 隱私權政策的維護備註

原本放在 `docs/privacy-policy-android.md` 開頭的 HTML 註解。GitHub Pages 會把註解原樣輸出到網頁原始碼，所以 2026-10-19 搬到 docs 外面（不會發布）。

```
  ─────────────────────────────────────────────────────────────
  **這一份是發布中的正式版本,網址是**
  https://privacy.thaijam.app/privacy-policy-android/

  ⚠️ **發布的來源是 `thaijam-app/thaijam-privacy` 這個 repo,不是 ThaiJam。**
  (2026-08-14 更正 —— 這一段原本寫「它由這個 repo 的 GitHub Pages 產生」,
  而那份檔案當時在 ThaiJam repo 裡。那句話讓人以為推 ThaiJam 就會發布,
  實際上推了 59 個 commit 一點反應都沒有,而線上停在五天前的舊版。)

  `thaijam-privacy/docs/` 才是 Pages 的來源(CNAME 在那裡)。ThaiJam repo
  裡的同名檔案是**編輯用的副本**,改完要複製過來才會上線。

  **兩份副本正是這一頁會過期的原因** —— 上一次是政策寫著「學習內容不會
  上傳」而跨裝置同步早就做出來了;這一次是政策沒有提到發音評測會把錄音
  送到 Microsoft Azure,而那個功能在 production 已經開著。
  改任何一邊之後,**一定要確認 https://privacy.thaijam.app 上真的變了**。

  iOS 版的政策在同目錄的 privacy-policy.md。兩個平台的功能範圍不同
  (iOS 有 iCloud 備份,Android 沒有),所以刻意分成兩頁而不是一頁分節。

  ⚠️ **這一行原本寫「Android 沒有 Apple Music」,那是錯的**(2026-08-14 更正)。
  Android 有完整的 Apple Music 整合(MusicKit 授權、搜尋、播放控制),
  也有聽歌辨識(ShazamKit)、Apple 登入、Google Play 購買 ——
  這四項當時政策裡一個字都沒有。**兩邊的功能差距比這份文件以為的小得多**,
  下次寫「Android 沒有 X」之前先去 app/src 確認。

  **AI 兩邊都有了**(2026-08-14 更正)。這一行原本寫「Android 目前沒有 AI」,
  而同一份文件的第四節就在說明 AI 點數 —— 一份自我矛盾的隱私權政策比
  過期的更糟,因為讀的人不知道該信哪一句。

  ─────────────────────────────────────────────────────────────
  **這一份的每一句都對應到 Android 的程式碼,改功能就要回來改它。**

  Play Console 的「資料安全」表單必須跟這一頁逐項對得上 ——
  對不上是下架等級的問題。填表的逐題答案在 ThaiJamAndroid repo 的
  docs/play-data-safety-answers.md。

  審核時逐項核對的來源(都在 ThaiJamAndroid):
    - 上傳哪些東西  → SyncCodecs.KIND_*(現在十個)
    - 會發哪些請求  → ThaiJamApi 裡有呼叫端的那幾支
    - 權限          → AndroidManifest.xml 的 uses-permission
    - 沒上線的功能  → 對應的 task 還是 pending

  有一條測試(PrivacySyncCoverageTest)會在同步的 kind 清單變動時變紅,
  提醒回來改這一頁。

  App 內的同一份說明在 ThaiJamAndroid 的
  app/src/main/java/com/thaijam/android/ui/settings/PrivacyPolicyScreen.kt,
  兩邊要一起改。
  ─────────────────────────────────────────────────────────────
```
