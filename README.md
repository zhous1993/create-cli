# create-cli
cli创建和发布
1. 新建文件夹 demo-cli
2. 在文件夹下执行 npm init
3. 创建index.js 并在顶部加上
  `#!/usr/bin/env node`
  标识在node环境中运行
4. 在package.json添加命令
  ```
  "bin": {
    "demo-cli": "./index.js"
  },
  ```
5. 安装依赖包 commander, shelljs, inquirer,download-github-repo,ora,chalk
  npm install --save commander shelljs inquire download-github-repo ora chalk
6. cli编码
  1. 输入路径
  2. 输入项目名
  3. 初始化项目名、版本号、作者、描述等信息,
  4. 下载模板
  5. 删除git信息
  6. 更新package.json
  7. cd到新项目，执行npm install
  8. 创建成功
7. 发布cli到npm
  1. 注册npm账号
  2. 在本地登录 
     执行npm adduser
  3. 运行 npm publish命令发布
8. 更新cli
  1. npm version <update_version>
  2. npm publish
