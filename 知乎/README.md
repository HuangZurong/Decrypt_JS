知乎登陆，无参提交破解；

其中包含最外层加密函数的解密和signature参数的解密。


模拟知乎登陆流程：1.获取初始网页cookie；  

2.获得验证码并验证，其中验证码包括静态验证码和点选验证码（选择倒置的文字），前者可用tensorflow构建CNN进行模型训练；后者提交形式是以选中倒置图片像素的数组的形式来进行提交，可调用打码平台进行破解；  

3.重写hamc算法以获得signature参数，并将其结合其他不变参数进行最外层函数加密；  

4.模拟登陆得到个人中心信息。  
