# 基于机器学习的商品匹配研究
随着电商行业飞速发展，越来越多的消费者选择网上购物，实体经济逐渐向数字经济转型。为了帮助消费者实现快速商品比价，可将深度学习中的计算机视觉和自然语言处理等技术应用到商品匹配研究中去。
针对商品匹配任务，本文从商品图像匹配和商品文本匹配两个角度分别建立模型。在商品图像匹配中选用了较为先进的卷积神经网络系列中的基线网络EfficientNet-B0。首先使用EfficientNet-B0提取出商品图像特征，接着采用KNN模型找到图像特征最匹配的商品。在商品文本匹配中，通过TF-IDF模型判断不同词在商品标题中的重要程度，找到能代表对应商品的词语，提取出商品标题中的文本特征向量，再根据余弦相似度算法对不同商品标题中的代表性词语进行相似性度量，得到文本特征最匹配的商品。最后把基于商品图像匹配出的预测商品与基于商品文本匹配出的预测商品进行多模态融合，得到最终的商品匹配结果，并且最后得到的F1-score为0.70。

With the rapid development of e-commerce industry, more and more consumers choose to shop online, and the real economy is gradually transforming into a digital economy. In order to help consumers achieve fast product comparison, techniques such as computer vision and natural language processing in deep learning can be applied to product matching research.
For the product matching task, this thesis builds models from two perspectives: product image matching and product text matching. In the product image matching, the baseline network EfficientNet-B0 in the more advanced convolutional neural network series is selected. First, EfficientNet-B0 is used to extract the product image features, and then the KNN model is used to find the product with the best matching image features. In the product text matching, the TF-IDF model is used to determine the importance of different words from the product title. The text feature vector of the product title is then extracted by finding the words that represent the corresponding product. Then, according to the cosine similarity algorithm, the similarity measurement of the representative words in the titles of different products is carried out, and the product with the best matching text features is obtained. Finally, the predicted products based on product image matching are fused with the predicted products based on product text matching in a multimodal manner to obtain the final product matching results, and the final F1-score is 0.70.

EDA代码1：https://www.kaggle.com/code/brianna1307/eda-part1

EDA代码2：https://www.kaggle.com/code/brianna1307/eda-part2

模型建立与训练代码：https://www.kaggle.com/code/brianna1307/model-building-and-training
