# Github 使用 LaTex 問題

## 問題

在 HackMD 上寫 LaTex 是使用 ＄ 包起來，但是將 markdown 下載下來並放上 github 卻是只有文字符號，ex: $\sum_{k=1}^{N}(Predict_k-y_k)^2$

## 解決

可以使用 LaTex 網站 codecogs 的云服务，把我們要的數學公式經由這個服務轉成圖片網址

Usage

```
![](http://latex.codecogs.com/gif.latex? + LaTex文字)
```

EX:

```
![](http://latex.codecogs.com/gif.latex?\sum_{k=1}^{N}(Predict_k-y_k)^2)
```

![](<http://latex.codecogs.com/gif.latex?\sum_{k=1}^{N}(Predict_k-y_k)^2>)
