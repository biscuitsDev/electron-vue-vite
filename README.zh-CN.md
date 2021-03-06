# electron-vue-vite

![awesome-vite](https://camo.githubusercontent.com/abb97269de2982c379cbc128bba93ba724d8822bfbe082737772bd4feb59cb54/68747470733a2f2f63646e2e7261776769742e636f6d2f73696e647265736f726875732f617765736f6d652f643733303566333864323966656437386661383536353265336136336531353464643865383832392f6d656469612f62616467652e737667)
![GitHub license](https://img.shields.io/github/license/caoxiemeihao/electron-vue-vite?style=flat)
![GitHub stars](https://img.shields.io/github/stars/caoxiemeihao/electron-vue-vite?color=fa6470&style=flat)
![GitHub forks](https://img.shields.io/github/forks/caoxiemeihao/electron-vue-vite?style=flat)


**[English](README.md) | ç®ä½ä¸­æ**

ð¥³ `Electron` + `Vue3` + `Vite2` æ´åæ¨¡æ¿ -- **ç»æç®åï¼å®¹æä¸æï¼**

## æ¦è¿°

&emsp;&emsp;è¿æ¯ä¸ä¸ªè¿½æ±ç²¾ç®ç`Electron`ç±»æ´åæ¨¡æ¿ï¼åªä¿ææåºæ¬çæä»¶ãæåºæ¬çä¾èµãæåºæ¬çåè½ï¼èä¸æ¯å¤§èå¨çãèè¿çè®¾è®¡ãè¿æ ·åçç®çæ¯è½ç¡®ä¿æ¨¡æ¿è¶³å¤çµæ´»ã

æä»¥è¯´å¦æä½ æ¯å¯¹ -- å·¥ç¨æ¨¡æ¿è¿½æ±ç²¾ç®ç Coderï¼æèåå¥ä¸çå°ç½æ³å¼æç½`Electron`æ´åç±»æ¨¡æ¿æåºç¡çå·¥ä½åçï¼äº¦æèä½ æ¯å¤§ç¥åªæ¯æ³å·æå°å¹²ç¹æ´»ï¼é£ä¹è¿ä¸ªæ¨¡æ¿æåéä½ ä¸è¿äºã

å°½ç®¡å¦æ­¤ï¼æè¿æ¯å¸æä½ å¯¹`Electron` `Vite`æä¸å®çåºç¡ï¼å ä¸ºé¤äºé¡¹ç®ç»æç®åå¤ï¼è¿ä»½`README`ä¹æ¾å¾ âç²¾ç®â ã

æ¨¡æ¿çå·ä½å®ç°ç»èæç¸ä¿¡ä½ çä¸¤éæºç å°±è½æå®åéäº ð

## è¿è¡é¡¹ç®

  ```bash
  # clone the project
  git clone git@github.com:caoxiemeihao/electron-vue-vite.git

  # enter the project directory
  cd electron-vue-vite

  # install dependency
  npm install

  # develop
  npm run dev
  ```

## ç®å½ç»æ

&emsp;&emsp;ä¸æ¦å¯å¨ææåèæ¬æ§è¡è¿ï¼ä¼å¨æ ¹ç®å½äº§ç **`dist` æä»¶å¤¹ï¼éé¢çæä»¶å¤¹å `src` ä¸æ¨¡ä¸æ ·**ï¼å¨ä½¿ç¨ä¸äºè·¯å¾è®¡ç®æ¶ï¼å°¤å¶æ¯ç¸å¯¹è·¯å¾è®¡ç®ï¼`dist` ä¸ `src` éé¢ä¿æç¸åçç®å½ç»æè½é¿å¼å¥½å¤é®é¢

```tree
â
âââ configs
â   âââ vite-main.config.ts          ä¸»è¿ç¨éç½®æä»¶ï¼ç¼è¯ src/main
â   âââ vite-preload.config.ts       é¢å è½½èæ¬éç½®æä»¶ï¼ç¼è¯ src/preload
â   âââ vite-renderer.config.ts      æ¸²æè¿ç¨éç½®æä»¶ï¼ç¼è¯ src/renderer
â
âââ dist                             æå»ºåï¼æ ¹æ® src ç®å½çæ
â   âââ main
â   âââ preload
â   âââ renderer
â
âââ scripts
â   âââ build.mjs                    é¡¹ç®æå»ºèæ¬ï¼å¯¹åº npm run build
â   âââ watch.mjs                    é¡¹ç®å¼åèæ¬ï¼å¯¹åº npm run dev
â
âââ src
â   âââ main                         ä¸»è¿ç¨æºç 
â   âââ preload                      é¢å è½½èæ¬æºç 
â   âââ renderer                     æ¸²æè¿ç¨æºç 
â
```

## æ¸²æè¿ç¨ä½¿ç¨ NodeJs API

> ð§ å ä¸ºå®å¨çåå  Electron é»è®¤ä¸æ¯æå¨ æ¸²æè¿ç¨ ä¸­ä½¿ç¨ NodeJs APIï¼ä½æ¯æäºå°æ²éå°±æ¯æ³è¿ä¹å¹²ï¼æ¦é½æ¦ä¸ä½ï¼å®å¨æ³é£ä¹å¹²çè¯ï¼è¿éæä¸ª ð npm å **[vitejs-plugin-electron](https://www.npmjs.com/package/vitejs-plugin-electron)** æèä½¿ç¨å¦ä¸ä¸ªæ¨¡æ¿ **[electron-vite-boilerplate](https://github.com/caoxiemeihao/electron-vite-boilerplate)**


#### æ¨èææç NodeJsãElectron API éè¿ `Preload-script` æ³¨å¥å° æ¸²æè¿ç¨ä¸­ï¼ä¾å¦ï¼

* **src/preload/index.ts**

  ```typescript
  import fs from 'fs'
  import { contextBridge, ipcRenderer } from 'electron'

  // --------- Expose some API to Renderer-process. ---------
  contextBridge.exposeInMainWorld('fs', fs)
  contextBridge.exposeInMainWorld('ipcRenderer', ipcRenderer)
  ```

* **src/renderer/src/global.d.ts**

  ```typescript
  // Defined on the window
  interface Window {
    fs: typeof import('fs')
    ipcRenderer: import('electron').IpcRenderer
  }
  ```

* **src/renderer/main.ts**

  ```typescript
  // Use Electron, NodeJs API in Renderer-process
  console.log('fs', window.fs)
  console.log('ipcRenderer', window.ipcRenderer)
  ```

## è¿è¡ææ
<img width="400px" src="https://raw.githubusercontent.com/caoxiemeihao/blog/main/electron-vue-vite/screenshot/electron-15.png" />

## å¾®ä¿¡ | | è¯·æåæ¯ä¸åè¶ ð¥³

<div style="display:flex;">
  <img width="244px" src="https://raw.githubusercontent.com/caoxiemeihao/blog/main/assets/wechat/group/qrcode.jpg" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img width="244px" src="https://raw.githubusercontent.com/caoxiemeihao/blog/main/assets/wechat/%24qrcode/%24.png" />
</div>
