# Privacy Policy Generator - LazyCat App

[App Privacy Policy Generator](https://github.com/nisrulz/app-privacy-policy-generator)（为移动应用生成定制隐私政策与服务条款）的懒猫微服（LazyCat）打包。

## 镜像来源

镜像由 [dockers-x/app-privacy-policy-generator](https://github.com/dockers-x/app-privacy-policy-generator) 自动构建：nginx 托管上游 `public/` 中的预构建静态站（168 个文件、多语言），跟随上游 tag 推送 `ghcr.io/dockers-x/app-privacy-policy-generator:{version,latest}`。

- **镜像模式（mirror）**：经 `ghcr.nju.edu.cn` 加速拉取，digest 校验与 GHCR 一致
- **自动跟随上游**：每日检查上游 semver tag
- **喵喵商店发布**：仅私有商店

## 说明

- 纯静态应用，无后端/数据库，无数据卷
- 页面数据全部在浏览器本地生成，不包含任何用户数据上传
- 健康检查 `/healthz`

## 所需 Secrets

| Secret | 说明 |
| --- | --- |
| `APPSTORE_URL` / `APPSTORE_TOKEN` | 喵喵商店 API 地址与发布令牌 |
| `APP_ID` | 可选 |
| `PRIVATE_STORE_GROUP_CODES` | 可选，私有分组码 |

## 许可

AGPL-3.0（上游）
