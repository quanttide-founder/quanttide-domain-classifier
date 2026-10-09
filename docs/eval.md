# 评测集

`eval.tsv` 是 ROADMAP 阶段 0 的首批评测数据，覆盖 5 个典型类别共 193 条片段，用于跑零样本基线并比较后续训练效果。

## 字段

| 字段 | 含义 |
| :-- | :-- |
| `id` | 类别前缀加三位序号 |
| `category` | 标注类别，取自 [category.md](./category.md) |
| `text` | 待分类片段，已压成单行 |
| `source` | 来源仓库与文件，形如 `repo#path` |
| `name_leak` | 片段是否出现该领域名，`yes` 为易样本 |

## 采样

来源限定为各领域根仓库 `.gitmodules` 中 `docs/*` 指向的子仓库，不取 `data/*` 陈述性记忆。知识工程的 `docs/*` 只接线了 gallery，另补同类的 `tutorial` 与 `specification` 两个仓库。

片段提取按空行切分正文，剔除 YAML 头、代码块、表格、纯标题、锚点导航、以「包括：」结尾的引出句，以及 `CHANGELOG.md` 等模板文件；去重后保留 20 至 900 字且含 15 个以上汉字的段落。取样按来源仓库轮转以避免单一大仓库垄断，随机种子 `20261010`，类别内按需放宽单文件上限。

## 统计

| 类别 | 条数 | 含领域名 | 来源仓库数 |
| :-- | --: | --: | --: |
| 元工程 | 40 | 6 | 6 |
| 软件工程 | 40 | 6 | 5 |
| 数据工程 | 40 | 11 | 5 |
| 知识工程 | 33 | 7 | 3 |
| 智能体工程 | 40 | 6 | 6 |

合计 193 条，其中 36 条含领域名。片段长度 20 至 387 字。

其余 45 个类别尚未采样，补齐后本文件的统计随之更新。

## 复现

```bash
python3 scripts/build_eval.py                      # 重建本文件已有类别
python3 scripts/build_eval.py --categories 元工程    # 指定类别
python3 scripts/build_eval.py --all                # category.md 全部类别
```

脚本读取 [category.md](./category.md) 得到领域与根仓库的对应关系，再取根仓库 `.gitmodules` 中 `docs/*` 指向的子仓库，按上述规则覆盖写入 `eval.tsv`；结果可复现，`--cache` 可复用克隆以加速。
