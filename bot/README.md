## 注意⚠️
整体逻辑是：
1. 登录amazon
2. 输入关键字
3. 点击商品 获取商品 标题、价格、图片、联盟营销链接、时间戳
4. 将数据同步`firestore.client()`
5. 回到搜索结果页 换下一个商品，重复3.


### Python script configuration.

In order to run the python script you will need to run the following command with pip. 

```
pip install -r requirements.txt 
```

⚠️Note: It seems that "firebase-tools" only works with Python3.7.5. So try installing these version if the pip install doesn't work.  

### Running script
After intalling all the libraries, setting up your proyect in firebase, downloading your firebase credentials and creating your affiliate account, your are ready to run: 
``` 
python myBot.py 'your firebase category' 'your amazon search'
```
And then magic will happen, amazon results will be in your firebase database. 
