# 這邊是 玩決策樹時 值得紀錄的要點

## case 1

### 
當時我參考這個網站 打算用內建方法看看預測成效
```
http://psop-blog.logdown.com/posts/3128905-python-machine-learning-decision-tree-random-forest
```
我用了這個code
```
predictions = dtree.predict(predict_X)
from sklearn.metrics import classification_report,confusion_matrix
print(classification_report(predict_y,predictions))
print(confusion_matrix(predict_y,predictions))

```
結果出現了錯誤是
```
ValueError: continuous is not supported
```
解法：由於DTree可以用回歸＆分類，上面的方法是分類用的，但我的case是回歸！！
於是改用回歸的方法
```
DT_model.score(predict_X, predict_y)
```
```
reference:https://stackoverflow.com/questions/32664717/got-continuous-is-not-supported-error-in-randomforestregressor
```
