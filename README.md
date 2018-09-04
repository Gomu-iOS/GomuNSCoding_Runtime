# GomuNSCoding_Runtime

归档解档
归档和解档需要对每个属性都实现一遍encodeObject:forKey:和decodeObjectForKey:方法，这样就会显得比较繁琐，但是我们可以利用Runtime获取所有属性来重写归档解档方法。

创建一个NSObject的分类@interface NSObject (Runtime)：

![image](https://github.com/PBgitHub/MyImage/raw/master/git_Image/GomuNSCoding_RuntimeImage/GomuNSCoding_RuntimeImage1.png)

归档的.m中的协议方法中分别调用这两个方法：

![image](https://github.com/PBgitHub/MyImage/raw/master/git_Image/GomuNSCoding_RuntimeImage/GomuNSCoding_RuntimeImage2.png)
