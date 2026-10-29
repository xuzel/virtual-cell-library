# AI4Science 虚拟细胞库 · 操作工作台

真实 scBaseCount 单细胞浏览器，每行一个细胞，支持筛选、排序、分页、表达详情、全基因精确查询及 CSV 导出。

## 已接入数据
- 来源：Arc Institute scBaseCount，2026-01-12 release
- 样本：ERX10300687，Homo sapiens
- 2122 个细胞，36601 个基因
- GeneFull_Ex50pAS / Unique：X 原始计数，无归一化
- 来源：https://storage.googleapis.com/arc-institute-virtual-cell-atlas/scbasecount/2026-01-12/h5ad/GeneFull_Ex50pAS/Homo_sapiens/ERX10300687.h5ad
- 细胞类型与本体编号沿用源文件；不虚构组织、疾病、处理或降维信息。

UMI 总数与检出基因从 X 重新计算。表达以每 100 个细胞一份 JSON 按需加载；稀疏矩阵未列出的值为 0。index.json 保留来源 URL 与源文件 SHA-256。原始 H5AD 不纳入 Git 仓库。不是全量 scBaseCount 镜像，也不提供模拟推断。

运行：python3 -m http.server 8766
