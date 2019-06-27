# 人脸识别签到小程序
## 进度
- **2019/5/25**  
  实现了学生上传或者拍摄图片到云存储，并结合腾讯云人脸识别完成了人脸信息检测与分析，展示了上传照片的魅力值
- **2019/5/26**  
  - 实现了管理员创建人员库的操作
  - 实现了验证创建的人员库名称和id是否存在的功能
- **2019/5/27**  
  修复学生登录功能
- **2019/5/28**  
  实现学生登陆后上传相片至人员库
- **2019/5/30**  
  解决无法上传学号和姓名的问题
- **2019/6/2**  
  实现教师扫描学生检测其是否存在在该人员库的功能
- **2019/6/3**  
  修复学生重复上传人脸的问题
- **2019/6/7**  
  完成
## 遇到并解决的问题
- **2019/5/25**  
  在控制台删除云函数后，在本地修改后再次上传若失败可以在云函数根目录右键并选择同步云函数列表
- **2019/5/28**  
  - 本地云函数修改并保存后记得要上传至云
  - 获取创建人员接口的参数时报很多奇怪的错，发现是修改了const
  - 调用`wx.chooseImage()`后，`object.success`回调函数的参数`res`中的`attribute tempFilePaths`不是image或url
  - 用云文件ID换取真实链接的API是在服务端调用的，而非小程序端
- **2019.5.29**
  - 云函数中不需要`wx.`
  - app.js里的变量云函数怎么可能能访问
  - 云函数里常见的两个数字错误码不能提供任何帮助，应该检查依次各个变量是否使用错误
- **2019.5.30**  
  reset或checkout后要记得把与之前在云上的函数不同的函数再上传一次

