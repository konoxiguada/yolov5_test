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
+ result //存放了部分验证结果
```

## TODO：

* 引用**Selenium**对B站登录操作弹出的验证码做全自动文字点选。
* 以包的方式调用YOLO进行训练，而不是直接用YOLOV5官方提供的代码仓库
