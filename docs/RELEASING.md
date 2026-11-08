# 正式发布流程

## 主站与版本

主站：https://shen-dongshan.github.io/bianjing-sishi/

仓库：https://github.com/Shen-Dongshan/bianjing-sishi

当前发行版：`V13_bianjing`。后续正式功能版本连续编号，发行版标题和标签采用`Vxx_bianjing`，日期以Europe/Budapest的实际发布时间记录。

## 网页资源

正式版网页资源以Release附件`site.zip`发布，根目录包含`index.html`。包内包含页面脚本、样式、画卷、字体与音频；发布前核对所需资源清单、版权来源和文件摘要。

GitHub自动生成的Source code压缩包对应仓库中的文档与发布配置。完整可运行网页请选择Release附件`site.zip`。

## 发布步骤

1. 在工作目录完成修改、资源核验和浏览器检查，按正式版本生成纯网页资源包。
2. 建立对应Release，采用`Vxx_bianjing`命名，上传审核后的`site.zip`，填写更新内容、作者版权、运行方法和SHA-256。
3. 更新`.github/workflows/pages.yml`中的资源包下载地址、预期SHA-256、文件数与展开字节数。工作流先校验再部署。
4. 以正常快进提交更新main，保留历史记录。等待Pages工作流成功，并检查主站实际页面及资源。
5. 完成正式档案，更新README、CHANGELOG及`docs/releases/`中的逐版记录，核对链接与线上内容。

## 日志与历史

V01–V13的历史日志保留原发布时的事实、代码提交时间、成功发布时间和素材实现边界。后续版本记录GitHub提交、Release和Pages成功部署依据。

正式版本保留独立快照与素材来源。草稿在工作目录迭代；同一版的说明和署名修订可补充记录，无须新增功能版本号。

## 作者及素材

作者：Shen Dongshan。项目与各类素材的署名、来源、许可及待核实事项统一维护于README、网页作者版权说明和资源包中的来源清单。记录版权状态时，以已有依据为准。
