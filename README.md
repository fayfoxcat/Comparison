# erp

此模板应有助于您开始在Vite中使用Vue 3进行开发。

## 建议的IDE设置

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (并禁用Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## TS中 “.Vue” 导入的类型支持

默认情况下，TypeScript无法处理 “.vue” 导入的类型信息，因此我们将 “tsc” CLI替换为 “vue-tsc” 以进行类型检查。在编辑器中，我们需要 [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items？itemName=Vue. vscode-typescrip-vue-plugin) 来使typescript语言服务识别 “.vue” 类型。

如果独立的TypeScript插件感觉不够快，Volar还实现了一个性能更高的 [接管模式](https://github.com/johnsoncodehk/volar/discussions/471 # discussioncomment-1361669)。您可以通过以下步骤启用它:

1.禁用内置的TypeScript扩展
1) 从VSCode的命令面板运行 “扩展: 显示内置扩展”
2) 找到 “typescript和JavaScript语言功能”，右键单击并选择 “禁用 (工作区)”
2.通过从命令面板运行 “开发人员: 重新加载窗口” 来重新加载VSCode窗口。
## 自定义配置

请参见 [Vite配置参考](https://vitejs.dev/config/).

## 项目设置

```sh
npm install
```

### 编译和热重载开发

```sh
npm run dev
```

### 为生产进行类型检查、编译和缩小

```sh
npm run build
```
