# TwitterDataProcessing 
[中文版](https://github.com/JinZhang666/TwitterDataProcessing/blob/master/README(%E4%B8%AD%E6%96%87).md)

## Project Summary 
1. Implemented a real-time processor with Spark for popular Twitter hashtags 使用spark实现对于twitter上面发帖的热门标签的实时统计
* split the data stream into words and add up count for each word separately 把数据流分隔成单词然后统计每个单词出现的次数
* We update count of each word based on last interval processing results 基于上一个区间处理数据的结果，我们更新每一个单词的数量
* Finally, we send those result to flask app 最后我们把那些结果送给了flask写的一个应用，它是一个可视化的应用

2. Designed and implemented positive/negative word monitor with Kafka and Spark (60 Tweets per second) 使用kafka和spark设计和实现对于积极词汇/消极词汇的监视

3. Optimized the processing with Flink with better efficiency and suitability 使用flink优化了数据处理的速度

4. Visualized the results with Ajax and Javascript chart for 1% of all public Tweets 使用ajax和Javascript实现数据的可视化

## Techiniques Used 
1. [spark](https://github.com/JinZhang666/TwitterDataProcessing/blob/master/Notes/Spark.md)
2. [kafka](https://github.com/JinZhang666/TwitterDataProcessing/blob/master/Notes/Kafka.md)
3. [flink](https://github.com/JinZhang666/TwitterDataProcessing/blob/master/Notes/Flink.md)
4. [scala](https://github.com/JinZhang666/TwitterDataProcessing/blob/master/Notes/Scala.md)

## Project Operations Log 
1. download scala: 使用linuxbrew这个包管理器进行下载
2. scala basic operations: 了解了scala一些基本的操作/语言特点: * 面向对象&函数式编程并存
3. download spark: 在apache的官网上下载了spark，spark的启动方法是到spark的文件夹里面跑一个叫做spark-shell的文件
4. spark basic operations: 了解了通过spark可以进行的基本操作，大概就是filter/map
5. 注册了twitter的开发者账号
6. twitterToSpark.py
