要手动创建一个webpack.config.js文件

```
const path = require('path')
var htmlwebpackplugin=require('html-webpack-plugin')
module.exports = {
    mode: 'development',
    entry:path.join(__dirname,'./src/main.js'),
    output:{
        path:path.join(__dirname,'./dist'),
        filename:'bundle.js'
    },
    plugins:[
        new htmlwebpackplugin(
            {
                template:path.join(__dirname,'./src/index.html'),
                filename:'index.html'
            }
        )
    ],
    module:{
        rules:[
            {test:/\.css/,use:['style-loader','css-loader']},

        ]
    }
```

