# Chrome

## Features

- Open Command Menu: `Ctrl + Shift + P`
- [Tabluar object view](https://umaar.com/dev-tips/82-console-table/) with `console.table(object)`
- [Toggle element classes](https://umaar.com/dev-tips/87-toggle-element-classes/)
- [Quick change CSS values](https://umaar.com/dev-tips/37-quick-change-css-values/):
  - Up / Down: increment / decrement by 1
  - Alt + Up: increment by 0.1
  - Shift + Up: increment by 10
  - Ctrl + Up: increment by 100
- [DevTools snippets](https://umaar.com/dev-tips/141-quick-open-menu-snippets/)
- [Blackbox scripts](https://umaar.com/dev-tips/128-blackboxing/)
- [Copy as curl](https://twitter.com/adrian_philipp/status/710438593936932864)

 ## Extensions

- [ModHeader](https://chrome.google.com/webstore/detail/modheader/idgpnmonknjnojddfkpgkljpfnnfcklj)
- [Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop)
- [Proxy SwitchySharp](https://chrome.google.com/webstore/detail/proxy-switchysharp/dpplabbmogkhghncfbfdeeokoefdjegm)
- [React Developer Tools](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi)
- [Redux DevTools](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd)
- [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm)

## Settings

- Hide the infobar for [remote debugging](https://stackoverflow.com/questions/18882497/jetbrains-ide-support-extension-how-to-disable-chrome-warnings)
  - `chrome://flags/` → Enable `Silent Debugging`
- Disable media keys:
  - `chrome://flags` → Hardware Media Key Handling

## Search engines

| Search engine         | Keyword | Query URL |
| --------------------- | --------|-----------|
| BoardGameGeek         | bgg     | https://boardgamegeek.com/geeksearch.php?action=search&objecttype=boardgame&q=%s   |
| DevDocs               | dd      | https://devdocs.io/#q=%s                                                           |
| Dict                  | dict    | https://www.dict.cc/?s=%s                                                          |
| Google Play           | app     | https://play.google.com/store/search?q=%s&c=apps                                   |
| IMDb                  | imdb    | https://www.imdb.com/find?s=all;q=%s                                               |
| Lodash                | lodash  | https://devdocs.io/#q=lodash %s                                                    |
| Thesaurus             | th      | https://www.thesaurus.com/browse/%s                                                |
| Ultimate Guitar       | ug      | https://www.ultimate-guitar.com/search.php?search_type=title&value=%s              |

## Override server response headers (ModHeader)

```
Access-Control-Allow-Credentials: true
Access-Control-Allow-Origin: http://localhost
Content-Security-Policy: <see below>
```

```
default-src *  data: blob: 'unsafe-inline' 'unsafe-eval';
script-src * data: blob: 'unsafe-inline' 'unsafe-eval';
connect-src * data: blob: 'unsafe-inline';
img-src * data: blob: 'unsafe-inline';
frame-src * data: blob: ;
style-src * data: blob: 'unsafe-inline';
font-src * data: blob: 'unsafe-inline';
```
