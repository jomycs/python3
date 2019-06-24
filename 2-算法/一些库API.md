## header=None
1.获取数据内容。pandas.read_csv(“data.csv”)默认情况下，会把数据内容的第一行默认为字段名标题。
为了解决这个问题，我们添加“header=None”，告诉函数，我们读取的原始文件数据没有列索引。因此，read_csv为自动加上列索引。

注意，有"header=None", df.ix[:,0:4]就是左闭右闭的区间
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;没有"header=None", df.ix[:,0:4]就是左闭右开的区间

## os.sep
os.sep:分隔符，windows下是‘\’.linux下是‘/’
os.path.join(...)：将多个路径组合后返回
os.sep.join(...)：连接字符串数组

## numpy 将多维数组转换为一维数组
ravel()：如果没有必要，不会产生源数据的副本 
flatten()：返回源数据的副本 
squeeze()：只能对维数为1的维度降维

另外，reshape(-1)也可以“拉平”多维数组


