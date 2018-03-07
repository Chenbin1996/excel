
# Java Excel
- 使用Java封装操作excel文件
# 特点
- 基于POI框架，封装操作excel，操作简单易懂
# 操作
1. 在实体类中加上如包内shopDTO类上的注解@ExcelSheet，name属性中是excel的sheet名称，若是默认excel的sheet1名称，name中写上sheet1即可，等价于navicat导入数据库相同， 要选择一个表，@ExcelField注解是表中的字段所对应的excel列名称
2. 导出操作只需要在随意一个controller类中或者有main的类中写上ExcelExportUtil.exportToFile(“路径”, 数据List)即可
3. 导入操作只需要在随意一个controller类中或者有main的类中写上ExcelImportUtil.importExcel(注解过的类名.class, 路径)即可
4. 详情查看test包中的ExcelTest类
5. service层操作查看个人博客 http://blog.csdn.net/m0_37701381/article/details/79217495
