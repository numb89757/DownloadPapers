1. 从web of science选择文献，导出EndNote Desktop格式文件`savedrecs.ciw`.
2. 下载EndNote，导入上述`savedrecs.ciw`，![1.png](images%2F1.png)
新建一个自定义的Style，选择Bibliography - Templates，右侧insert Field 内选择DOI，保存。
![2.png](images%2F2.png)
    >=>编辑Edit\
    =>输出样式Output Style\
    =>新建输出样式New Style\
    =>参考文献Bibliography\
    =>模板Templates\
    =>插入DOI
    =>保存样式 \
    参考：https://www.bilibili.com/read/cv14968104/

3. EndNote选择File -> Export... 如下界面，在Output Style中选择第2步设置的格式DOI。记得是先点击Select Another Style...才能选择自定义格式。
![4.png](images%2F4.png)
![3.png](images%2F3.png)
保存到桌面，命名为`doi.txt`
4. 自行配置python环境，进入`main.py`, 把doi.txt的路径改为你自己的路径，并把pdf结果保存路径修改为你自己的路径。
5. 运行`main.py`, 等待下载即可！ 
（tips: 小概率下载失败，在生成的文件`./error.txt`中记录了下载失败的文献doi，一般是由于SCIHub中没有该文献的记录，没有下载
权限，这部分请各显神通自行解决😁）

