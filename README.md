# locale-zh-Hans

這個倉庫包含了 State of JS/CSS/HTML 等調查的中文（繁體）語言文件。你可以在這裡查看 [所有語言倉庫列表](https://github.com/orgs/Devographics/repositories?q=locale-&type=all&language=&sort=name)。

## 如何貢獻代碼

#### 1. 成為翻譯者

要開始幫助翻譯調查，你應該 [加入 Discord](https://discord.com/invite/zRDb35jfrt) 並私訊我（`SachaG`）你的 GitHub 用戶名，以及你希望幫助翻譯的語言區域代碼（例如 `fr-FR`、`zh-Hant` 等）。

接著，我會授予你該所有翻譯 `yaml` 文件倉庫的維護者權限，之後你可以和其他翻譯團隊成員一起管理它。

#### 2. 尋找要翻譯的東西

你可以通過瀏覽調查應用、調查結果網站等方式來查找未翻譯的字串，或者使用我們的 API 獲得額外的資料，例如某語言區域的完成百分比或所有未翻譯的字串：

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

#### 3. 獲得貢獻認可

每位翻譯者都會在使用翻譯的調查應用網站中獲得貢獻認可。為了獲得認可，請將你的 GitHub 用戶名添加到每個語言區域 `config.yml` 文件中的 `translators` 陣列中。

以下是 `de-DE` 語言區域的範例：

- https://github.com/Devographics/locale-de-DE/blob/main/config.yml#L3

#### 4. 即時推送你的更改

目前沒有自動化的 GitHub Hooks 來更新翻譯好的語言文件，所以目前最好的方法是從 Discord 私訊告訴我你完成了翻譯。

## 翻譯文件

#### 調查應用

這些字串與用戶填寫實際調查時使用的應用相關。

- `surveys.yml`
- `accounts.yml`
- `state_of_js_2020_survey.yml`

#### 結果應用

這些字串僅出現在顯示調查結果和統計資料的靜態網站中。

- `results.yml`
- `state_of_css_2020.yml`
- `state_of_js_2020.yml`

#### 兩者都有

這些字串都出現在兩者中。

- `common.yml`
- `state_of_css.yml`
- `state_of_js.yml`

#### 其他

- `homepage.yml`

## 加入翻譯團隊

建議你加入你想翻譯的 [翻譯團隊](https://github.com/orgs/Devographics/teams/translators/teams)。

## 本地開發

目前在本地開發時，沒有簡單的方式查看字串的上下文。我們正在努力解決這個問題。

## 獲得幫助

加入 [我們的 Discord](https://discord.gg/zRDb35jfrt) 以獲得幫助。
