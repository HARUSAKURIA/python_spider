## Xpath 主要知识点
- 使用xpath helper或者是chrome中的copy xpath都是从element中提取的数据，但是爬虫爬取的是url对应的响应，往往和element不一样
- 获取文本
  - `a/text()` 获取a下的文本
  - `a//text()` 获取a下的所有标签的文本
  - `//a[text()='']` 选择文本为下一页三个字的a标签
  
 - `@符号`
   - `a/@herf` 获取a下的属性
   - `//ul[@id='detail-list']` 获取任意标签下，属性`id='detail-list'` 的ul标签
  
 - `//`
   - 在xpath最前面表示从当前html中任意一个位置开始选择
   - `li//a` 表示的是li下任何一个a标签
  
