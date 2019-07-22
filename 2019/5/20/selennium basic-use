# selennium 基础用法

- selennium是一个web自动化测试工具，可以接收指令，驱动浏览器，获取数据，截取屏幕画面
- PhantomJS是无界面浏览器，把网站加载到内存中，可以截屏网页

```python
# coding=utf-8
from selenium import webdriver
import time

#实例化一个浏览器对象
driver = webdriver.Chrome()
# phantomJS是一个无界面浏览器
# driver = webdriver.PhantomJS()

#设置窗口大小（分辨率）
# driver.set_window_size(1920,1080)

#最大化窗口
driver.maximize_window()

#发送请求，驱动浏览器访问
driver.get("http://www.baidu.com")

#进行页面截屏（存放地址）
driver.save_screenshot("./baidu.png")

#元素定位的方法
driver.find_element_by_id("kw").send_keys("python")
driver.find_element_by_id("su").click()

# driver 获取html字符串
print(driver.page_source) #浏览器中elements的内容

# 打印当前浏览器的url地址，
print(driver.current_url)

#driver获取cookie
cookies = driver.get_cookies()
# 得到一个列表，列表中为字典类型的cookies
print(cookies)
# print("*"*100)
# 字典推导式组成一个字典
cookies = {i["name"]:i["value"] for i in cookies}
# print(cookies)


time.sleep(3)
# 关闭当前页面
driver.close()
# 退出浏览器（主要使用）
driver.quit()
```
