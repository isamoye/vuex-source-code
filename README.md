# ð¢ è¯´æ

æ¬ä»åºç¨äºéè¯»å¹¶è®°å½ `Vuex` æºç ï¼**æ³¨ï¼** ææå¯¹äºæºç çè§£è¯»é½å¨ç¸åºæä»¶ï¼`./src`ï¼ä¸­å ä¸äºä¸­ææ³¨é

>è¥ä½ è§å¾æ¬ä»åºå¯¹ä½ éå¸¸æå¸®å©ï¼æ¬¢è¿ç¹ä¸ª **star** æ¯ææä¸ä¸å¦ï½

éå¸¸å»ºè®®ä¸äºè½åæéå¹¶ä¸ä»æªéè¯»è¿æçåºæºç çåç«¯æ **Vuexæºç ** ä½ä¸ºèªå·±ç¬¬ä¸ä¸ªéè¯»æºç çåºï¼å ä¸ºå®æ¬èº«ä»£ç éåªæå ç¾è¡ï¼å®ç°é»è¾ä¹éå¸¸ææï¼æç¸ä¿¡åªè¦ç¨å¿ãè¯è±è´¹æ¶é´ï¼ä¸å®è½å°å®çæºç è¯»æç

å½ç¶ï¼éè¯»æºç çåææ¯ä½ å¿é¡»å¯¹è¿ä¸ªåºæä¸å®çä½¿ç¨ç»éªä»¥åäºè§£ï¼å¦åå°±ç®å¼å§éè¯»æºç äºï¼ä½ ä¹å¾é¾ç¥éå®å¨åä»ä¹  â¡ï¸   [Vuexå®æ¹ææ¡£](https://vuex.vuejs.org/zh/)

åå¼å§åå¥½éè¯»æºç çåå¤ï¼æç»èªå·±å®ä¸çæéæ¯ `15`å¤©ï¼æç»ç®ä¸ç¼åæ­¤ææ¡£çæ¶é´ï¼ä¸å±ç¨äº `8` å¤©

`Vuex`ä¹æ¯æç¬¬ä¸æ¬¡éè¯»æºç çåºï¼æ¬ä»åºä¼è®°å½ä¸æéè¯»æºç çå¨è¿ç¨ä»¥åç»éªåäº«ï¼å¸æå¯ä»¥å¸®å©å°å¤§å®¶ï½

# âï¸ è¿åº¦ï¼8/8ï¼

**ã2021å¹´ã** æ¯å¤©éè¯»ææ»ç»æ´ç2å°æ¶ï¼æ¶é´çº¿ä¸­è¥æªåºç°çæ¥æï¼å¯è½æ¯å ä¸ºå¶å®äºæè½æäºï¼

> **Start**   1æ15æ¥ ï¼çæäº `Modules` çæ³¨åæµç¨

>1æ16æ¥ï¼äºè§£äºä¸ä¸æ¯ä¸ª `module` æ³¨å `state` ã`mutations` ã`actions`ã`getters` çå¤§ä½æµç¨

>1æ17æ¥ï¼è¯¦ç»äºè§£äº `vm` å¯¹ `state` ã`getters` çå¤çæ¹å¼

>1æ19æ¥ï¼å¤§è´äºè§£å®äºå¨é¨çæµç¨ï¼ä½è¿æå¾å¤ç»èæ²¡æç½ï¼å¹¶æ¥åäºé¨åæºç çéè¯»ææ¡£

>1æ20æ¥ï¼ææ¸äºå¾å¤ç»èé¨åï¼åæ¶æ´æ°äºé¨åæºç çéè¯»ææ¡£

>1æ23æ¥ï¼ç¼åäºé¨åæºç çéè¯»ææ¡£

> 1æ25æ¥ï¼ç¼åäºç»å¤§é¨åæºç çéè¯»ææ¡£

> **End** 1æ26æ¥ï¼äºè§£äº `Vuex` ç `install` æ¹æ³ãè¾å©å½æ°ï¼å¹¶æ´æ°äºå¨é¨çæºç éè¯»ææ¡£

# ð¥ æºç è§£æ

## ä¸ãæºç ç®å½ç»æåæ
æ´ä¸ª `Vuex` çæºç æä»¶éå¸¸å¤ï¼æä»¬ç´æ¥çæä¸»è¦çæä»¶ï¼å³ `src` æä»¶å¤¹ä¸­çåå®¹ï¼ç»æç¤ºä¾å¦ä¸ï¼

```js
âââ src
    âââ module    // ä¸æ¨¡åç¸å³çæä½
    â   âââ module-collection.js   // ç¨äºæ¶éå¹¶æ³¨åæ ¹æ¨¡åä»¥ååµå¥æ¨¡å
    â   âââ module.js   // å®ä¹Moduleç±»ï¼å­å¨æ¨¡ååçä¸äºä¿¡æ¯ï¼ä¾å¦: state...
    â
    âââ plugins   // ä¸äºæä»¶
    â   âââ devtool.js   // å¼åè°è¯æä»¶
    â   âââ logger.js    // 
    â
    âââ helpers.js       // è¾å©å½æ°ï¼ä¾å¦ï¼mapStateãmapGettersãmapMutations...
    âââ index.cjs.js     // commonjs æåå¥å£
    âââ index.js         // å¥å£æä»¶
    âââ index.mjs        // es6 module æåå¥å£
    âââ mixin.js         // å°vuexå®ä¾æè½½å°å¨å±Vueç$storeä¸
    âââ store.js         // æ ¸å¿æä»¶ï¼å®ä¹äºStoreç±»
    âââ util.js          // æä¾ä¸äºå·¥å·å½æ°ï¼ä¾å¦: deepCopyãisPromiseãisObject...
```



## äºãæºç éè¯»

### 1. æ¥çå·¥å·å½æ°

é¦åæä¸ªäººè§å¾è¯å®æ¯è¦çä¸ä¸ `util.js` ï¼è¿éé¢å­æ¾çæ¯æºç ä¸­é¢ç¹ç¨å°çå·¥å·å½æ°ï¼æä»¥æè§å¾è¦æåäºè§£ä¸ä¸æ¯ä¸ªå½æ°çä½ç¨æ¯ä»ä¹

```js
/**
 * Get the first item that pass the test
 * by second argument function
 *
 * @param {Array} list
 * @param {Function} f
 * @return {*}
 */

// æ¾å°æ°ç»listä¸­ç¬¬ä¸ä¸ªç¬¦åè¦æ±çåç´ 
export function find (list, f) {
  return list.filter(f)[0]
}

/**
 * æ·±æ·è´
 * 
 * @param {*} obj
 * @param {Array<Object>} cache
 * @return {*}
 */
export function deepCopy (obj, cache = []) {
  // just return if obj is immutable value
  if (obj === null || typeof obj !== 'object') {
    return obj
  }

  // if obj is hit, it is in circular structure
  const hit = find(cache, c => c.original === obj)
  if (hit) {
    return hit.copy
  }

  const copy = Array.isArray(obj) ? [] : {}
  // put the copy into cache at first
  // because we want to refer it in recursive deepCopy
  cache.push({
    original: obj,
    copy
  })

  Object.keys(obj).forEach(key => {
    copy[key] = deepCopy(obj[key], cache)
  })

  return copy
}

// éåobjå¯¹è±¡çæ¯ä¸ªå±æ§çå¼
export function forEachValue (obj, fn) {
  Object.keys(obj).forEach(key => fn(obj[key], key))
}

// å¤æ­æ¯å¦ä¸ºå¯¹è±¡ï¼æé¤nullï¼
export function isObject (obj) {
  return obj !== null && typeof obj === 'object'
}

// å¤æ­æ¯å¦ä¸ºPromiseå¯¹è±¡
export function isPromise (val) {
  return val && typeof val.then === 'function'
}

// æ­è¨
export function assert (condition, msg) {
  if (!condition) throw new Error(`[vuex] ${msg}`)
}

// ä¿çåå§åæ°çé­åå½æ°
export function partial (fn, arg) {
  return function () {
    return fn(arg)
  }
}
```

æ¯ä¸ªå½æ°çä½ç¨æé½åä¸äºæ³¨éï¼ç¨å¾®éè¯»ä¸ä¸åºè¯¥å¯ä»¥æç½å¶ä½ç¨

### 2. å¥å£æä»¶

æä¸»è¦çä»£ç é½å¨ `src` ç®å½ä¸ï¼æä»¥ä»¥ä¸æå°çæä»¶é½æ¯é»è®¤ `src` ç®å½ä¸çæä»¶

é¦åï¼è¯å®ä»å¥å£æä»¶ `index.js` å¼å§çï¼ä½è½åç°çæ¯ï¼è¿æ `index.cjs` å `index.mjs` ï¼è¿ä¸¤èåå«æ¯ `commonjs` å `es6 module` çæåå¥å£ï¼æä»¬å°±ä¸ç¨ç®¡äº

```js
import { Store, install } from './store'
import { mapState, mapMutations, mapGetters, mapActions, createNamespacedHelpers } from './helpers'
import createLogger from './plugins/logger'

export default {
  Store,
  install,
  version: '__VERSION__',
  mapState,
  mapMutations,
  mapGetters,
  mapActions,
  createNamespacedHelpers,
  createLogger
}

export {
  Store,
  install,
  mapState,
  mapMutations,
  mapGetters,
  mapActions,
  createNamespacedHelpers,
  createLogger
}
```

ä»å¥å£æä»¶ä¸­å¯ä»¥çå°ï¼ä¸»è¦å¯¼åºäº `Store` ç±» ã`install` æ¹æ³ä»¥åä¸äºè¾å©å½æ°ï¼mapStateãmapMutationsãmapGetters...ï¼

é£ä¹æä»¬ä¸»è¦ççå°±æ¯ `vuex` çæ ¸å¿ä»£ç ï¼å³ `store.js` ï¼å¯ä»¥çå° `Store` ç±»å°±åºèªäºè¿ä¸ªæä»¶

### 3. Storeç±»çå®ç°

æ´ä¸ª `Store` ç±»çä¸»è¦é»è¾é½å¨å®çæé å½æ° `constructor` ä¸­ï¼å æ­¤æä»¬å°±ä» `constructor` ä¸­åæ­¥å»æé»è¾ãçä»£ç 

#### 3.1 å­æ¾ç±»çç¶æ

é¦åæ¯å®ä¹äºä¸äºå®ä¾ç¶æï¼ç¨äºå­æ¾æ¨¡åã`mutations` ã`actions` ã`getters` ç¼å­ç­ä¸è¥¿

```js
const {
  plugins = [],
  strict = false
} = options      // çæStoreç±»çå¥å

this._committing = false        // è¡¨ç¤ºæäº¤çç¶æï¼å½éè¿mutationsæ¹æ³æ¹åstateæ¶ï¼è¯¥ç¶æä¸ºtrueï¼stateå¼æ¹åå®åï¼è¯¥ç¶æåä¸ºfalse; å¨ä¸¥æ ¼æ¨¡å¼ä¸ä¼çå¬stateå¼çæ¹åï¼å½æ¹åæ¶ï¼_committingä¸ºfalseæ¶ï¼ä¼ååºè­¦åï¼å³è¡¨æstateå¼çæ¹åä¸æ¯ç»è¿mutationsç

this._actions = Object.create(null)  // ç¨äºè®°å½ææå­å¨çactionsæ¹æ³åç§°ï¼åæ¬å¨å±çåå½åç©ºé´åçï¼ä¸åè®¸éå¤å®ä¹ï¼      

this._actionSubscribers = []       // å­æ¾actionsæ¹æ³è®¢éçåè°å½æ°

this._mutations = Object.create(null)  // ç¨äºè®°å½ææå­å¨ççmutationsæ¹æ³åç§°ï¼åæ¬å¨å±çåå½åç©ºé´åçï¼ä¸åè®¸éå¤å®ä¹ï¼

this._wrappedGetters = Object.create(null)  // æ¶éæææ¨¡ååè£åççgettersï¼åæ¬å¨å±çåå½åç©ºé´åçï¼ä½ä¸åè®¸éå¤å®ä¹ï¼

this._modules = new ModuleCollection(options)  // æ ¹æ®ä¼ å¥çoptionséç½®ï¼æ³¨ååä¸ªæ¨¡åï¼æ­¤æ¶åªæ¯æ³¨åãå»ºç«å¥½äºåä¸ªæ¨¡åçå³ç³»ï¼å·²ç»å®ä¹äºåä¸ªæ¨¡åçstateç¶æï¼ä½gettersãmutationsç­æ¹æ³ææªæ³¨å

this._modulesNamespaceMap = Object.create(null)   // å­å¨å®ä¹äºå½åç©ºé´çæ¨¡å

this._subscribers = []    // å­æ¾mutationsæ¹æ³è®¢éçåè°

this._watcherVM = new Vue()  // ç¨äºçå¬stateãgetters

this._makeLocalGettersCache = Object.create(null)   // gettersçæ¬å°ç¼å­
```

å³äºåä¸ªåéç¶æçä½ç¨é½åå¨è¿äºï¼å¶ä¸­åªæ `this._modules = new ModuleCollection(option)` æ§è¡äºä¸äºæä½ï¼å¶ä½ç¨å°±æ¯è¿è¡**æ¨¡åéå½æ¶é**ï¼æ ¹æ® `ModuleCollection` çæ¥æºï¼æä»¬ç§»æ­¥å° `./module/module-collection.js` æä»¶

##### 3.1.1 éå½æ¶éæ¨¡å

å¨ `Module-collection.js` æä»¶ä¸­å®ä¹äº `ModuleCollection` ç±»ï¼å¶ä½ç¨å°±æ¯éè¿éå½éå `options` å¥åï¼å°æ¯ä¸ªæ¨¡åé½çæä¸ä¸ªç¬ç«ç `Moudle`

è¿éåæ¥çæä¸ä¸ `options` çç»æï¼å¦ä¸ï¼

```js
import Vuex from 'vuex'

const options = {
  state: {...},
  getters: {...},
  mutations: {...},
  actions: {...},
  modules: {
    ModuleA: {
      state: {...},
      ...
      modules: {
        ModuleA1: {...}
      }
    },
    ModuleB: {
      state: {...},
      ...
      modules: {
        ModuleB1: {...}
      }
    }
  }
}

const store = new Vuex.Store(options)

export default store
```

å¯ä»¥çå°ä¼ å¥ç `options` æ´ä½å¯ä»¥çæä¸ä¸ªæ ¹æ¨¡å `root` ï¼ç¶å `root` ç `modules` ä¸­åµå¥çå¦å¤ä¸¤ä¸ªå­æ¨¡åï¼`ModuleA` å`ModuleB` ï¼è `ModuleA` å`ModuleB` åé¨ä¹åå«åµå¥çä¸ä¸ªå­æ¨¡åï¼åå«ä¸º `ModuleA1` ã`ModuleB1` ãè¿æ ·å°±ç»æäºä¸ä¸ªæ¨¡åæ ï¼å æ­¤ `ModuleCollection` ç±»çå·¥ä½å°±æ¯å°ä¿çåæ¥çæ¨¡åå³ç³»ï¼å°æ¯ä¸ªæ¨¡åå°è£å°ä¸ä¸ª `Module` ç±»ä¸­

```js
export default class ModuleCollection {
  constructor (rawRootModule) {
    // éå½æ³¨åæ¨¡å
    this.register([], rawRootModule, false)
  }
  
  // æ ¹æ®è·¯å¾é¡ºåºï¼ä»æ ¹æ¨¡åå¼å§éå½è·åå°æä»¬åå¤æ·»å æ°çæ¨¡åçç¶æ¨¡å
  get (path) {
    return path.reduce((module, key) => {
      return module.getChild(key)
    }, this.root)
  }
  
  // éå½æ³¨åæ¨¡å
  register (path, rawModule, runtime = true) {
    if (__DEV__) {
      assertRawModule(path, rawModule)
    }
    
    const newModule = new Module(rawModule, runtime)  // åå§åä¸ä¸ªæ°çæ¨¡å
    if (path.length === 0) {    // å½åæ²¡æå«çæ¨¡å
      this.root = newModule     // åæ­¤æ¨¡åä¸ºæ ¹æ¨¡å
    } else {    // æå¤ä¸ªæ¨¡å     
      const parent = this.get(path.slice(0, -1))   // è·åå°æ°æ¨¡åä»å±çç¶æ¨¡åï¼æä»¥æ¯path.slice(0, -1)ï¼æåä¸ä¸ªåç´ å°±æ¯æä»¬è¦æ·»å çå­æ¨¡åçåç§°
      parent.addChild(path[path.length - 1], newModule)    // å¨ç¶æ¨¡åä¸­æ·»å æ°çå­æ¨¡å
    }

    if (rawModule.modules) {     // å¦ææåµå¥æ¨¡å
      /**
       *  1. éåææçå­æ¨¡åï¼å¹¶è¿è¡æ³¨å;
       *  2. å¨pathä¸­å­å¨é¤äºæ ¹æ¨¡åä»¥å¤ææå­æ¨¡åçåç§°
       *  */ 
      forEachValue(rawModule.modules, (rawChildModule, key) => {
        this.register(path.concat(key), rawChildModule, runtime)
      })
    }
  }
}
```

**å½æ°ä½ç¨ï¼**

1. `register(path, rawModule, runtime)`ï¼æ³¨åæ°çæ¨¡åï¼å¹¶æ ¹æ®æ¨¡åçåµå¥å³ç³»ï¼å°æ°æ¨¡åæ·»å ä½ä¸ºå¯¹åºæ¨¡åçå­æ¨¡å

- pathï¼è¡¨ç¤ºæ¨¡ååµå¥å³ç³»ãå½åä¸ºæ ¹æ¨¡åæ¶ï¼æ²¡æä»»ä½åµå¥å³ç³»ï¼æ­¤æ¶ `path = []` ; å½åä¸æ¯æ ¹æ¨¡åæ¶ï¼å­å¨åµå¥å³ç³»ï¼ä¾å¦ä¸è¿°ä¾å­ä¸­ç `ModuleA1` ï¼å®æ¯ `ModuleA` çå­æ¨¡å ï¼è `ModuleA` åæ¯æ ¹æ¨¡åçå­æ¨¡åï¼æ­¤æ¶ `path = ['ModuleA', 'ModuleA1']`
- rawModuleï¼è¡¨ç¤ºæ¨¡åå¯¹è±¡ï¼æ­¤æ¶æ¯ä¸ä¸ªå¯¹è±¡ç±»å
- runtimeï¼è¡¨ç¤ºç¨åºè¿è¡æ¶



2. `get(path)`ï¼æ ¹æ®ä¼ å¥ç `path` è·¯å¾ï¼è·åå°æä»¬æ³è¦ç `Module` ç±»

   

`ModuleCollection` çæé å½æ°ä¸­è°ç¨äº `register` å½æ°ï¼åä¸¤ä¸ªåæ°åå«ä¸ºï¼`[]` ã`rawRootModule` ï¼æ­¤æ¶è¯å®æ¯ä»æ ¹æ¨¡åå¼å§æ³¨åçï¼æä»¥ `path` éæ åå®¹ï¼å¹¶ä¸ `rawRootModule` æåçæ¯æ ¹æ¨¡å



ç¶åæ¥çä¸ä¸ `register` å½æ°éçé»è¾ã

1. é¦åå°å½åè¦æ³¨åçæ¨¡åçæä¸ä¸ª `Module` ï¼å¹¶å° `rawModule` ä½ä¸ºåæ°ï¼ç¨äºå­æ¾ `Module` çä¿¡æ¯

2. ç¶åéè¿ `if(path.length === 0)` å¤æ­æ¯å¦ä¸ºæ ¹æ¨¡åï¼æ¯çè¯å°±å° `this.root` æå `Module` ; å¦åå°±è·³å°ç¬¬3æ­¥
3. å¤æ­å½åæ¨¡åä¸æ¯æ ¹æ¨¡åï¼å°±éè¿ `get` å½æ°æ¾å°å½åæ¨¡åçç¶æ¨¡åï¼ç¶åè°ç¨ç¶æ¨¡åä¸­ç `addChild` æ¹æ³å°å½åæ¨¡åæ·»å å°å­æ¨¡åä¸­
4. æååå¤æ­å½åæ¨¡åæ¯å¦è¿æåµå¥çæ¨¡åï¼æçè¯å°±éæ°åå°ç¬¬1æ­¥è¿è¡éå½æä½ ; å¦åä¸åä»»ä½å¤ç



æç§ä¸é¢çé»è¾ï¼å°±å¯ä»¥å°ææçæ¨¡åéå½æ¶éå¹¶æ³¨åå¥½äºï¼å¶ä¸­æä¸ä¸ª `Module` ç±»è¿æ²¡æå·ä½æå°ï¼æä»¥è¿éç§»æ­¥å° `./module/module.js` 

```js
import { forEachValue } from '../util'

// å®ä¹äºVuexä¸­ç Module ç±»ï¼åå«äºstateãmutationsãgettersãactionsãmodules
export default class Module {
  constructor (rawModule, runtime) {
    this.runtime = runtime
    
    this._children = Object.create(null)   // åå»ºä¸ä¸ªç©ºå¯¹è±¡ï¼ç¨äºå­æ¾å½åæ¨¡åçå­æ¨¡å
    
    this._rawModule = rawModule         // å½åæ¨¡åçä¸äºä¿¡æ¯ï¼ä¾å¦ï¼stateãmutationsãgettersãactionsãmodules
    const rawState = rawModule.state    // 1. å½æ°ç±»å => è¿åä¸ä¸ªobjå¯¹è±¡; 2. ç´æ¥è·åå°objå¯¹è±¡

    // å­å¨å½åæ¨¡åçstateç¶æ
    this.state = (typeof rawState === 'function' ? rawState() : rawState) || {}   
  }

  // å¤æ­è¯¥æ¨¡åæ¯å¦å®ä¹äºnamespacedï¼å®ä¹äºåè¿åtrue; å¦åè¿åfalse
  get namespaced () {
    return !!this._rawModule.namespaced
  }

  // æ·»å å­æ¨¡åï¼åç§°ä¸ºkey
  addChild (key, module) {
    this._children[key] = module
  }

  // ç§»é¤åç§°ä¸ºkeyçå­æ¨¡å
  removeChild (key) {
    delete this._children[key]
  }

  // è·ååç§°ä¸ºkeyçå­æ¨¡å
  getChild (key) {
    return this._children[key]
  }

  // æ¯å¦å­å¨åç§°ä¸ºkeyçå­æ¨¡å
  hasChild (key) {
    return key in this._children
  }
	
  // å°å½åæ¨¡åçå½åç©ºé´æ´æ°å°æå®æ¨¡åçå½åç©ºé´ä¸­ï¼å¹¶åæ¶æ´æ°ä¸ä¸actionsãmutationsãgettersçè°ç¨æ¥æº
  update (rawModule) {
    this._rawModule.namespaced = rawModule.namespaced
    if (rawModule.actions) {
      this._rawModule.actions = rawModule.actions
    }
    if (rawModule.mutations) {
      this._rawModule.mutations = rawModule.mutations
    }
    if (rawModule.getters) {
      this._rawModule.getters = rawModule.getters
    }
  }

  // éåå½åæ¨¡åçææå­æ¨¡åï¼å¹¶æ§è¡åè°æä½
  forEachChild (fn) {
    forEachValue(this._children, fn)
  }

  // éåå½åæ¨¡åçæægettersï¼å¹¶æ§è¡åè°æä½
  forEachGetter (fn) {
    if (this._rawModule.getters) {
      forEachValue(this._rawModule.getters, fn)
    }
  }

  // éåå½åæ¨¡åçææactionsï¼å¹¶æ§è¡åè°æä½
  forEachAction (fn) {
    if (this._rawModule.actions) {
      forEachValue(this._rawModule.actions, fn)
    }
  }

  // éåå½åæ¨¡åçææmutationsï¼å¹¶æ§è¡åè°æä½
  forEachMutation (fn) {
    if (this._rawModule.mutations) {
      forEachValue(this._rawModule.mutations, fn)
    }
  }
}
```

æ¥çä¸ä¸åææ¨¡åæ¶éæ¶ï¼åå»ºç `Module` ç±»åé¨åäºä»ä¹äºæï¼åæ ·çä» `constructor` ä¸­å¼å§ç

`this._children` æ¯ä¸ä¸ªå¯¹è±¡å¼ï¼ç¨äºå­æ¾è¯¥æ¨¡ååµå¥çå¶å® `Module` ç±» ;

`this._rawModule` å°±æ¯ç¨äºå­æ¾è¯¥æ¨¡ååé¨çä¸äºä¿¡æ¯ï¼ä¾å¦ï¼`state` ã`mutations` ã`actions` ã`getters` ã`moudles` ;

`this.state` å¯¹åºçå°±æ¯ `this._rawModule` ä¸­ç `state` ;

 è¿æ¯æ´ä¸ªæé å½æ°ä¸­æ§è¡çæä½ï¼æä»¬å¯ä»¥çå°ï¼å¨çæä¸ä¸ª `Module` ç±»çæ¶åï¼å¶åªå®ä¹äº `state` å±æ§ï¼è `mutations` ã`getters` ã`actions` ã`modules` é½æ¯æ²¡æè¢«å®ä¹çï¼å³ä¾å¦ç°å¨æ¯æ æ³éè¿ `Module.mutations` è·åå°è¯¥æ¨¡åææç `mutations` æ¹æ³ï¼é£ä¹è¿äºæ¹æ³é½æ¯å¨ä½æ¶è¢«å®ä¹çå¢ï¼èªç¶æ¯ç­æ¨¡åå¨é¨é½æ¶éå®æ¯ä»¥åæè¿è¡çæä½ï¼å ä¸º `vuex` ä¸­çåµå¥æ¨¡åå¯è½ä¼å­å¨å½åç©ºé´ `namespaced` 

#### 3.2 æ³¨åæ¨¡å

å°æ­¤ä¸ºæ­¢ï¼åä¸ªæ¨¡åçç±»é½åå»ºå¥½äºï¼é£ä¹ç»§ç»­åå° `./src/store.js` ç `constructor` æé å½æ°ä¸­

```js
// å° dispatch å commit æ¹æ³ç»å®å° Store çå®ä¾ä¸ï¼é¿ååç»­ä½¿ç¨dispatchæcommitæ¶æ¹åäºthisæå
const store = this
const { dispatch, commit } = this
this.dispatch = function boundDispatch (type, payload) {
  return dispatch.call(store, type, payload)
}
this.commit = function boundCommit (type, payload, options) {
  return commit.call(store, type, payload, options)
}

// å¤æ­storeæ¯å¦æªä¸¥æ ¼æ¨¡å¼ãtrue: ææçstateé½å¿é¡»ç»è¿mutationsæ¥æ¹å
this.strict = strict

// å°æ ¹æ¨¡åçstateèµå¼ç»stateåé
const state = this._modules.root.state
```

è¿æ®µä»£ç é¦åå¯¹ `Store` å®ä¾ä¸ç `dispatch` å `commit` æ¹æ³è¿è¡äºä¸å±åè£ï¼å³éè¿ `call` å°è¿ä¸¤ä¸ªæ¹æ³çä½ç¨å¯¹è±¡æåå½åç `Store` å®ä¾ï¼è¿æ ·å°±è½é²æ­¢åç»­æä»¬æä½æ¶ï¼åºç° `this.$store.dispatch.call(obj, 1)` ç±»ä¼¼çæåµèæ¥é

 `this.strict` æ¯ç¨äºå¤æ­æ¯å¦æ¯ä¸¥æ ¼æ¨¡å¼ãå ä¸º `vuex` ä¸­ï¼å»ºè®®ææç `state` åéçååé½å¿é¡»ç»è¿ `mutations` æ¹æ³ï¼å ä¸ºè¿æ ·æè½è¢« `devtool` æè®°å½ä¸æ¥ï¼æä»¥å¨ä¸¥æ ¼æ¨¡å¼ä¸ï¼æªç»è¿ `mutations` èç´æ¥æ¹åäº `state` çå¼ï¼å¼åç¯å¢ä¸ä¼ååºè­¦åâ ï¸

`const state = this._modules.root.state`  è·åçæ¯æ ¹æ¨¡åç `state` ï¼ç¨äºåç»­çä¸äºæä½

ä¸åé½åå¤å°±ç»ªäºï¼ä¸é¢å°±å¼å§ä¸ºæ¯ä¸ªæ¨¡åæ³¨åä¿¡æ¯äº

```js
// ä»æ ¹æ¨¡åå¼å§ï¼éå½å®ååä¸ªæ¨¡åçä¿¡æ¯
installModule(this, state, [], this._modules.root)
```

è°ç¨äº `installModule` æ¹æ³ï¼å¹¶å° `store` å®ä¾å¯¹è±¡ ã`state` å±æ§ ãè·¯å¾ ãæ ¹æ¨¡åå¯¹è±¡ä¾æ¬¡ä½ä¸ºåæ°è¿è¡ä¼ é

```js
// æ³¨åå®ååä¸ªæ¨¡ååçä¿¡æ¯
function installModule (store, rootState, path, module, hot) {
  const isRoot = !path.length  // æ¯å¦ä¸ºæ ¹æ¨¡å
  const namespace = store._modules.getNamespace(path)  // è·åå½åæ¨¡åçå½åç©ºé´ï¼æ ¼å¼ä¸ºï¼second/ æ second/third/

  // å¦æå½åæ¨¡åè®¾ç½®äºnamespaced æ ç»§æ¿äºç¶æ¨¡åçnamespacedï¼åå¨modulesNamespaceMapä¸­å­å¨ä¸ä¸å½åæ¨¡å
  if (module.namespaced) {
    if (store._modulesNamespaceMap[namespace] && __DEV__) {
      console.error(`[vuex] duplicate namespace ${namespace} for the namespaced module ${path.join('/')}`)
    }
    store._modulesNamespaceMap[namespace] = module
  }

  // å¦æä¸æ¯æ ¹æ¨¡åï¼å°å½åæ¨¡åçstateæ³¨åå°å¶ç¶æ¨¡åçstateä¸
  if (!isRoot && !hot) {
    const parentState = getNestedState(rootState, path.slice(0, -1)) // è·åç¶æ¨¡åçstate
    const moduleName = path[path.length - 1]   // å½åæ¨¡åçåç§°
    store._withCommit(() => {
      if (__DEV__) {
        if (moduleName in parentState) {
          console.warn(
            `[vuex] state field "${moduleName}" was overridden by a module with the same name at "${path.join('.')}"`
          )
        }
      }
      // å°å½åæ¨¡åçstateæ³¨åå¨ç¶æ¨¡åçstateä¸ï¼å¹¶ä¸æ¯ååºå¼ç
      Vue.set(parentState, moduleName, module.state)
    })
  }

  // è®¾ç½®å½åæ¨¡åçä¸ä¸æcontext
  const local = module.context = makeLocalContext(store, namespace, path)

  // æ³¨åæ¨¡åçææmutations
  module.forEachMutation((mutation, key) => {
    const namespacedType = namespace + key     // ä¾å¦ï¼first/second/mutations1
    registerMutation(store, namespacedType, mutation, local)
  })

  // æ³¨åæ¨¡åçææactions
  module.forEachAction((action, key) => {
    /**
     * actionsæä¸¤ç§åæ³ï¼
     * 
     * actions: {
     *    AsyncAdd (context, payload) {...},   // ç¬¬ä¸ç§åæ³
     *    AsyncDelete: {                       // ç¬¬äºç§åæ³
     *      root: true,
     *      handler: (context, payload) {...}
     *    } 
     * }
     */
    const type = action.root ? key : namespace + key   // å¤æ­æ¯å¦éè¦å¨å½åç©ºé´éæ³¨åä¸ä¸ªå¨å±çaction
    const handler = action.handler || action          // è·åactionså¯¹åºçå½æ°
    registerAction(store, type, handler, local)   
  })

  // æ³¨åæ¨¡åçæægetters
  module.forEachGetter((getter, key) => {
    const namespacedType = namespace + key
    registerGetter(store, namespacedType, getter, local)
  })

  // éå½æ³¨åå­æ¨¡å
  module.forEachChild((child, key) => {
    installModule(store, rootState, path.concat(key), child, hot)
  })
}
```

`const namespace = store._modules.getNamespace(path)` æ¯å°è·¯å¾ `path` ä½ä¸ºåæ°ï¼ è°ç¨ `ModuleCollection` ç±»å®ä¾ä¸ç `getNamespace` æ¹æ³æ¥è·åå½åæ³¨åå¯¹è±¡çå½åç©ºé´ç

```js
/**
* æ ¹æ®æ¨¡åæ¯å¦æå½åç©ºé´æ¥è®¾å®ä¸ä¸ªè·¯å¾åç§°
* ä¾å¦ï¼Aä¸ºç¶æ¨¡åï¼Bä¸ºå­æ¨¡åï¼Cä¸ºå­å­æ¨¡å
* 1. è¥Bæ¨¡åå½åç©ºé´ä¸ºsecond,Cæ¨¡åæªè®¾å®å½åç©ºé´æ¶; Cæ¨¡åç»§æ¿äºBæ¨¡åçå½åç©ºé´ï¼ä¸º second/
* 2. è¥Bæ¨¡åæªè®¾å®å½åç©ºé´, Bæ¨¡åå½åç©ºé´ä¸ºthird; åæ­¤æ¶Bæ¨¡åç»§æ¿çæ¯Aæ¨¡åçå½åç©ºé´ï¼èCæ¨¡åçå½åç©ºé´è·¯å¾ä¸º third/
*/
getNamespace (path) {
  let module = this.root
  return path.reduce((namespace, key) => {
    module = module.getChild(key)   // è·åå­æ¨¡å
    return namespace + (module.namespaced ? key + '/' : '')
  }, '')
}
```

ä»è¿å¯ä»¥çåºï¼æªæå®å½åç©ºé´çæ¨¡åä¼ç»§æ¿ç¶æ¨¡åçå½åç©ºé´

```js
  // å¦æå½åæ¨¡åè®¾ç½®äºnamespaced æ ç»§æ¿äºç¶æ¨¡åçnamespacedï¼åå¨modulesNamespaceMapä¸­å­å¨ä¸ä¸å½åæ¨¡å
if (module.namespaced) {
  if (store._modulesNamespaceMap[namespace] && __DEV__) {
    console.error(`[vuex] duplicate namespace ${namespace} for the namespaced module ${path.join('/')}`)
  }
  store._modulesNamespaceMap[namespace] = module
}
```

è¿æ®µä»£ç æ¯å°ææå­å¨å½åç©ºé´çæ¨¡åè®°å½å¨ `store._modulesNamespaceMap` ä¸­ï¼ä¾¿äºä¹åçè¾å©å½æ°å¯ä»¥è°ç¨ï¼è¿éè¿æªæå°è¾å©å½æ°ï¼å¯ä»¥åä¸ç®¡ï¼å°æ¶ååå¤´æ¥çï¼

##### 3.2.1 æ³¨åæ¨¡åçstate

```js
// å¦æä¸æ¯æ ¹æ¨¡åï¼å°å½åæ¨¡åçstateæ³¨åå°å¶ç¶æ¨¡åçstateä¸
if (!isRoot && !hot) {
  const parentState = getNestedState(rootState, path.slice(0, -1)) // è·åç¶æ¨¡åçstate
  const moduleName = path[path.length - 1]   // å½åæ¨¡åçåç§°
  store._withCommit(() => {
    if (__DEV__) {
      if (moduleName in parentState) {
        console.warn(
          `[vuex] state field "${moduleName}" was overridden by a module with the same name at "${path.join('.')}"`
        )
      }
    }
    // å°å½åæ¨¡åçstateæ³¨åå¨ç¶æ¨¡åçstateä¸ï¼å¹¶ä¸æ¯ååºå¼ç
    Vue.set(parentState, moduleName, module.state)
  })
}
```

è¿æ®µä»£ç ä¸»è¦æ¯å°éæ ¹æ¨¡åç `state` æè½½å°ç¶æ¨¡åç `state` ä¸

`const parentState = getNestedState(rootState, path.slice(0, -1))` æ ¹æ®å½åçæ¨¡åè·¯å¾ï¼ä»æ ¹æ¨¡åç `state` å¼å§æ¾ï¼æç»æ¾å°å½åæ¨¡åçç¶æ¨¡åç `state`ï¼å¯ä»¥çä¸ä¸ `getNestedState` æ¹æ³åé¨çå·ä½å®ç°

```js
// è·åå°åµå¥çæ¨¡åä¸­çstate
function getNestedState (state, path) {
  return path.reduce((state, key) => state[key], state)
}
```

`const moduleName = path[path.length - 1]` ä»è·¯å¾ `path` ä¸­å°å½åæ¨¡åçåç§°æååºæ¥

```js
store._withCommit(() => {
  if (__DEV__) {
    if (moduleName in parentState) {
      console.warn(
        `[vuex] state field "${moduleName}" was overridden by a module with the same name at "${path.join('.')}"`
      )
    }
  }
  // å°å½åæ¨¡åçstateæ³¨åå¨ç¶æ¨¡åçstateä¸ï¼å¹¶ä¸æ¯ååºå¼ç
  Vue.set(parentState, moduleName, module.state)
})
```

è¿æ®µä»£ç ä¸­æä¸»è¦çé¨åå°±æ¯ `Vue.set(parentState, moduleName, module.state)` ï¼ä½ç¨å°±æ¯è°ç¨äº `Vue` ç `set` æ¹æ³å°å½åæ¨¡åç `state` ååºå¼å°æ·»å å°äºç¶æ¨¡åç `state` ä¸ï¼è¿æ¯å ä¸ºå¨ä¹åæä»¬ä¼çå° `state` ä¼è¢«æ¾å°ä¸ä¸ªæ°ç `Vue` å®ä¾ç `data` ä¸­ï¼æä»¥è¿éä¸å¾ä¸ä½¿ç¨ `Vue` ç `set` æ¹æ³æ¥ååºå¼å°æ·»å 

åæ ·çï¼ä»è¿æ®µä»£ç ä¸­æä»¬ä¹å¯ä»¥ç¥éäºä¸ºä»ä¹å¹³æ¶å¨è·åå­æ¨¡åä¸ `state` çå±æ§æ¶ï¼æ¯éè¿ `this.$store.state.ModuleA.name` è¿æ ·çå½¢å¼æ¥è·åçäº

##### 3.2.2 çææ¨¡åè°ç¨ä¸ä¸æ

```js
// è®¾ç½®å½åæ¨¡åçä¸ä¸æcontext
const local = module.context = makeLocalContext(store, namespace, path)
```

è¿è¡ä»£ç ä¹å¯ä»¥è¯´æ¯éå¸¸æ ¸å¿çä¸æ®µä»£ç äºï¼å®æ ¹æ®å½åç©ºé´ä¸ºæ¯ä¸ªæ¨¡ååå»ºäºä¸ä¸ªå±äºè¯¥æ¨¡åè°ç¨çä¸ä¸æï¼å¹¶å°è¯¥ä¸ä¸æèµå¼äºç»äºè¯¥æ¨¡åç `context` å±æ§

æ¥ä¸æ¥çä¸ä¸è¿ä¸ªä¸ä¸ææ¯å¦ä½åå»ºçå§

```js
// è¥è®¾ç½®äºå½åç©ºé´ååå»ºä¸ä¸ªæ¬å°çcommitãdispatchæ¹æ³ï¼å¦åå°ä½¿ç¨å¨å±çstore
function makeLocalContext (store, namespace, path) {
  const noNamespace = namespace === ''  

  const local = {
    dispatch: noNamespace ? store.dispatch : (_type, _payload, _options) => {
      const args = unifyObjectStyle(_type, _payload, _options)
      const { payload, options } = args
      let { type } = args

      if (!options || !options.root) {  // è¥ä¼ å¥äºç¬¬ä¸ä¸ªåæ°è®¾ç½®äºroot:trueï¼åæ´¾åçæ¯å¨å±ä¸å¯¹åºççactionsæ¹æ³
        type = namespace + type
        if (__DEV__ && !store._actions[type]) {
          console.error(`[vuex] unknown local action type: ${args.type}, global type: ${type}`)
          return
        }
      }

      return store.dispatch(type, payload)
    },

    commit: noNamespace ? store.commit : (_type, _payload, _options) => {
      const args = unifyObjectStyle(_type, _payload, _options)
      const { payload, options } = args
      let { type } = args

      if (!options || !options.root) {   // è¥ä¼ å¥äºç¬¬ä¸ä¸ªåæ°è®¾ç½®äºroot:trueï¼åæ´¾åçæ¯å¨å±ä¸å¯¹åºççmutationsæ¹æ³
        type = namespace + type
        if (__DEV__ && !store._mutations[type]) {
          console.error(`[vuex] unknown local mutation type: ${args.type}, global type: ${type}`)
          return
        }
      }

      store.commit(type, payload, options)
    }
  }

  /**
   * è¥æ²¡æè®¾å®å½åç©ºé´ï¼åç´æ¥è¯»åstore.gettersï¼store.getterså·²ç»æè½½å°vueå®ä¾çcomputedä¸äºï¼;
   * è¥è®¾å®äºå½åç©ºé´ï¼åä»æ¬å°ç¼å­_makeLocalGettersCacheä¸­è¯»ågetters
   */
  Object.defineProperties(local, {
    getters: {
      get: noNamespace
        ? () => store.getters    
        : () => makeLocalGetters(store, namespace)
    },
    state: {
      get: () => getNestedState(store.state, path)
    }
  })

  return local
}
```

`local` è¿ä¸ªåéå­å¨çå°±æ¯ä¸ä¸ªæ¨¡åçä¸ä¸æã

åæ¥çå¶ç¬¬ä¸ä¸ªå±æ§ `dispatch` ï¼å½è¯¥æ¨¡åæ²¡æè®¾ç½®å½åç©ºé´æ¶ï¼è°ç¨è¯¥ä¸ä¸æç `dispatch` æ¹æ³æ¶ä¼ç´æ¥è°ç¨ `sotre.dispatch` ï¼å³è°ç¨äºæ ¹æ¨¡åç `dispatch` æ¹æ³ ; èå­å¨å½åç©ºé´æ¶ï¼ä¼åå¤æ­ç¸åºçå½åç©ºé´ï¼ä»¥æ­¤æ¥å³å®è°ç¨åªä¸ª `dispatch` æ¹æ³

`if (!options || !options.root)` æ¯å¤æ­è°ç¨ `dispatch` æ¹æ³æ¶ææ²¡æä¼ å¥ç¬¬ä¸ä¸ªåæ° `{root: true}` ï¼è¥æåè¡¨ç¤ºè°ç¨å¨å±æ ¹æ¨¡åä¸å¯¹åºçç `dispatch` æ¹æ³

é£ä¹åæ ·çï¼`local` ä¸­ç `commit` å±æ§å°±ç±»ä¼¼äº `dispatch` ï¼è¿éå°±ä¸å¤è¯´äº

ç¶åæåéè¿ `Object.defineProperties` æ¹æ³å¯¹ `local` ç `getters` å±æ§å `state` å±æ§è®¾ç½®äºä¸å±è·åä»£çï¼ç­åç»­å¯¹å¶è®¿é®æ¶ï¼æä¼è¿è¡å¤çãä¾å¦ï¼è®¿é® `getters` å±æ§æ¶ï¼åå¤æ­æ¯å¦å­å¨å½åç©ºé´ï¼è¥æ²¡æï¼åç´æ¥è¿å `store.getters` ; å¦åçè¯ï¼æ ¹æ®å½åç©ºé´åå»ºä¸ä¸ªæ¬å°ç `getters` ç¼å­ï¼æ ¹æ®è¿ä¸ªç¼å­æ¥è·åå¯¹åºç `getters` ï¼æ¥çä¸ä¸ä»£ç 

```js
// åå»ºæ¬å°çgettersç¼å­
function makeLocalGetters (store, namespace) {
  // è¥ç¼å­ä¸­æ²¡ææå®çgettersï¼ååå»ºä¸ä¸ªæ°çgettersç¼å­å°__makeLocalGettersCacheä¸­
  if (!store._makeLocalGettersCache[namespace]) {
    const gettersProxy = {}
    const splitPos = namespace.length
    Object.keys(store.getters).forEach(type => {
      // å¦æstore.gettersä¸­æ²¡æä¸namespaceå¹éçgettersï¼åä¸è¿è¡ä»»ä½æä½
      if (type.slice(0, splitPos) !== namespace) return

      // è·åæ¬å°gettersåç§°
      const localType = type.slice(splitPos)

      // å¯¹gettersæ·»å ä¸å±ä»£ç
      Object.defineProperty(gettersProxy, localType, {
        get: () => store.getters[type],
        enumerable: true
      })
    })
    // æä»£çè¿çgettersç¼å­å°æ¬å°
    store._makeLocalGettersCache[namespace] = gettersProxy
  }

  return store._makeLocalGettersCache[namespace]
}
```

å½å­å¨å½åç©ºé´æ¶è®¿é® `local.getters` ï¼é¦åä¼å» `store._makeLocalGettersCache` æ¥æ¾æ¯å¦æå¯¹åºç `getters` ç¼å­ï¼è¥æ²¡æï¼ååå»ºä¸ä¸ª `gettersProxy` ï¼å¨ `store.getters` ä¸æ¾å°å¯¹åºç `getters` ï¼ç¶åç¨ `Object.defineProperty` å¯¹ `gettersProxy` åä¸å±å¤çï¼å³å½è®¿é® `local.getters.func` æ¶ï¼ç¸å½äºè®¿é®äº `store.getters['first/func']` ï¼è¿æ ·åä¸å±ç¼å­ï¼ä¸ä¸æ¬¡è®¿é®è¯¥ `getters` æ¶ï¼å°±ä¸ä¼éæ°éå `store.getters` äº ; è¥æç¼å­ï¼åç´æ¥ä»ç¼å­ä¸­è·å

ä¸ä¸æå·²ç»åå»ºå¥½äºï¼æ¥ä¸æ¥å°±æ¯æ³¨å `mutations` ã`actions` ã`getters` äº

##### 3.2.3 æ³¨åæ¨¡åçmutations

```js
// æ³¨åæ¨¡åçææmutations
module.forEachMutation((mutation, key) => {
  const namespacedType = namespace + key     // ä¾å¦ï¼first/second/mutations1
  registerMutation(store, namespacedType, mutation, local)
})
```

è¿ééåäºæ¨¡åçææ `mutations` æ¹æ³ï¼éè¿å½åç©ºé´ + `mutations` æ¹æ³åçå½¢å¼çæäº `namespacedType`

ç¶åè·³å° `registerMutations` æ¹æ³ççå·ä½æ¯å¦ä½æ³¨åç

```js
// æ³¨åmutationsæ¹æ³
function registerMutation (store, type, handler, local) {
  const entry = store._mutations[type] || (store._mutations[type] = [])  // éè¿store._mutations è®°å½æææ³¨åçmutations
  entry.push(function wrappedMutationHandler (payload) {
    handler.call(store, local.state, payload)
  })
}
```

é¦åæ ¹æ®æä»¬ä¼ å¥ç `type` ä¹å°±æ¯ä¸é¢ç `namespacedType` å» `store._mutations` å¯»æ¾æ¯å¦æå¥å£ `entry` ï¼è¥æåç´æ¥è·å ; å¦åå°±åå»ºä¸ä¸ªç©ºæ°ç»ç¨äºå­å¨ `mutations` æ¹æ³

å¨è·åå° `entry` ä»¥åï¼å°å½åç `mutations` æ¹æ³æ·»å å° `entry` æ«å°¾è¿è¡å­å¨ãå¶ä¸­ `mutations` æ¥æ¶çåæ°æä¸¤ä¸ªï¼å³ ä¸ä¸æä¸­ç `state` å æä»¬ä¼ å¥çåæ° `payload`

ä»è¿æ®µä»£ç æä»¬å¯ä»¥çåºï¼æ´ä¸ª `store` å®ä¾çææ `mutations` æ¹æ³é½æ¯å­å¨å¨ `store._mutations` ä¸­çï¼å¹¶ä¸æ¯ä»¥é®å¼å¯¹çå½¢å¼å­æ¾çï¼ä¾å¦ï¼

```js
store._mutations = {
  'mutations1': [function handler() {...}],
  'ModuleA/mutations2': [function handler() {...}, function handler() {...}],
  'ModuleA/ModuleB/mutations2': [function handler() {...}]
}
```

å¶ä¸­**é®**æ¯ç±å½åç©ºé´å `mutations` æ¹æ³åç»æçï¼**å¼**æ¯ä¸ä¸ªæ°ç»ï¼å­æ¾çææè¯¥é®å¯¹åºç `mutations` æ¹æ³

ä¸ºä»ä¹æ¯ç¨æ°ç»å­æ¾å¢ï¼å ä¸ºå¨ä¸é¢è¯´è¿ï¼åè®¾ç¶æ¨¡å`ModuleA` éæä¸ä¸ªå« `func` ç `mutations` æ¹æ³ï¼é£ä¹å¶å¨ `store._mutations` ä¸­å°±æ¯è¿ä¸ªæ ·å­ç

```js
store._mutations = {
  'ModuleA/func': [function handler() {...}]
}
```

 è¥å­æ¨¡åæ²¡æè®¾ç½®å½åç©ºé´ï¼é£ä¹ä»æ¯ä¼ç»§æ¿ç¶æ¨¡åçå½åç©ºé´çï¼æ­¤æ¶å­æ¨¡åéä¹æä¸ä¸ªå« `func` ç `mutations` æ¹æ³ï¼é£ä¹å¨è·å `entry ` æ¶ï¼è·åå°çæ¯ `store._mutations['ModuleA/func']` ï¼ä½æ­¤æ¶è¿ä¸ª `entry` ä¸­å·²ç»æä¸ä¸ª `mutations` æ¹æ³äºï¼é£ä¹ä¸ºäºä¿è¯ä¹åçæ¹æ³ä¸è¢«æ¿æ¢ï¼å°±éæ©æ·»å å°æ°ç»çæ«å°¾ï¼æ­¤æ¶åºè¯¥å°±å¯ä»¥çæµå°äºï¼åç»­å¦æè°ç¨è¯¥ `mutations` æ¹æ³ï¼ä¼åè·åå°ç¸åºçæ°ç»ï¼ç¶åéåä¾æ¬¡æ§è¡

å¾åºä¸ª**ç»è®º**ï¼`mutations` æ¹æ³æ¯å¯ä»¥éåç

##### 3.2.4 æ³¨åæ¨¡åçactions

```js
// æ³¨åæ¨¡åçææactions
module.forEachAction((action, key) => {
  const type = action.root ? key : namespace + key   // å¤æ­æ¯å¦éè¦å¨å½åç©ºé´éæ³¨åä¸ä¸ªå¨å±çaction
  const handler = action.handler || action          // è·åactionså¯¹åºçå½æ°
  registerAction(store, type, handler, local)   
})
```

éåæ¨¡åçææ `actions` æ¹æ³ï¼å¶ä¸­å¯¹äº `type` å `handler` çå¤çä¸»è¦æ¯ä¸ºäºå¼å®¹ä¸¤ç§åæ³ï¼

```js
// ç¬¬ä¸ç§åæ³ï¼
actions: {
  func(context, payload) {
    // çç¥ä¸å¡ä»£ç ...
  }
}

// ç¬¬äºç§åæ³ï¼
actions: {
  func: {
    root: true,
    handler(context, payload) {
      // çç¥ä¸å¡ä»£ç ...
    }
  }
}
```

å½éç¨ç¬¬äºç§åæ³ï¼å¹¶ä¸ `root = true` æ¶ï¼å°±ä¼å°è¯¥ `actions` æ¹æ³æ³¨åå°å¨å±ä¸ï¼å³åé¢ä¸å ä¸ä»»ä½çå½åç©ºé´åç¼

åæ¥çç `registerAction` æ¹æ³éå·ä½å®ç°äºä»ä¹

```js
// æ³¨åactionsæ¹æ³ï¼æ¥æ¶ä¸¤ä¸ªåæ°ï¼contextï¼åå«äºä¸ä¸æä¸­çdispatchæ¹æ³ãcommitæ¹æ³ãgettersæ¹æ³ãstateï¼ãä¼ å¥çåæ°payload
function registerAction (store, type, handler, local) {
  const entry = store._actions[type] || (store._actions[type] = [])   // éè¿store._actions è®°å½æææ³¨åçactions
  entry.push(function wrappedActionHandler (payload) {
    let res = handler.call(store, {
      dispatch: local.dispatch,
      commit: local.commit,
      getters: local.getters,
      state: local.state,
      rootGetters: store.getters,
      rootState: store.state
    }, payload)
    // è¥è¿åå¼ä¸æ¯ä¸ä¸ªpromiseå¯¹è±¡ï¼ååè£ä¸å±promiseï¼å¹¶å°è¿åå¼ä½ä¸ºthençåæ°
    if (!isPromise(res)) {
      res = Promise.resolve(res)
    }
    if (store._devtoolHook) {
      return res.catch(err => {
        store._devtoolHook.emit('vuex:error', err)
        throw err
      })
    } else {
      return res
    }
  })
}
```

ä¸ `mutations` ç±»ä¼¼ï¼åä» `store._actions` è·åå¥å£ `entry` ï¼ç¶åå°å½åç `actions` è¿è¡åè£å¤çåæ·»å å° `entry` çæ«å°¾ã `actions` æ¹æ³æ¥æ¶ä¸¤ä¸ªåæ°ï¼å³ `context` åæä»¬ä¼ å¥çåæ° `payload` ï¼å¶ä¸­ `context` æ¯ä¸ä¸ªå¯¹è±¡ï¼éé¢åå«äº `dispatch` ã`commit` ã`getters` ã`state` ã`rootGetters` ã`rootState` ï¼å4ä¸ªé½æ¯å¨å½åæ¨¡åçä¸ä¸æä¸­è°ç¨çï¼å2ä¸ªæ¯å¨å¨å±ä¸è°ç¨ç

æåå¯¹äº `actions` çè¿åå¼è¿åäºä¸å±å¤çï¼å ä¸º `actions` è§å®æ¯å¤çå¼æ­¥ä»»å¡çï¼æä»¥æä»¬è¯å®å¸æå¶å¼æ¯ä¸ä¸ª `promise` å¯¹è±¡ï¼è¿æ ·æ¹ä¾¿åç»­çæä½ãæä»¥è¿éå¯¹ `actions` æ¹æ³çè¿åå¼åäºä¸ä¸ªå¤æ­ï¼å¦ææ¬èº«å°±æ¯ `promise` å¯¹è±¡ï¼é£ä¹å°±ç´æ¥è¿å ï¼è¥ä¸æ¯ï¼ååè£ä¸å± `promise` å¯¹è±¡ï¼å¹¶å°è¿åå¼ `res` ä½ä¸ºåæ°è¿åç» `.then`

åæ ·çï¼`actions` æ¹æ³ä¹æ¯å¯ä»¥éåç

##### 3.2.5 æ³¨åæ¨¡åçgetters

```js
// æ³¨åæ¨¡åçæægetters
module.forEachGetter((getter, key) => {
  const namespacedType = namespace + key
  registerGetter(store, namespacedType, getter, local)
})
```

ä¸ä¸é¢çç±»ä¼¼ï¼è¿éå°±ä¸å¤è¯´äºï¼ç´æ¥è·³å° `registerGetters` æ¹æ³

```js
// æ³¨ågetters
function registerGetter (store, type, rawGetter, local) {
  if (store._wrappedGetters[type]) {   // è¥è®°å½è¿gettersäºï¼åä¸åéå¤è®°å½
    if (__DEV__) {
      console.error(`[vuex] duplicate getter key: ${type}`)
    }
    return
  }
  // å¨store._wrappedGettersä¸­è®°å½getters
  store._wrappedGetters[type] = function wrappedGetter (store) {
    return rawGetter(
      local.state, // local state
      local.getters, // local getters
      store.state, // root state
      store.getters // root getters
    )
  }
}
```

è¿éåç° `getters` å¹¶ä¸å `mutations` å `actions` ä¸æ ·å»è·åä¸ä¸ª `entry` ï¼èæ¯ç´æ¥æ¥ç `store._wrappedGetters[type]` æ¯å¦æå¯¹åºç `getters` ï¼è¥æï¼åä¸åéå¤è®°å½ ; å¦åå° `getters` åè£ä¸ä¸å­å¨ `sotre._wrappedGetters` ä¸­ï¼å¶ä¸­ç»è¿åè£åç `getters` æ¥æ¶4ä¸ªåæ°ï¼å³ `state` ã`getters` ã`rootState` ã`rootGetters` ï¼å2ä¸ªåå«è¡¨ç¤ºå½åä¸ä¸æä¸­ç `state` å `getters` ï¼å2ä¸ªåå«è¡¨ç¤ºæ ¹æ¨¡åç `state` å `getters`

æä»¥æä»¬å¨ä½¿ç¨ `Vuex` æ¶ï¼è°ç¨å­æ¨¡åç `getters` æ¶æ¯è¿æ ·çï¼

```js
const store = Vuex.Store({
  state: {
    a: 1,
    b: 2
  },
  getters: {
    addA(state) {
      return state.a + 1
    }
  },
  modules: {
    // å­æ¨¡åA
    ModuleA: {
      state: {
        c: 3
      },
      getters: {
      	sum(state, getters, rootState, rootGetters) {
          console.log(state.c)   // 3
          console.log(getters.addC)  // 4
          console.log(rootState.b)  // 2
          console.log(rootGetters.addA)  // 2
        },
        addC(state) {
          return state.c + 1
        }
      }
    }
  }
})
```

æåæä»¬åæ¬¡å¾åºä¸ä¸ªç»è®ºï¼`getters` æ¯ä¸è½éåçï¼å¹¶ä¸åä¸ä¸ªå½åçä¸ä¼è¢«åä¸ä¸ªå½åçæè¦ç

##### 3.2.6 éå½æ³¨åå­æ¨¡å

```js
// éå½æ³¨åå­æ¨¡å
module.forEachChild((child, key) => {
  installModule(store, rootState, path.concat(key), child, hot)
})
```

ç¶åå°±æ¯å¤æ­å½åçæ¨¡åéææ²¡æåµå¥çå­æ¨¡åäºï¼æçè¯å°±å°å­æ¨¡åçåç§°æ·»å å° `path` æ«å°¾ï¼ç¶åæç¸åºçåæ°ä¼ å¥ `installModule` æ¹æ³ï¼éæ°èµ°ä¸éæ¬æä¸­ `3.2` éææçæµç¨

#### 3.3 æ³¨åvm

ä¸é¢å·²ç»å°æ¨¡åçæ³¨åå®æ¯äºï¼çä¸ä¸ `constructor` ä¸­ä¸ä¸è¡ä»£ç æ¯ä»ä¹ï¼

```js
resetStoreVM(this, state)
```

è·³å°ç¸åºçæ¹æ³ä¸­å»çä¸ä¸ï¼

```js
// åå§åvm
function resetStoreVM (store, state, hot) {
  const oldVm = store._vm

  store.getters = {}    // å¨å®ä¾storeä¸è®¾ç½®getterså¯¹è±¡
  
  store._makeLocalGettersCache = Object.create(null)  // æ¸ç©ºæ¬å°ç¼å­
  const wrappedGetters = store._wrappedGetters
  const computed = {}
  // éågettersï¼å°æ¯ä¸ä¸ªgetteræ³¨åå°store.gettersï¼è®¿é®å¯¹åºgetteræ¶ä¼å»vmä¸è®¿é®å¯¹åºçcomputed
  forEachValue(wrappedGetters, (fn, key) => {
    computed[key] = partial(fn, store)
    Object.defineProperty(store.getters, key, {
      get: () => store._vm[key],
      enumerable: true // for local getters
    })
  })

  const silent = Vue.config.silent
  Vue.config.silent = true
  // ä½¿ç¨Vueå®ä¾æ¥å­å¨Vuexçstateç¶ææ ï¼å¹¶å©ç¨computedå»ç¼å­gettersè¿åçå¼
  store._vm = new Vue({
    data: {
      $$state: state
    },
    computed
  })
  Vue.config.silent = silent

  // å¯ç¨ä¸¥æ ¼æ¨¡å¼ççå¬è­¦å
  if (store.strict) {
    enableStrictMode(store)
  }

  // è¥å­å¨æ§çvm, éæ¯æ§çvm
  if (oldVm) {
    if (hot) {
      // è§£é¤å¯¹æ§çvmå¯¹stateçå¼ç¨
      store._withCommit(() => {
        oldVm._data.$$state = null
      })
    }
    Vue.nextTick(() => oldVm.$destroy())
  }
}
```

è¿ä¸ªæ¹æ³éä¸»è¦åçå°±æ¯çæä¸ä¸ª `Vue` çå®ä¾ `_vm` ï¼ç¶åå° `store._makeLocalGettersCache` éç `getters` ä»¥å `store.state` äº¤ç»ä¸ä¸ª `_vm` æç®¡ï¼å³å° `store.state` èµå¼ç» `_vm.data.$$state` ï¼å° `store._makeLocalGettersCache` éè¿è½¬ååèµå¼ç» `_vm.computed` ï¼è¿æ ·ä¸æ¥ï¼`state` å°±å®ç°äºååºå¼ï¼`getters` å®ç°äºç±»ä¼¼ `computed` çåè½

å ä¸ºçæäºæ°ç `_vm` ï¼æä»¥æåéè¿ `oldVm.$destory()` å°æ§ç `_vm` ç»éæ¯æäº

å¼å¾æ³¨æçæ¯ï¼å¶å° `sotre.getters` çæä½æ¾å¨äºè¿ä¸ªæ¹æ³éï¼æ¯å ä¸ºæä»¬åç»­è®¿é®æä¸ª `getters` æ¶ï¼è®¿é®çå¶å®æ¯ `_vm.computed` ä¸­çåå®¹ãå æ­¤ï¼éè¿ `Object.defineProperty` å¯¹ `store.getters` è¿è¡äºå¤ç

#### 3.4 è®¿é® state ãmutations ãactions

å°æ­¤ä¸ºæ­¢ï¼å·²ç»å®ç°äºå¯ä»¥éè¿ `store.getter.æä¸ªgetters` æ¥ä½¿ç¨ `getters` ï¼é£ä¹å¦ä½è®¿é® `state` ã`mutations` ã`actions` å¢ï¼

##### 3.4.1 è®¿é® state

éè¿æç´¢ï¼å¨ `Store` ç±»ä¸­å®ä¹äºä¸ä¸ª `get` å½æ°ï¼ç¨äºå¤ç `store.state` çæä½ï¼

```js
get state () {
  return this._vm._data.$$state
}
```

å¯ä»¥å¾æ¸æ¥å°çå°ï¼å½æä»¬è®¿é® `store.state` æ¶ï¼å°±æ¯å»è®¿é® `store._vm.data.$$state` ï¼ä¸åæä»ç» `_vm` æ¶è¯´çä¸æ ·

##### 3.4.2 è®¿é® mutations

å¶å® `mutations` çè®¿é®å¨ä¸å¼å§å°±è§¦åå°äºï¼åªä¸è¿å½æ¶åªæ¯æäºä¸å´ï¼å ä¸ºå½æ¶ç´æ¥æ¥çå¯è½ä¸ä¼å¤ªæç½

```js
const store = this
const { dispatch, commit } = this
this.dispatch = function boundDispatch (type, payload) {
  return dispatch.call(store, type, payload)
}
this.commit = function boundCommit (type, payload, options) {
  return commit.call(store, type, payload, options)
}
```

å¨ `Store` ä¸­ï¼å¯¹ `store.commit` å `store.dispatch` æ¹æ³åäºä¸å±å¤çï¼å°è¯¥æ¹æ³çè°ç¨æåäº `store` ï¼åæ¥çç `commit` æ¹æ³çå·ä½å®ç°

```js
commit (_type, _payload, _options) {
  // check object-style commit
  const {
    type,
    payload,
    options
  } = unifyObjectStyle(_type, _payload, _options)

  const mutation = { type, payload }
  const entry = this._mutations[type]    // æ¥æ¾_mutationsä¸æ¯å¦æå¯¹åºçæ¹æ³
  // æ¥æ¾ä¸å°åä¸æ§è¡ä»»ä½æä½
  if (!entry) {
    if (__DEV__) {
      console.error(`[vuex] unknown mutation type: ${type}`)
    }
    return
  }

  // è¥æç¸åºçæ¹æ³ï¼åæ§è¡
  this._withCommit(() => {
    entry.forEach(function commitIterator (handler) {
      handler(payload)
    })
  })

  this._subscribers
    .slice() // shallow copy to prevent iterator invalidation if subscriber synchronously calls unsubscribe
    .forEach(sub => sub(mutation, this.state))

  if (
    __DEV__ &&
    options && options.silent
  ) {
    console.warn(
      `[vuex] mutation type: ${type}. Silent option has been removed. ` +
      'Use the filter functionality in the vue-devtools'
    )
  }
}
```

é¦åéè¿ `unifyObjectStyle` æ¹æ³å¯¹ä¼ å¥çåæ°è¿è¡äºå¤çï¼æ¥çä¸ä¸è¿ä¸ªæ¹æ³æ¯å¹²ä»ä¹ç 

```js
function unifyObjectStyle (type, payload, options) {
  if (isObject(type) && type.type) {
    options = payload
    payload = type
    type = type.type
  }

  if (__DEV__) {
    assert(typeof type === 'string', `expects string as the type, but found ${typeof type}.`)
  }

  return { type, payload, options }
}
```

ä½¿ç¨è¿ `Vuex` çåºè¯¥é½ç¥éï¼`commit` æä¸¤ç§æäº¤æ¹å¼ï¼

```js
// ç¬¬ä¸ç§æäº¤æ¹å¼
this.$store.commit('func', 1)

// ç¬¬äºç§æäº¤æ¹å¼
this.$store.commit({
  type: 'func',
  num: 1
})
```

å¶åå¯¹ç¬¬ä¸ä¸ªåæ°è¿è¡å¤æ­æ¯å¦ä¸ºå¯¹è±¡ï¼æ¯çè¯å°±å½ä½å¯¹è±¡æäº¤é£æ ¼å¤çï¼å¦åçè¯å°±ç´æ¥è¿å

å¨å¤çå®åæ°ä»¥åï¼æ ¹æ® `type` ä» `store._mutations` ä¸è·åå° `entry` ï¼åé¢åæè¿äºï¼`mutations` æ¹æ³æ¯ä»¥æ°ç»å½¢å¼å­å¨çï¼æä»¥å¯è½æå¤ä¸ªæ¹æ³ãç¶åå¨ `_withCommit` æ¹æ³ä¸­éå `entry` ä¾æ¬¡æ§è¡ `mutations` æ¹æ³ï¼è¿æ¯å ä¸º `Vuex` è§å® `state` çæ¹åé½è¦éè¿ `mutations` æ¹æ³ï¼`store._committing` è¿ä¸ªå±æ§å°±æ¯ç¨æ¥å¤æ­å½åæ¯å¦å¤äºè°ç¨ `mutations` æ¹æ³çï¼å½ `state` å¼æ¹åæ¶ï¼ä¼åå»å¤æ­ `store._committing` æ¯å¦ä¸º `true` ï¼è¥ä¸ä¸º `true` ï¼åè¡¨ç¤º `state` çå¼æ¹åæ²¡æç»è¿ `mutations` æ¹æ³ï¼äºæ¯ä¼æå°è­¦åâ ï¸ ä¿¡æ¯

è `this._subscribers` è¿æ®µä»£ç æææ¶è¿ä¸æ¸æ¥æ¯å¹²ä»ä¹çï¼éè¿è¯ä¹ï¼ç®æµåºè¯¥æ¯ä¸ä¸ªå­æ¾è®¢éçä¸è¥¿å§ï¼å°±åæ¾çä¸ç®¡äºï¼ç­åç»­åæ¥åç

##### 3.4.3 è®¿é® actions

```js
dispatch (_type, _payload) {
  // check object-style dispatch
  const {
    type,
    payload
  } = unifyObjectStyle(_type, _payload)

  const action = { type, payload }
  const entry = this._actions[type]  // æ¥æ¾_actionsä¸æ¯å¦æå¯¹åºçæ¹æ³
  // æ¥æ¾ä¸å°åä¸æ§è¡ä»»ä½æä½
  if (!entry) {
    if (__DEV__) {
      console.error(`[vuex] unknown action type: ${type}`)
    }
    return
  }

  try {
    this._actionSubscribers
      .slice() // shallow copy to prevent iterator invalidation if subscriber synchronously calls unsubscribe
      .filter(sub => sub.before)
      .forEach(sub => sub.before(action, this.state))
  } catch (e) {
    if (__DEV__) {
      console.warn(`[vuex] error in before action subscribers: `)
      console.error(e)
    }
  }

  const result = entry.length > 1
  ? Promise.all(entry.map(handler => handler(payload)))
  : entry[0](payload)

  return new Promise((resolve, reject) => {
    result.then(res => {
      try {
        this._actionSubscribers
          .filter(sub => sub.after)
          .forEach(sub => sub.after(action, this.state))
      } catch (e) {
        if (__DEV__) {
          console.warn(`[vuex] error in after action subscribers: `)
          console.error(e)
        }
      }
      resolve(res)
    }, error => {
      try {
        this._actionSubscribers
          .filter(sub => sub.error)
          .forEach(sub => sub.error(action, this.state, error))
      } catch (e) {
        if (__DEV__) {
          console.warn(`[vuex] error in error action subscribers: `)
          console.error(e)
        }
      }
      reject(error)
    })
  })
}
```

ååé¨åä¸ `commit` æ¹æ³ç±»ä¼¼ï¼å°±ä¸å¤è¯´äº

ä»£ç ä¸­ååºç°äº `this._actionSubscribers` ï¼ä¸ `commit` ä¸­çä¹ç±»ä¼¼ï¼å¯è½è¿éæ¯å­æ¾ `actions` çè®¢éèçä¸è¥¿ï¼æä»¥è¿äºé½åä¸çäº

å¶ä¸­åé `result` ï¼åå¤æ­ `entry` çé¿åº¦ï¼è¥å¤§äº1ï¼åè¡¨ç¤ºæå¤ä¸ªå¼æ­¥æ¹æ³ï¼æä»¥ç¨ `Promise.all` è¿è¡åè£¹ ; å¦åç´æ¥æ§è¡ `entry[0]` 

æååå»ºå¹¶è¿åäºä¸ä¸ªæ°ç `promise` ï¼åé¨å¤æ­äº `result` çç¶æï¼æååæ§è¡ `resolve` ï¼å¤±è´¥åæ§è¡ `reject`

å°æ­¤ä¸ºæ­¢ï¼æä»¬å·²ç»å®ç°äº `store.state` ã`store.getters` ã`store.commit` ã`store.dispatch` çè°ç¨äº

#### 3.5 æä»¶çè°ç¨

ç»§ç»­ç `constructor` ä¸­çä»£ç ï¼è¿æ®µä»£ç ä¹æ¯æ´ä¸ª `Store` ç±»çæé å½æ°ä¸­æåçä¸å°æ®µä»£ç äºï¼

```js
// ä¾æ¬¡è°ç¨ä¼ å¥çæä»¶
plugins.forEach(plugin => plugin(this))

const useDevtools = options.devtools !== undefined ? options.devtools : Vue.config.devtools
// ä½¿ç¨vueçå¼åæä»¶
if (useDevtools) {
  devtoolPlugin(this)
}
```

é¦åå°±æ¯éååå»º `Store` ç±»æ¶ä¼ å¥çåæ° `Plugins` ï¼ä¾æ¬¡è°ç¨ä¼ å¥çæä»¶å½æ°ï¼å½ç¶ä¸è¬æä»¬é½æ²¡æä¼ å¥ï¼æä»¥ `Plugins` é»è®¤æ¯ç©ºæ°ç»ï¼

ç¶åå°±æ¯è°ç¨ `devtoolPlugin` æ¹æ³å¦ï¼æ ¹æ®å¯¼å¥çè·¯å¾æä»¬å»å°ç¸åºçæä»¶

```js
// æä»¶è·¯å¾ï¼./plugins/devtool.js
const target = typeof window !== 'undefined'
  ? window
  : typeof global !== 'undefined'
    ? global
    : {}
const devtoolHook = target.__VUE_DEVTOOLS_GLOBAL_HOOK__

export default function devtoolPlugin (store) {
  if (!devtoolHook) return

  store._devtoolHook = devtoolHook

  devtoolHook.emit('vuex:init', store)

  devtoolHook.on('vuex:travel-to-state', targetState => {
    store.replaceState(targetState)
  })

  store.subscribe((mutation, state) => {
    devtoolHook.emit('vuex:mutation', mutation, state)
  }, { prepend: true })

  store.subscribeAction((action, state) => {
    devtoolHook.emit('vuex:action', action, state)
  }, { prepend: true })
}
```

çäºåå¤©ï¼æç´¢äºåå¤©ï¼é½æ²¡ææ¾å°åªä¸ªæä»¶éæ `__VUE_DEVTOOLS_GLOBAL_HOOK__` ï¼åºè¯¥æ¯ `dev-tools` æä»¶éå®ä¹çï¼ä¸ºäºä¿è¯ `Vuex` çæºç éè¯»è¿åº¦ï¼å°±åèå¼éè¯» `dev-tools` æä»¶çåå®¹äº

#### 3.6 å¶å®æ¹æ³

æ´ä¸ª `Store` å®ä¾çæçå¨è¿ç¨å·®ä¸å¤å°±æ¯è¿æ ·äºï¼å¦å¤è¿ä¼åç°ï¼å¶å®æå¾å¤æ¹æ³é½æ²¡æè¢«ç¨å°ï¼ä½æ¯å´è¢«å®ä¹åºæ¥äºï¼è¿éå¯ä»¥ç¨å¾®åä¸¾å ä¸ªç®åå°çä¸ä¸

##### 3.6.1 æ´æ° state

```js
// å¨store._committing = true çç¶æä¸æ´æ°ä¸ä¸state
replaceState (state) {
  this._withCommit(() => {
    this._vm._data.$$state = state
  })
}
```

ä¸ç®äºç¶ï¼è¿æ¯æä¾äºä¸ç§ç´æ¥ä¿®æ¹ `state` çæ¹æ³ï¼å¹¶ä¸ä¸ä¼æå°è­¦åä¿¡æ¯

##### 3.6.2 æ³¨åãå¸è½½æ¨¡å

```js
// æ³¨åæ¨¡å
registerModule (path, rawModule, options = {}) {
  if (typeof path === 'string') path = [path]

  if (__DEV__) {
    assert(Array.isArray(path), `module path must be a string or an Array.`)
    assert(path.length > 0, 'cannot register the root module by using registerModule.')
  }

  this._modules.register(path, rawModule)
  installModule(this, this.state, path, this._modules.get(path), options.preserveState)
  // reset store to update getters...
  resetStoreVM(this, this.state)
}

// å¸è½½æ¨¡å
unregisterModule (path) {
  if (typeof path === 'string') path = [path]

  if (__DEV__) {
    assert(Array.isArray(path), `module path must be a string or an Array.`)
  }

  this._modules.unregister(path)
  this._withCommit(() => {
    const parentState = getNestedState(this.state, path.slice(0, -1))
    Vue.delete(parentState, path[path.length - 1])
  })
  resetStore(this)
}
```

##### 3.6.3 éç½® store å®ä¾

```js
// éç½®storeï¼å³æ³¨åæ¨¡åãçævmç­æä½
function resetStore (store, hot) {
  store._actions = Object.create(null)
  store._mutations = Object.create(null)
  store._wrappedGetters = Object.create(null)
  store._modulesNamespaceMap = Object.create(null)
  const state = store.state
  // init all modules
  installModule(store, state, [], store._modules.root, true)
  // reset vm
  resetStoreVM(store, state, hot)
}
```

å°ææçç¶æé½æ¸ç©ºï¼ç¶åéæ°æ§è¡ä¸è¾¹ `installModule` å `resetStoreVM` ï¼è¿ä¸è¬å¨æ¨¡åç»æååä»¥åè°ç¨ï¼ä¾å¦æä¸ªæ¨¡åè¢«å¸è½½

### 4. install æ³¨å

`Store` ç±»çææå®ç°é½äºè§£å®äºï¼åæ¥çä¸ä¸å¥å£æä»¶éè¿æä»ä¹ï¼çªç¶åç°å¿è®°çä¸ä¸éå¸¸éè¦ç `install` æ¹æ³äºï¼æ ¹æ® `install` æ¹æ³çå¯¼å¥è·¯å¾æ¾å°ç¸åºçå½æ°ï¼

```js
// æä¾installæ¹æ³
export function install (_Vue) {
  if (Vue && _Vue === Vue) {
    if (__DEV__) {
      console.error(
        '[vuex] already installed. Vue.use(Vuex) should be called only once.'
      )
    }
    return
  }
  Vue = _Vue
  applyMixin(Vue)
}
```

å½æä»¬è°ç¨ `Vue.use(vuex)` æ¶ï¼è°ç¨è¿ä¸ªæ¹æ³ï¼åå¤æ­ `vuex` æ¯å¦å·²è¢«æ³¨åï¼è¥å·²è¢«æ³¨åï¼åä¸æ§è¡ä»»ä½æä½ ; è¥æ²¡æè¢«æ³¨åï¼åè°ç¨ `applyMixin` æ¹æ³ï¼ç°å¨ç§»æ­¥å° `./mixin.js` æä»¶ï¼

```js
export default function (Vue) {
  const version = Number(Vue.version.split('.')[0])

  // 2.xçæ¬ç´æ¥éè¿å¨å±æ··å¥Vue.mixinçæ¹å¼æè½½store
  if (version >= 2) {
    Vue.mixin({ beforeCreate: vuexInit })
  } else {
    // å¼å®¹1.xçæ¬
    const _init = Vue.prototype._init
    Vue.prototype._init = function (options = {}) {
      options.init = options.init
        ? [vuexInit].concat(options.init)
        : vuexInit
      _init.call(this, options)
    }
  }

  // å°vuexæ··å¥å°$optionsä¸­
  function vuexInit () {
    // è·åå½åç»ä»¶ç $options
    const options = this.$options
    // è¥å½åç»ä»¶ç$optionsä¸å·²å­å¨storeï¼åå°$options.storeèµå¼ç»this.$storeï¼ä¸è¬æ¯ç¨äºæ ¹ç»ä»¶çï¼
    if (options.store) {
      this.$store = typeof options.store === 'function'
        ? options.store()
        : options.store
    } 
    // å½åç»ä»¶ç$optionsä¸æ²¡æstoreï¼åè·åç¶ç»ä»¶ä¸ç$storeï¼å³$options.parent.$storeï¼å¹¶å°å¶èµå¼ç»this.$storeï¼ä¸è¬ç¨äºå­ç»ä»¶ï¼
    else if (options.parent && options.parent.$store) {
      this.$store = options.parent.$store
    }
  }
}
```

`applyMixin` æ¹æ³åå¤æ­äº `Vue` ççæ¬å·ï¼ä¸»è¦åçæ¯ä¸ä¸ªåä¸å¼å®¹ `Vue 1.x` ççæ¬ï¼è¿éæå¯¹ `Vue 1.x` ççæ¬ä¸å¤ªçæï¼æä»¥å°±ç´æ¥ç `Vue 2.x` çæ¬çå¤çæ¹å¼å§

éè¿ `Vue.minxin` æ¹æ³åäºä¸ä¸ªå¨å±çæ··å¥ï¼å¨æ¯ä¸ªç»ä»¶ `beforeCreate` çå½å¨ææ¶ä¼è°ç¨ `vuexInit` æ¹æ³ï¼è¯¥æ¹æ³å¤çå¾éå¸¸å·§å¦ï¼é¦åè·åå½åç»ä»¶ç `$options` ï¼å¤æ­å½åç»ä»¶ç `$options` ä¸æ¯å¦æ `sotre` ï¼è¥æåå° `store` èµå¼ç»å½åç»ä»¶ï¼å³ `this.$store` ï¼è¿ä¸ªä¸è¬æ¯å¤æ­æ ¹ç»ä»¶çï¼å ä¸ºåªæå¨åå§å `Vue` å®ä¾çæ¶åæä»¬ææå¨ä¼ å¥äº `store` ; è¥ `$options` ä¸æ²¡æ `store` ï¼åä»£è¡¨å½åä¸æ¯æ ¹ç»ä»¶ï¼æä»¥æä»¬å°±å»ç¶ç»ä»¶ä¸è·åï¼å¹¶èµå¼ç»å½åç»ä»¶ï¼å³å½åç»ä»¶ä¹å¯ä»¥éè¿ `this.$store` è®¿é®å° `store` å®ä¾äº

è¿éä¸å¾ä¸æå¹ï¼è¿ä¸ªå¤çæ¹å¼å¤ªæ£äºã

### 5. è¾å©å½æ°

`store`å®ä¾çæå¹¶ä¸ä¹ `install` å° `Vue` ä¸äºï¼çä¸ä¸å¥å£æä»¶ä¸­åªå©ä¸è¾å©å½æ°äºï¼å®ä»¬æ `mapState` ã`mapGetters` ã`mapMutations` ã`mapActions` ã`createNamespacedHelpers` ï¼è¿å°ç¸åºçæä»¶ `./helpers.js` ä¸­çä¸ä¸

```js
import { isObject } from './util.js'

export const mapState = normalizeNamespace((namespace, states) => {
  const res = {}
  if (__DEV__ && !isValidMap(states)) {
    console.error('[vuex] mapState: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(states).forEach(({ key, val }) => {
    res[key] = function mappedState () {
      let state = this.$store.state
      let getters = this.$store.getters
      if (namespace) {
        const module = getModuleByNamespace(this.$store, 'mapState', namespace)
        if (!module) {
          return
        }
        state = module.context.state
        getters = module.context.getters
      }
      return typeof val === 'function'
        ? val.call(this, state, getters)
        : state[val]
    }
    // mark vuex getter for devtools
    res[key].vuex = true
  })
  return res
})


export const mapMutations = normalizeNamespace((namespace, mutations) => {
  const res = {}
  if (__DEV__ && !isValidMap(mutations)) {
    console.error('[vuex] mapMutations: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(mutations).forEach(({ key, val }) => {
    res[key] = function mappedMutation (...args) {
      // Get the commit method from store
      let commit = this.$store.commit
      if (namespace) {
        const module = getModuleByNamespace(this.$store, 'mapMutations', namespace)
        if (!module) {
          return
        }
        commit = module.context.commit
      }
      return typeof val === 'function'
        ? val.apply(this, [commit].concat(args))
        : commit.apply(this.$store, [val].concat(args))
    }
  })
  return res
})


export const mapGetters = normalizeNamespace((namespace, getters) => {
  const res = {}
  if (__DEV__ && !isValidMap(getters)) {
    console.error('[vuex] mapGetters: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(getters).forEach(({ key, val }) => {
    // The namespace has been mutated by normalizeNamespace
    val = namespace + val
    res[key] = function mappedGetter () {
      if (namespace && !getModuleByNamespace(this.$store, 'mapGetters', namespace)) {
        return
      }
      if (__DEV__ && !(val in this.$store.getters)) {
        console.error(`[vuex] unknown getter: ${val}`)
        return
      }
      return this.$store.getters[val]
    }
    // mark vuex getter for devtools
    res[key].vuex = true
  })
  return res
})


export const mapActions = normalizeNamespace((namespace, actions) => {
  const res = {}
  if (__DEV__ && !isValidMap(actions)) {
    console.error('[vuex] mapActions: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(actions).forEach(({ key, val }) => {
    res[key] = function mappedAction (...args) {
      // get dispatch function from store
      let dispatch = this.$store.dispatch
      if (namespace) {
        const module = getModuleByNamespace(this.$store, 'mapActions', namespace)
        if (!module) {
          return
        }
        dispatch = module.context.dispatch
      }
      return typeof val === 'function'
        ? val.apply(this, [dispatch].concat(args))
        : dispatch.apply(this.$store, [val].concat(args))
    }
  })
  return res
})

/**
 * Rebinding namespace param for mapXXX function in special scoped, and return them by simple object
 * @param {String} namespace
 * @return {Object}
 */
export const createNamespacedHelpers = (namespace) => ({
  mapState: mapState.bind(null, namespace),
  mapGetters: mapGetters.bind(null, namespace),
  mapMutations: mapMutations.bind(null, namespace),
  mapActions: mapActions.bind(null, namespace)
})


function normalizeMap (map) {
  if (!isValidMap(map)) {
    return []
  }
  return Array.isArray(map)
    ? map.map(key => ({ key, val: key }))
    : Object.keys(map).map(key => ({ key, val: map[key] }))
}

function isValidMap (map) {
  return Array.isArray(map) || isObject(map)
}

function normalizeNamespace (fn) {
  return (namespace, map) => {
    if (typeof namespace !== 'string') {
      map = namespace
      namespace = ''
    } 
    else if (namespace.charAt(namespace.length - 1) !== '/') {
      namespace += '/'
    }
    return fn(namespace, map)
  }
}

function getModuleByNamespace (store, helper, namespace) {
  const module = store._modulesNamespaceMap[namespace]
  if (__DEV__ && !module) {
    console.error(`[vuex] module namespace not found in ${helper}(): ${namespace}`)
  }
  return module
}
```

æ´ä¸ªæä»¶éä¸è¥¿éå¸¸å¤ï¼ä½æä»¬å¾æç¡®å°ç¥éï¼æä»¬ä¸»è¦ççå°±æ¯é£å ä¸ªè¾å©å½æ°ï¼è§å¯åç°ï¼æ¯ä¸ªè¾å©å½æ°é½ä¼åè°ç¨ `normalizeNamespace` å½æ°è¿è¡å¤çï¼é£ä¹æä»¬å°±åççè¿ä¸ªå½æ°åäºä»ä¹ï¼

```js
function normalizeNamespace (fn) {
  return (namespace, map) => {
    if (typeof namespace !== 'string') {
      map = namespace
      namespace = ''
    } 
    else if (namespace.charAt(namespace.length - 1) !== '/') {
      namespace += '/'
    }
    return fn(namespace, map)
  }
}
```

æ ¹æ®å½æ°åçå­é¢ææç¥éè¿åºè¯¥æ¯æ ¹æ®ä¸åçè°ç¨æ¹æ³ï¼æ ååå½åç©ºé´çã

é¦åè¿åä¸ä¸ªå½æ°ï¼æ¥æ¶ä¸¤ä¸ªåæ°ï¼å³ `namespace` å `map` ï¼è¿ä¹æ¯æä»¬è°ç¨è¾å©å½æ°æ¶å¯ä»¥ä¼ å¥çä¸¤ä¸ªåæ° ;

ç¶åå¤æ­ `namespace` æ¯å¦ä¸ºå­ç¬¦ä¸²å½¢å¼ï¼è¥ä¸æ¯å­ç¬¦ä¸²ï¼åè¡¨ç¤ºæ¯æ®éçè°ç¨æ¹å¼ï¼ä¾å¦ï¼

```
mapMutations(['first/second/foo', 'first/second/bar'])

mapMutations({
   foo: 'first/second/foo',
   bar: 'first/second/bar',
})
```

è¿ç§æåµï¼å°±ç´æ¥å°ç¬¬ä¸ä¸ªåæ° `namespace` èµå¼ç»æ å°åé `map` ï¼è `namespace` è®¾ä¸ºç©º

è¥æ¯å­ç¬¦ä¸²çè¯ï¼åè¡¨ç¤ºè°ç¨çæ¯å¸¦å½åç©ºé´çç»å®å½æ°çï¼ä¾å¦ï¼

```js
mapState('first/second', ['foo', 'bar'])

mapState('first/second', {
  foo: 'foo',
  bar: 'bar',
})
```

å¤çå¥½è¿ä¸¤ç§ä¸åçè°ç¨æ¹å¼ä»¥åï¼è°ç¨ä¸ä¸ `fn` ï¼å¹¶å° `namespace` å `map` ä½ä¸ºåæ°

é£ä¹å°±åä» `mapState` å¼å§çå§

##### 5.1 mapState

```js
export const mapState = normalizeNamespace((namespace, states) => {
  const res = {}
  if (__DEV__ && !isValidMap(states)) {
    console.error('[vuex] mapState: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(states).forEach(({ key, val }) => {
    res[key] = function mappedState () {
      let state = this.$store.state
      let getters = this.$store.getters
      if (namespace) {
        const module = getModuleByNamespace(this.$store, 'mapState', namespace)
        if (!module) {
          return
        }
        state = module.context.state
        getters = module.context.getters
      }
      return typeof val === 'function'
        ? val.call(this, state, getters)
        : state[val]
    }
    // mark vuex getter for devtools
    res[key].vuex = true
  })
  return res
})
```

è¿éç `namespace` æ¯ä¸ä¸ªå­ç¬¦ä¸²ï¼`states` æ¯æä»¬åæå¤çå¥½çæ å°åé `map`

é¦ååå»ºä¸ä¸ªç©ºå¯¹è±¡ `res` ï¼è¿æ¯æä»¬æåå¤çå¥½è¦è¿åçåé ;

ç¶åéè¿ `isValidMap` æ¹æ³å¤æ­ `map` æ¯å¦ç¬¦åè¦æ±ï¼å³æ¯å¦æ¯æ°ç»æå¯¹è±¡ ;

åç¶åè°ç¨äº `normalizeMap` æ¹æ³å¤çäºåé `states` ï¼ä»å­é¢æä¹ä¸æ¥çï¼è¿æ¯ç¨æ¥æ ååè¯¥åéçï¼å ä¸ºæ¯ç«æå¯è½æ¯æ°ç»åæå¯è½æ¯å¯¹è±¡åï¼æä»¥è¦ç»ä¸ä¸ä¸ãæ¥çä¸ä¸ `normalizeMap` æ¹æ³çå®ç°ï¼

```js
function normalizeMap (map) {
  if (!isValidMap(map)) {
    return []
  }
  return Array.isArray(map)
    ? map.map(key => ({ key, val: key }))
    : Object.keys(map).map(key => ({ key, val: map[key] }))
}
```

é¦åä»ç¶è¦åå¤æ­ `map` æ¯å¦åæ³ï¼è¥ä¸åæ³ï¼åè¿åç©ºæ°ç»ï¼é¿ååç»­çä»£ç æ¥é ;

ç¶åå¤æ­ `map` æ¯å¦ä¸ºæ°ç»ï¼è¥æ¯æ°ç»ï¼åéå `map` è¿è¡å¤çï¼

```js
å° [1, 2, 3] åæ [{key: 1, val: 1}, {key: 2, val: 2}, {key: 3, val: 3}]
```

è¥ `map` ä¸æ¯æ°ç»ï¼åä¸å®ä¸ºå¯¹è±¡ï¼é£ä¹åæ ·ä¹è¦æå¶å¤çæè·ä¸é¢ä¸æ ·çæ ¼å¼ï¼

```js
å° {a: 1, b: 2, c: 3} åæ [{key: a, val: 1}, {key: b, val: 2}, {key: c, val: 3}]
```

å¤çå¥½äºä»¥åå°±ç´æ¥è¿åï¼å¨å¾å°æ ååä»¥åç `map` åè¦å¯¹å¶è¿è¡ `forEach` éåï¼å°éåå°çæ¯ä¸ä¸ªå¯¹è±¡ç»è¿å¤çåå­æ¾å¨ `res` ä¸­ï¼å³ `res[key] = function mappedState() {...}` ï¼æ¥çä¸ä¸è¿ä¸ª `mappedState` éåäºä»ä¹å¤ç

é¦åè·åä¸ä¸æ ¹æ¨¡åä¸ç `state` å `getters`

```js
// è·åæ ¹æ¨¡åç state ãgetters
let state = this.$store.state
let getters = this.$store.getters
```

ç¶åå¤æ­æ¯å¦å­å¨å½åç©ºé´ï¼å³ `namespace` æ¯å¦ä¸ºç©ºï¼è¥ä¸ºç©ºï¼åä¸åä»»ä½å¤ç ; å¦åè°ç¨ `getModuleByNamespace` æ¹æ³è·åå° `namespace` å¯¹åºçæ¨¡å `module` 

```js
function getModuleByNamespace (store, helper, namespace) {
  const module = store._modulesNamespaceMap[namespace]
  if (__DEV__ && !module) {
    console.error(`[vuex] module namespace not found in ${helper}(): ${namespace}`)
  }
  return module
}
```

å¯ä»¥çå° `store._modulesNamespaceMap` ç»äºæ´¾ä¸äºç¨åºï¼å¨çæ `Store` å®ä¾æ³¨åæææ¨¡åçæ¶åï¼å°å¸¦æå½åç©ºé´çæ¨¡åé½å­å¨å¨äºè¯¥åéä¸ï¼åæ¥æ¯å¨è¿éç¨ä¸äº

ç¶åå°åæå£°æçåé `state` å `getters` æ¿æ¢æ `module` å¯¹åºä¸ä¸æä¸­ç `state` å `getters` 

```js
if (namespace) {
  // è·åå½åç©ºé´namespaceå¯¹åºçæ¨¡å
  const module = getModuleByNamespace(this.$store, 'mapState', namespace)
  if (!module) {
    return
  }
  // å° state ãgetters åæè¯¥æ¨¡åä¸ä¸æä¸­ç state ãgetters
  state = module.context.state
  getters = module.context.getters
}
```

è¿ä¸ª `context` ä¹æ¯éå¸¸çå·§å¦ï¼å¨æ³¨åæ¨¡åçæ¶åï¼è·åå°è¯¥æ¨¡åçä¸ä¸æçåæ¶ï¼è¿å°å¶å­å¨äºä¸ä¸ï¼å³ï¼

```js
const local = module.context = makeLocalContext(store, namespace, path)
```

ä¹åçå°çæ¶åä¸ç¥éæå¥ç¨ï¼ä½å¨è¿éçå°åï¼è§å¾ççéå¸¸å¾èµ ð

ç¡®å®å¥½äº `state` å `getters` çå¼ï¼æåå°±å¯ä»¥è¿åå¼äº

```js
return typeof val === 'function'
  ? val.call(this, state, getters)
	: state[val]
```

è¿éè¿åäºä¸å±å¤çæ¯å ä¸ºè¦å¤çä¸¤ç§ä¸åçæ¹å¼ï¼ä¾å¦ï¼

```js
mapState({
  foo: state => state.foo,
  bar: 'bar'
})
```

å¨è¿éæååç°äºä¸ä¸ªå®æ¹ææ¡£éæ²¡ææåçï¼å°±æ¯ä»¥å½æ°å½¢å¼è¿åçæ¶åï¼è¿è½æ¥æ¶ç¬¬äºä¸ªåæ° `getters` ï¼å³ï¼`foo: (state, getters) => state.foo + getters.bar`

##### 5.2 mapMutations

```js
export const mapMutations = normalizeNamespace((namespace, mutations) => {
  const res = {}
  if (__DEV__ && !isValidMap(mutations)) {
    console.error('[vuex] mapMutations: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(mutations).forEach(({ key, val }) => {
    res[key] = function mappedMutation (...args) {
      // Get the commit method from store
      let commit = this.$store.commit
      if (namespace) {
        const module = getModuleByNamespace(this.$store, 'mapMutations', namespace)
        if (!module) {
          return
        }
        commit = module.context.commit
      }
      return typeof val === 'function'
        ? val.apply(this, [commit].concat(args))
        : commit.apply(this.$store, [val].concat(args))
    }
  })
  return res
})
```

`mapMutations` ä¸ `mapState` çå®ç°å¤§ä½ç¸ä¼¼ï¼ä¸»è¦çä¸åå°±å¨ä¸é¢è¿æ®µä»£ç ï¼

```js
return typeof val === 'function'
  ? val.apply(this, [commit].concat(args))
	: commit.apply(this.$store, [val].concat(args))
```

è¿éä¹æ¯å `mapState` ä¸æ ·å¤çäºå½æ°çè°ç¨ç±»ååæ®éçè°ç¨ç±»åï¼ä¾å¦ï¼

```js
mapMutations({
  foo: (commit, num) => {
    commit('foo', num)
  },
  bar: 'bar'
})
```

å½æ¯å½æ°çè°ç¨ç±»åæ¶ï¼åå° `commit` ä½ä¸ºç¬¬ä¸ä¸ªåæ°ï¼å¹¶æé¢å¤çåæ°ä¸å¹¶ä¼ å¥ï¼æä»¥ææç `val.apply(this, [commit].concat(args))` è¿æ®µä»£ç  ;

å½æ¯æ®éçè°ç¨ç±»åæ¶ï¼åç´æ¥æ§è¡ `commit` ï¼å¶ä¸­ `val` å¯¹åºçå°±æ¯è¯¥å½åç©ºé´ä¸éè¦è°ç¨ç `mutations` æ¹æ³åï¼ç¶ååæ¥æ¶é¢å¤çåæ°ï¼å³ `commit.apply(this.$store, [val].concat(args))`

##### 5.3 mapGetters

```js
export const mapGetters = normalizeNamespace((namespace, getters) => {
  const res = {}
  if (__DEV__ && !isValidMap(getters)) {
    console.error('[vuex] mapGetters: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(getters).forEach(({ key, val }) => {
    // The namespace has been mutated by normalizeNamespace
    val = namespace + val
    res[key] = function mappedGetter () {
      if (namespace && !getModuleByNamespace(this.$store, 'mapGetters', namespace)) {
        return
      }
      if (__DEV__ && !(val in this.$store.getters)) {
        console.error(`[vuex] unknown getter: ${val}`)
        return
      }
      return this.$store.getters[val]
    }
    // mark vuex getter for devtools
    res[key].vuex = true
  })
  return res
})
```

è¿ä¸ªä¹æ²¡ä»ä¹å¥½è¯´çäºï¼æ¿å°å½åç©ºé´ `namespace` ï¼ç´æ¥æ¼æ¥ä¸ `val` éè¿ `this.$store.getters[val]` è¿è¡è®¿é®ãç®åä¸¾ä¸ªä¾å­ï¼

ç¬¬ä¸ç§æåµ

```js
// ç¬¬ä¸ç§
mapGetters(['first/foo'])
```

è¿ç§æåµä¸ `namespace` è¢«å¤çæäºç©ºå­ç¬¦ä¸²ï¼`map` è¢«å¤çæäº `['first/foo']` ï¼éå `map` ï¼æ­¤æ¶ `val = 'first/foo'` ï¼é£ä¹ `val = namespace + val` å¤çå `val` ä»ç¶ç­äº `first/foo` ï¼æä»¥æåå°±ç¸å½äºè°ç¨ `this.$store.getters['first/foo']`

åæ¥çç¬¬äºç§æåµ

```js
// ç¬¬äºç§
mapGetters('first', ['foo'])
```

 è¿ç§æåµä¸ `namespace` è¢«å¤çæäº `first/`ï¼`map` è¢«å¤çæäº `['foo']` ï¼éå `map` ï¼æ­¤æ¶ `val = 'foo'` ï¼é£ä¹ `val = namespace + val` å¤çå `val` å°±ç­äº `first/foo` ï¼æä»¥æåä»ç¶æ¯ç¸å½äºè°ç¨ `this.$store.getters['first/foo']`

##### 5.4 mapActions

```js
export const mapActions = normalizeNamespace((namespace, actions) => {
  const res = {}
  if (__DEV__ && !isValidMap(actions)) {
    console.error('[vuex] mapActions: mapper parameter must be either an Array or an Object')
  }
  normalizeMap(actions).forEach(({ key, val }) => {
    res[key] = function mappedAction (...args) {
      // get dispatch function from store
      let dispatch = this.$store.dispatch
      if (namespace) {
        const module = getModuleByNamespace(this.$store, 'mapActions', namespace)
        if (!module) {
          return
        }
        dispatch = module.context.dispatch
      }
      return typeof val === 'function'
        ? val.apply(this, [dispatch].concat(args))
        : dispatch.apply(this.$store, [val].concat(args))
    }
  })
  return res
})
```

ç®åçäºä¸ä¸ï¼å¤çæµç¨è· `mapMutations` å ä¹ä¸æ¨¡ä¸æ ·ï¼å°±ä¸å¤è¯´äº

##### 5.5 createNamespacedHelpers

```js
export const createNamespacedHelpers = (namespace) => ({
  mapState: mapState.bind(null, namespace),
  mapGetters: mapGetters.bind(null, namespace),
  mapMutations: mapMutations.bind(null, namespace),
  mapActions: mapActions.bind(null, namespace)
})
```

è¯¥æ¹æ³æ¯æ ¹æ®ä¼ å¥çå½åç©ºé´ `namespace` åå»ºä¸ç»è¾å©å½æ°ãå·§å¦ä¹å¤å°±æ¯åéè¿ `bind` å½æ°æç¬¬ä¸ä¸ªåæ°åä¼ å¥

```js
import { createNamespacedHelpers } from 'vuex'

const { mapState, mapActions } = createNamespacedHelpers('first/second')

export default {
  computed: {
    ...mapState({
      a: 'a',  // ç¸å½äº first/second/a
      b: 'b',  // ç¸å½äº first/second/b
    })
  },
  methods: {
    ...mapActions([
      'foo',      // ç¸å½äº first/second/foo
      'bar',      // ç¸å½äº first/second/bar
    ])
  }
}
```

# ð¡ å¿å¾ä½ä¼

é¦åï¼æä¸ç´æä¸ä¸ªéè¯»æºç çæ³æ³ï¼ä½å´å ä¸ºè½åæéè¿è¿æ²¡æè¡å¨ï¼ä¹åå¨ä¸æ¬¡ä¸å¤§ä½¬çäº¤æµä¸­ï¼æåç°äºèªå·±çä¸è¶³ï¼æ²¡ææ·±å¥å­¦ä¹ ï¼å³åªåçå¨**ä¼ç¨**çé¶æ®µï¼å´æ²¡æåå°ç¥å¶ç¶ç¥å¶æä»¥ç¶ãè¯´å®è¯ï¼è¿æ ·ççå¾é¾åï¼æ¯æ¬¡ç¨æä¸ªåºæ¶ï¼åºç°äºæä¸ªé®é¢åªä¼åçèèæ¯å¦èªå·±è°ç¨çæ¹å¼æé®é¢ï¼ç¶åä¸æç´¢å¼ææ¾ç­æ¡ï¼é¿æè¿æ ·èªå·±ä¹å¾é¾æè¿æ­¥ã

æä»¥ï¼å ä¸ºä»¥ä¸ä¸ç¹åå ï¼æåå¤é èªå·±å¥½å¥½çä¸ä¸ `Vuex` æºç ï¼

1. `Vuex` çæ ¸å¿æºç æ¯è¾å°ï¼å¯¹äºåæä¸æ ·ç¬¬ä¸æ¬¡éè¯»æºç çäººæ¯è¾åå¥½
2. æ·±å¥å­¦ä¹ äºå¸¸ç¨çåºä»¥åï¼å¨ä½¿ç¨çæ¶åéå°é®é¢ï¼å¯ä»¥å¿«éå°æ¾å°é®é¢æ ¹æº
3. ä¸è½åªåçå¨æççåºçè¡¨é¢ï¼è¦å­¦ä¹ å®ä»¬çææ³ãææ¯ï¼è¿æ ·æå©äºèªå·±çæé¿

åå¼å§ä¸ç¥éèªå·±è½è±å¤ä¹æ¶é´çå® `Vuex` çæ ¸å¿æºç ï¼æåæ­¥ç»èªå·±å®äº `15` å¤©çæéï¼é¢è®¡æ¯å¤©è³å°ç `2` å°æ¶ãäºæ¯ææ `Vuex` çæºç  `fork` å¹¶ `clone` äºä¸æ¥ï¼ç¬¬ä¸å¤©ç®åå°æ¾äºä¸ä¸æ ¸å¿ä»£ç çä½ç½®ï¼ç¶åéå¸¸ç²ç¥å°çäºä¸ä¸æºç éçå¤§è´æµç¨ãåæ¶ï¼æå» `Vuex` å®æ¹ææ¡£ééæ°ä»ä»ç»ç»å°åé¡¾äºä¸ä¸ææçæ ¸å¿ä½¿ç¨æ¹æ³

æ¥ä¸æ¥çæ¶é´æå°±æç§ææ¬æçéè¯»é¡ºåºè¿è¡æºç çéè¯»

è¿éæ»ç»å ç¹éè¯»æºç ç**å¿å¾ä½ä¼**å§ï¼

1. å¯¹äºè¿ä¸ªåºçä½¿ç¨ä¸å®è¦ååçç»ï¼å³æç½åç§æ¹æ³çä½¿ç¨ï¼å¼ºçå»ºè®®æå®æ¹ææ¡£åéï¼**éç¹**ï¼
2. æ¾å°æ ¸å¿ä»£ç çä½ç½®ï¼ä»å¥å£æä»¶å¼å§ï¼ä¸æ­¥æ­¥ç
3. å¤çæºç ä¸­çè±ææ³¨éï¼çä¸æçå¯ä»¥ç¨ç¿»è¯ï¼è¿äºæ³¨éåºæ¬ä¸è½å¸®ä½ çè§£è¿æ®µä»£ç çä½ç¨
4. éå°çä¸æçå°æ¹å¯ä»¥åæä¸ªå¤æ³¨ï¼å ä¸ºå®å¯è½ä¸åé¢çæäºä»£ç ææèç³»ï¼ç­ä¹ååå¤´æ¥çä¹åçä¸æçä»£ç æ¶ï¼å°±ä¼æç½äº
5. éè¯»æºç çè¿ç¨ä¸­ï¼çå°æäºåéæå½æ°æ¶ï¼åçå½åï¼å ä¸ºè¿äºå½åçå­é¢ææåºæ¬ä¸å°±ä»£è¡¨äºå®çä½ç¨ï¼ç¶åè¦å­¦ä¼èæ³å°è¿ä¸ªæ­£å¸¸çè°ç¨æ¯ä»ä¹æ ·çï¼è¿æ ·æ´ä¾¿äºçè§£
6. å¤å¤å©ç¨ç¼è¯å¨çæç´¢åè½ãå ä¸ºææ¶ä½ çå°çå½æ°æåéå¯è½å¨å«çå°æ¹ä¹æç¨å°ï¼ä¸ºäºæ¹ä¾¿å¯»æ¾ï¼å¯ä»¥å©ç¨å¥½ç¼è¯å¨çæç´¢åè½ï¼åæ¬å½å**æ¬å°æç´¢**å**å¨å±æç´¢**ï¼

![æ¬å°æç´¢](local-search.png)



![å¨å±æç´¢](global-search.png)

# ð æå

è¥æ¬ä»åºå¯¹äº `Vuex` æºç éè¯»æä»»ä½éè¯¯çå°æ¹ï¼æ¬¢è¿å¤§å®¶ç»ææ `Issues`ï¼ä¸å®èå¿å¬åä½ ä»¬çææ­£ï¼è§å¾æ¬ä»åºä¸éçï¼ä¹å¯ä»¥ç¹ä¸ª **star** æ¯æä¸ä¸æãæåï¼ä¹å¯ä»¥æ·»å æçå¾®ä¿¡ï¼`Lpyexplore333`ï¼ç§åºä¸è¿è¡äº¤æµ

