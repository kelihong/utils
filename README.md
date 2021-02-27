# @kelihong/utils



### Why?

<div style="background-color: #eee; padding-left: 10px;">
	<b>TL;DR </b> Let coding easier.
</div>

常用方法集合，为了使开发更方便。

### Getting started

##### install 

via  `npm`

```shell
npm install @kelihong/utils --save
```



##### use

```
import zkutil from ''
```



*the notes after every methods means the return value*

1. `cookie` settings:

   ```javascript
   // set
   setCookie(cname, cvalue, exdays) // true
   
   // get
   getCookie(cname) // cvalue
   
   // remove
   removeCookie(key) // cname
   
   ```



2. `localStorage`  settings:

   ```javascript
   // set
   setStorage(key, value) // true
   
   // get
   getStorage(key) // value
   
   // remove
   removeStorage(key) // key
   
   // clear
   clearStorage(key) // undefined
   ```

   

3. random data

   ```javascript
   // number
   // default value: max = 1, min = 0
   randomNum({max=1, min=0})
   
   // color
   // format: rgb(0,0,0)
   randomColor() // rgb(value, value, value)
   ```

   

4. colorful `console.log`:

   ```javascript
   log()
   ```

   

5. create a document element （ DON'T USE IT )

   ```javascript
    createEl({
       parentNode: document.body, // parent node
       tagName: 'div',	// new element's tagName
       id: '', // the id of new el
       classLists: [], // classlist of new el
       html: '',	// innerHTML of new el
       styles: {}, // inline style
       otherAttr: {} // attribute inside new element tags
   })
   
   ```

   



```javascript

    setCookie, // 设置 cookie
    getCookie, // 获取 cookie
    removeCookie, // 清空 cookie
    setStorage,// 设置 localStorage
    getStorage, // 获取 localStorage
    removeStorage, // 移除 localStorage
    clearStorage, // 清空 localStorage
    createEl, // 创建 DOM 元素
    isEmpty, // 判断表单是否为空
    randomNum, // 生成随机数
    randomColor, // 生成随机颜色
    log, // 改良版 console.log

```

