## 任务背景
用户确认数据管理Tab正常后，点击「导出Excel」报错tuple index out of range。

## 执行过程
1. 排查发现export_excel函数hardcoded row索引与数据库schema不一致
2. DB只有14列，代码用row[15]读infantry_grade导致越界
3. 与/api/list同样的问题根源
4. 修复：改用PRAGMA table_info动态获取列名，按列名映射替代hardcoded索引
5. 服务已重启

## 关键结果
- ✅ 导出Excel越界修复
- PRAGMA动态获取列名替代hardcoded索引
- 修改文件：app.py

## 结论建议
用户可再次测试导出Excel功能。