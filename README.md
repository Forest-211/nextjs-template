<p align="center">
  <img src="https://user-images.githubusercontent.com/26466516/141659551-d7ba5630-7200-46fe-863b-87818dae970a.png" alt="Next.js TypeScript Starter">
</p>

<br />

## Features

- ⚡️ Next.js 12
- ⚛️ React 17
- ⛑ TypeScript
- 📏 ESLint -查找并修复代码中的问题
- 💖 Prettier — 代码格式化器以保持一致的风格
- 🐶 Husky — 用于在提交之前运行脚本
- 📄 Commitizen — 定义提交规则的标准方式
- 🚓 Commitlint — 确保您的提交消息遵循约定
- 🚫 lint-staged — 针对暂存的 Git 文件运行 ESLint 和 Prettier
- 👷 CI/CD — git action 自动化部署
- ⚙️ EditorConfig - 跨编辑器和 IDE 保持一致的编码风格
- 🗂 路径映射 — 使用 `@` 前缀导入组件或图像

## 基于此项目创建
此项目是基于 [Create Next App](https://nextjs.org/docs/api-reference/create-next-app)脚手架创建
```
yarn create next-app -e https://github.com/Forest-211/nextjs-template
# or
npx create-next-app -e https://github.com/Forest-211/nextjs-template
```

### 启动项目

```bash
# 安装依赖
$ yarn install

## 运行项目
$ yarn dev
```
成功运行之后访问：`http://localhost:3000`

### 目录结构

```tree
.
├── .github
├── .husky
├── .next
├── public
├── src
│   ├── pages
│   └── styles
├── .commitlintrc
├── .editorconfig
├── .eslintrc
├── .gitignore
├── .npmrc
├── .nvmrc
├── .prettierrc
├── LICENSE
├── next-env.d.ts
├── next.config.js
├── package.json
├── README.md
├── renovate.json
├── tsconfig.json
└── yarn.lock
```

### Scripts

- `yarn dev` — 在开发模式下启动应用程序，运行成功后访问 `http://localhost:3000`
- `yarn build` — 构建应用程序的生产版本
- `yarn start` — 在生产模式下启动应用程序
- `yarn type-check` — 使用 TypeScript 编译器验证代码
- `yarn lint` — `eslint` 检查 `src` 文件夹下的所有文件
- `yarn format` — `prettier`  检查 `src` 文件夹下的所有文件
- `yarn commit` — git提交； 替代`git commit`

### 路径映射
预先配置了自定义路径映射。 要导入组件或文件，请使用 `@` 前缀。

```tsx
import { Button } from '@/components/Button';

// To import images or other files from the public folder
import avatar from '@/public/avatar.png';
```
