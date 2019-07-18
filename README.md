# pgsql_etl源码参照
1 history_clean_json表  是一个逻辑表，把data_value字段进行网上json格式解析后，就能看到它里面的字段。百度关键字查询json选一个在线解析网，均可解析。
2 标志位说明：
3 解析后的数据字段flag  代表状态（F停运 M维护 A超标 S测试 D故障 C校准 q临界超标，K考核），其中 A超标 q临界超标 N正常 是参与计算的有效数据。

4 站点名称和检测设备号对照表（在dms）
mn_code                                                     对应站点名称
06057581301001 河涌监测站点 cf3fc05943444baba27b14ff87ab8513 泌冲大桥
06057581301002 河涌监测站点 8b8460a52f3844f3ad9f9dce6c744f94 里水河
06057581301003 河涌监测站点 f617483ab30b4690ba1c809ed3f6df8a 鲁岗涌
06057581301004 河涌监测站点 ddb2a33a7f74408da13425fd7f501f7e 文教埠头
06057581301005 河涌监测站点 0e515c0f43724f3ea8e999ad6f712be4 雅瑶水道
06057581301006 河涌监测站点 e8958479821d489ca6613c54ac4e1813 黄岐
06057581301007 河涌监测站点 d2a1457d916f430aba19c5eb84387e88 西航道入境
06057581301008 河涌监测站点 92c05295a70e49e3a68ec93744995e5b 和顺大桥

5 指标名称与参数对照表
101 ：总磷
"060": 氨氮
"W01": 水温
"W02": 溶解氧
"W07":高锰酸盐
001： PH
