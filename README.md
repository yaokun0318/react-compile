## 编译、构建、工程化学习清单

从 0 开始，从官网的 guide 开始，不要照着现有项目抄代码

### npm：包管理

1. npm7 wordspace
2. npm7 对 package-lock 的修改
3. npm7 对 peerdependency 的策略
4. lerna（可选）

### babel、webpack、typescript：传统的 bundle 编译手段

1. corejs 配置策略
2. webpack terser 压缩器
3. tsc 单独执行类型检查
   一定对照编译后的结果来看

### esbuild、vite、snowpack：es module 编译手段

0. 理解为什么会出现 esbuild
1. 学习使用 esbuild-register 替代 ts-node，提升 ts 代码解释速度，思考和 ts-node 的不同之处
2. 学习 vitejs 的 bundle 模式（production 使用非 es module，而采用传统的编译方式）
3. 学习 snowpack 的 webpack 模式
   一定对照编译后的结果来看

### prettier、eslint、stylelint：代码质量管理

1. 对 ts 代码配置 eslint 和 prettier
2. 对 styled-components 或别的 css 预处理器代码配置 stylelint

### tsdx、rollup：库开发

1. 学习使用 rollup vue plugin 输出 js 模块
2. 学习使用 tsdx 输出 js 模块
3. 在学习 tsdx 过程中加深 npm 的 dev dependency、dependency、peer dependency 理解
4. Semver

### jest、cypress：测试自动化

1. 单元测试和 E2E 测试概念
2. 学习在 jest 中测试 typescript
3. 学习用 cypress 模拟点击
4. 将测试流程集成到某种 ci 里面去（推荐用自己的 github 尝试 circle ci 和 travis ci）
5. 学习输出测试覆盖率

### 进阶：编译器学习，babel 插件开发
