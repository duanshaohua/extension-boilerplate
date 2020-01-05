<div align="center">
  <h1>
    扩展样板  
  </h1>

  <p>
    <strong>为Chrome、Opera和Firefox创建浏览器扩展的样板。</strong>
  </p>
</div>
现在Firefox支持Web扩展，在不复制代码库的情况下，为多个浏览器构建浏览器扩展/插件变得容易多了。这个项目可以作为一个明智的起点来帮助你开始。

<div align="center">
  <a href="https://www.emailthis.me/open-source/extension-boilerplate">
    <img src="./resources/chrome-promo/large.png" alt="Extension Boilerplate">
  </a>
</div>

I have extracted this from the browser extensions that I built for my side-project, [Email This](https://www.emailthis.me).

> Side note: Do check out [**Email This**](https://www.emailthis.me). It is a simpler alternative to bookmarking tools like Pocket, Readability & Instapaper. Email This will remove ads & distractions from an article and send you a nice email with just the text/images. No need to install any additional applications or login to another app just to access your bookmarks. 
The Chrome Extensions is available [on the Chrome Web Store](https://chrome.google.com/webstore/detail/email-this/lgblkllcjgihfnlefhnnpppndbbjallh).


## Features

<dl>
  <dt>写一次并部署到 Chrome, Opera & Firefox</dt>
  <dd>
    基于Web扩展。它还包括一个小的polyfill，为不同浏览器暴露的api带来一致性。
  </dd>
</dl>

<dl>
  <dt>Live-reload</dt>
  <dd>
    你对CSS、HTML和JS文件的修改将会被立即转发，而无需手动重新加载扩展。 这最终节省了大量时间并改善了开发人员的体验。
  </dd>
</dl>

<dl>
  <dt>明智的起点</dt>
  <dd>
    它提供了一个基于gulp的工作流，可以转换为现代工作流 <strong>ES6</strong> JavaScript and <strong>SCSS</strong> to JS/CSS. 
    脚本使用Babel进行转换，并使用Browserify绑定。
    源文件可用于JS和SCSS。
  </dd>
</dl>

<dl>
  <dt>Sketch (.sketch) assets for icons and promo images</dt>
  <dd>
    A .sketch file is included in the resources directory. This has all the icons and promo images that will be needed while uploading the extensions to the app stores.
  </dd>
</dl>

<dl>
  <dt>Easily configurable and extendable</dt>
  <dd>
    The gulpfile is easily understandable and configurable. If you want to add additional tasks or remove un-used ones, you can easily tweak that file to suit your needs.
  </dd>
</dl>

<dl>
  <dt>Platform specific & Environment specific variables.</dt>
  <dd>
    You might need to specify different data variables based on your environment. For example, you might want to use a localhost API endpoint during development and a production API endpoint once the extension is submitted to the appstore. You can specify such data in the json files inside `config` directory.

    You can also set custom data variables based on the platform (different variable for Chrome, FF, Opera).
  </dd>
</dl>



## Installation
1. Clone the repository `git clone https://github.com/EmailThis/extension-boilerplate.git`
2. Run `npm install`
3. Run `npm run build`

Alternately, if you want to try out the sample extension, here are the download links. After you download it, unzip the file and load it in your browser using the steps mentioned below.
 - [**Download Chrome Extension**](https://github.com/EmailThis/extension-boilerplate/releases/download/v1.0/chrome.zip)
 - [**Download Opera Extension**](https://github.com/EmailThis/extension-boilerplate/releases/download/v1.0/opera.zip)
 - [**Download Firefox Extension**](https://github.com/EmailThis/extension-boilerplate/releases/download/v1.0/firefox.zip)


##### Load the extension in Chrome & Opera
1. Open Chrome/Opera browser and navigate to chrome://extensions
2. Select "Developer Mode" and then click "Load unpacked extension..."
3. From the file browser, choose to `extension-boilerplate/build/chrome` or (`extension-boilerplate/build/opera`)


##### Load the extension in Firefox
1. Open Firefox browser and navigate to about:debugging
2. Click "Load Temporary Add-on" and from the file browser, choose `extension-boilerplate/build/firefox`


## Developing
The following tasks can be used when you want to start developing the extension and want to enable live reload - 

- `npm run chrome-watch`
- `npm run opera-watch`
- `npm run firefox-watch`


## Packaging
Run `npm run dist` to create a zipped, production-ready extension for each browser. You can then upload that to the appstore.


## TODO
- [ ] Add support for Safari
- [x] Add Firefox & Opera Promo images
- [x] Add sample screenshot templates
- [ ] Write a guide for using config variables & JS preprocessor


-----------
This project is licensed under the MIT license. 

If you have any questions or comments, please create a new issue. I'd be happy to hear your thoughts.


Bharani, [Email This](https://www.emailthis.me)
