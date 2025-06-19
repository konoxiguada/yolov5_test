# Geetest文字点选验证码训练练习

使用了yolov5官方提供的[代码仓库](https://github.com/ultralytics/yolov5)，根据环境配置中numpy版本较高而对yolov5官方的部分数据类型做出了修改，

该模型能够框选出验证码中的图案或文字部分，文件夹结构如下：

```markdown
+ myimg
  + images //Geetest文字点选原始图片集
  + labels //标签集
+ runs
    + train
      + exp1 //YOLOV5训练结果
    + detect //YOLOV5验证结果
+ models //模型集合
  +yolov5s_captcha //训练用模型配置文件
+ utils //工具函数
+ weights
  + yolov5s //预训练模型
+ data
  + captcha //配置文件
```
* 调研——CNN无法解决图案类识别问题——YOIOV5——获取验证码集合——YOLOV5训练——验证结果——学习使用github——学习markdown语法
## TODO：

* 引用**Selenium**对B站登录操作弹出的验证码做全自动文字点选。
* 以包的方式调用YOLO进行训练，而不是直接用YOLOV5官方提供的代码仓库
![项目实战思路](https://github.com/konoxiguada/yolov5_test/blob/main/%E9%A1%B9%E7%9B%AE%E5%AE%9E%E6%88%98%E6%80%9D%E8%B7%AF.png?raw=true)
