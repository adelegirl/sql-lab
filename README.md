---
AIGC:
    Label: "1"
    ContentProducer: 001191110102MACQD9K64018705
    ProduceID: 7633258890624368931-data_volume/files/所有对话/主对话/数据库课程/SQL练习场/README.md
    ReservedCode1: ""
    ContentPropagator: 001191110102MACQD9K64028705
    PropagateID: 3159351570729316#1783173593040
    ReservedCode2: ""
---
# ❄️ SQL 练习场

> 面向**非计算机专业**的 SQL 教学配套练习平台，纯前端、免安装、打开即用。
> 上海电力大学 · 《数据库原理及应用》课程配套。

---

## 🔗 在线访问

| 通路 | 地址 |
|---|---|
| GitHub Pages（主入口） | https://adelegirl.github.io/sql-lab/ |
| EdgeOne（降级备份） | https://sql-lab-sqsjcoek.edgeone.cool/ |

四个页面均可独立访问：`index.html` / `ddl.html` / `dml.html` / `dcl.html`

---

## 📚 内容概览（v0.10）

| 页面 | 主题 | 题量 | 说明 |
|---|---|---|---|
| **index** | SELECT 查询练习 | 50 题 | SQLZoo 中文改编，SELECT 从入门到进阶 |
| **ddl** | DDL 数据定义 | 15 题 | CREATE / ALTER / DROP，覆盖约束、索引、视图 |
| **dml** | DML 数据操纵 | 15 题 | INSERT / UPDATE / DELETE，含事务与批量操作 |
| **dcl** | DCL 数据控制 | 15 题 | GRANT / REVOKE / ROLE，虚拟权限矩阵模拟 |

**统一业务场景**：`employee` / `department` / `project` 三张表贯穿全部 95 题练习。

---

## 📝 学习报告（v0.10 亮点）

每个页面右侧进度面板提供**「导出学习报告」**按钮，一键生成教师批改友好的**单文件 HTML 报告**：

- **学号识别**：导出前弹窗收集学号，本地记忆下次自动预填，Enter/Esc 快捷提交
- **可视化统计**：GitHub 蓝渐变头卡 + 4 大数字统计（通过率 / 通过 / 尝试 / 看过答案）
- **分组明细**：每个题组独立表格，带绿色通过率进度条
- **三栏 badge**：已通过 / 尝试未通过 / 看过答案 一目了然
- **打印友好**：内置 `@media print` 样式，可直接打印归档

文件命名：`SQL练习场_[模块]学习报告_{学号}_{日期}.html`

---

## 🛠️ 技术栈

- **sql.js**（SQLite WebAssembly 编译版）—— 浏览器内直接执行 SQL
- 纯 HTML + CSS + JS，零依赖、零后端
- 进度保存在 `localStorage`（各页独立 key，三态追踪：通过 / 尝试 / 看过答案）

**DCL 特别说明**：SQLite 本身不支持 GRANT / REVOKE / ROLE。DCL 页面用**虚拟权限矩阵**模拟执行，页面顶部有诚实 banner 提示"本页 DCL SQL 不真跑在 SQLite"。

---

## 🎓 教学设计原则

- **4 口令**：`查询 / 修改结构 / 修改数据 / 权限` —— 对应 SELECT / DDL / DML / DCL 四大类
- **2 铁律**：
  1. 每题必给验收标准
  2. 提示（hints）上限 3 条，不锁难度
- **主战场**：机房 + 电脑，浏览器直接打开链接即可

---

## 📖 版本演进

| 版本 | 里程碑 | 备注 |
|---|---|---|
| v0.5 |  中文版 25 题 | 初版单页，老 repo `adelegirl/sql-playground` 冻结留念 |
| v0.6 | 扩展到 50 题 | 独立业务场景 employee/department/project |
| v0.7 | 拆分三页（index + ddl + dml） | 双通路上线 GitHub Pages + EdgeOne |
| v0.8 | 新增 DCL 页面，四页齐活 | 主题色统一 GitHub 蓝 `#0969da` |
| v0.9 | 右侧进度面板 + 三态追踪 + 学习报告初版 | JSON 格式报告 |
| **v0.10** | **学号识别 modal + HTML 表格版学习报告** | 教师批改视觉友好，可打印归档 |

---

## 📝 Credits

- 查询题库中文改编自课程题库 
- 教学场景与业务需求：上海电力大学 经济与管理学院 数据库原理及应用 课程

---

## 📄 License

教学非营利用途，改编 / 转载请注明出处。

---

> 本内容由 Coze AI 生成，请遵循相关法律法规及《人工智能生成合成内容标识办法》使用与传播。
