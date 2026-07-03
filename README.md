❄️ SQL 练习场

面向非计算机专业的 SQL 教学配套练习平台，纯前端、免安装、打开即用。

上海电力大学 · 《数据库原理及应用》课程配套。

🔗 在线访问

表格
通路	地址
GitHub Pages（主入口）	https://adelegirl.github.io/sql-lab/
EdgeOne（降级备份）	https://sql-lab-sqsjcoek.edgeone.cool/

四个页面均可独立访问：index.html / ddl.html / dml.html / dcl.html

📚 内容概览（v0.8）

表格
页面	主题	题量	说明
index	查询练习	50 题	SQLZoo 中文改编，SELECT 从入门到进阶
ddl	DDL 建表	15 题	CREATE / ALTER / DROP，覆盖约束、索引、视图
dml	DML 数据操作	15 题	INSERT / UPDATE / DELETE，含事务与批量操作
dcl	DCL 权限控制	15 题	GRANT / REVOKE / ROLE，虚拟权限矩阵模拟

统一业务场景：employee / department / project 三张表贯穿全部练习。

🛠️ 技术栈

sql.js（SQLite WebAssembly 编译版）—— 浏览器内直接执行 SQL
纯 HTML + CSS + JS，零依赖、零后端
进度保存在 localStorage（各页独立 key）

DCL 特别说明：SQLite 本身不支持 GRANT / REVOKE / ROLE。DCL 页面用虚拟权限矩阵模拟执行，页面顶部有诚实 banner 提示"本页 DCL SQL 不真跑在 SQLite"。

🎓 教学设计原则

4 口令：查询 / 修改结构 / 修改数据 / 权限 —— 对应 SELECT / DDL / DML / DCL 四大类
2 铁律：
每题必给验收标准
提示（hints）上限 3 条，不锁难度
主战场：机房 + 电脑，浏览器直接打开链接即可

📖 版本演进

表格
版本	里程碑	备注
v0.5	SQLZoo 中文版 25 题	初版单页
v0.6	扩展到 50 题	独立业务场景 employee/department/project
v0.7	拆分三页（index + ddl + dml）	双通路上线 GitHub Pages + EdgeOne
v0.8	新增 DCL 页面，四页齐活	主题色统一 GitHub 蓝 #0969da

📝 Credits

查询题库中文改编自 SQLZoo
教学场景与业务需求：上海电力大学《数据库原理及应用》
教材参考：赵明渊《数据库原理与应用(SQL Server)》电子工业出版社 2019

📄 License

教学非营利用途，改编 / 转载请注明出处。
