# music
## rem配置
+ 安装
  ```   
    1.  npm install postcss-pxtorem --save-dev  用于把页面的px=>rem
    2.  npm install lib-flexible --save   用于根据设备宽度计算html的font-size
    3.  postcss.config.js 添加插件
        "postcss-pxtorem": {
            "rootValue": 37.5, // 设计稿宽度的1/10,（JSON文件中不加注释，此行注释及下行注释均删除）
            "propList":["*"] // 需要做转化处理的属性，如`hight`、`width`、`margin`等，`*`表示全部
        }
    4. main.js 引入 lib-flexible

  ```
