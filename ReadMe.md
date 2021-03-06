# Puppeteer-IE

Headless **Internet Explorer** NodeJS API inspired by [Puppeteer](https://github.com/GoogleChrome/puppeteer).

**[ Notice ]**  [Microsoft Edge](https://www.microsoft.com/en-us/windows/microsoft-edge) isn't supported by this package as it utilizes [ActiveX](https://msdn.microsoft.com/en-us/library/windows/desktop/ms693753),
whereas Edge uses the [WebDriver protocol](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/) & [DevTools Protocol](https://docs.microsoft.com/en-us/microsoft-edge/devtools-protocol/) for automation.
So you can control it by [Selenium](http://seleniumhq.github.io/selenium/docs/api/javascript/index.html) or [Edge diagnostics adapter](https://github.com/Microsoft/edge-diagnostics-adapter).

[![NPM](https://nodei.co/npm/puppeteer-ie.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/puppeteer-ie/)



## Installation

```Shell
npm install puppeteer-ie
```

**[ Notice ]**  If you get some error at installing, try to execute the command below:

```Shell
npm install --global --production windows-build-tools
```
([More about this](https://github.com/nodejs/node-gyp#option-1))



## Usage

Only change the Package Name, and then do as [Puppeteer does](https://github.com/GoogleChrome/puppeteer/blob/master/docs/api.md).

**[ Recommendation ]**  Use [DayDream](https://github.com/segmentio/daydream) to record operation scripts in [Google Chrome](https://www.google.com/chrome/).

**API document** accesses from https://techquery.github.io/Puppeteer-IE/ or `npm run help`.



## Known issue

 1. *Loading pages* of IE will be blocked if a *Web server* running in the same *NodeJS process*

 2. *Loading pages* from `localhost` will lost the `window` object in *NodeJS process*

For the above reasons, I recommend using [KoApache](https://www.npmjs.com/package/koapache) to [host your Web pages for testing](https://github.com/TechQuery/Puppeteer-IE/blob/master/test/Page.js#L19) or other things.



## Development

[Contributor guide](https://github.com/TechQuery/Puppeteer-IE/blob/master/Contributing.md)



## Acknowledgement

 1. [Puppeteer](https://github.com/GoogleChrome/puppeteer)

 2. [Node-ActiveX](https://github.com/durs/node-activex)

 3. [HTML2Canvas](http://html2canvas.hertzen.com/)
