[![License](https://img.shields.io/badge/License-GNU%20AGPL%20V3-green.svg?style=flat)](https://www.gnu.org/licenses/agpl-3.0.en.html)
## License

web-apps is released under an GNU AGPL v3.0 license. See the LICENSE file for more information.

## 项目说明

本项目fork自 [ONLYOFFICE官方web-apps](https://github.com/ONLYOFFICE/web-apps)

现根据GUN AGPL v3.0协议开源本项目

## only-office 镜像打包流程

1. 编译 sdkjs 和 web-apps 两个工程，流程如下（如有需要）
2. web-apps 工程中的 index.html 变更项复制入 index.html.deploy 中（如有变更）
3. cd /build 目录，执行 grunt 命令
4. nginx/html 目录下，执行 build.sh，打包开发环境的 docker
5. cd /test 目录，执行 build.sh，打包并上传测试环境的 docker（如有需要）
6. cd /prod 目录，直接 build.sh、build2.sh，打包并上传正式环境的两个 docker
