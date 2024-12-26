# locale-zh-Hans

這個 Repo (Repository) 包含了 State of JS/CSS/HTML 等調查的中文（繁體）文件。你可以在這裡查看 [所有 Repository 列表](https://github.com/orgs/Devographics/repositories?q=locale-&type=all&language=&sort=name)。

## 如何參與

#### 1. 成為翻譯者

如果想協助翻譯，你可以 [加入 Discord](https://discord.com/invite/zRDb35jfrt) 並向（`SachaG`）私訊提供你的 GitHub 使用者名稱，以及希望翻譯的地區代碼（例如 `fr-FR`、`zh-Hant` 等）。

待收到翻譯團隊邀請後，你便可以和其他團隊成員進行翻譯與維護。

#### 2. 尋找要翻譯的東西

你可以瀏覽調查結果網站來查找尚未翻譯的文字，或者使用我們的 API 取得額外的資料，例如某地區代碼的完成百分比，或者是所有未翻譯的字串：

- https://graphiql.devographics.com/

以下是範例查詢：

```graphql
query GetLocaleData {
  locale(localeId: ru_RU) {
    completion
    totalCount
    translatedCount
    translators
    untranslatedKeys
  }
}
```

#### 3. 取得貢獻認可

每一位翻譯者都能在貢獻列表中顯示自己的名字，因此你可以將 GitHub 使用者名稱新增到 `config.yml` 文件的 `translators` 中。

以下是 `de-DE` 語言區域的範例：

- https://github.com/Devographics/locale-de-DE/blob/main/config.yml#L3

#### 4. 即時推送你的更改

目前沒有自動化的 GitHub Hooks 來更新翻譯好的文件，請直接從 Discord 文字頻道或私訊（`SachaG`）說明你完成了翻譯。

## 翻譯文件

#### 調查相關文件

這些文件會在調查問卷中出現。

- `surveys.yml`
- `accounts.yml`
- `state_of_js_2020_survey.yml`

#### 調查結果相關文件

這些文件僅出現在問卷結果和統計資料的靜態網站中。

- `results.yml`
- `state_of_css_2020.yml`
- `state_of_js_2020.yml`

#### 共通文件

這些文件都會出現在上述兩種情境。

- `common.yml`
- `state_of_css.yml`
- `state_of_js.yml`

#### 其他

- `homepage.yml`

## 加入翻譯團隊

建議你可以加入對應語言區域的 [翻譯團隊](https://github.com/orgs/Devographics/teams/translators/teams)。

## 本地開發

目前在本地開發時，沒有相對簡單的方式來反查字串的原文內容。我們正在努力解決這個問題。

## 取得幫助

加入 [我們的 Discord](https://discord.gg/zRDb35jfrt) 以取得幫助。
