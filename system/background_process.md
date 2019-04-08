# Background Process

## 問題

使用 SSH 連實驗室 GPU 訓練模型，但 Command line 關閉卻會中斷

## 解決

使用 `nohup` 使令 或是 `Screen`
這次問題則是使用 nohup 來解決



## nohup 用法

[Reference](https://blog.gtwang.org/linux/linux-nohup-command-tutorial/)

```bash
# 讓程式登出後可繼續執行
nohup /path/my_program > out_file & #在尾端加上 & 把這個程式放在背景執行
```

nohup 預設輸出會在 nohup.out 裡面

我們可以使用 `cat`來觀看

```bash
cat nohup.out
```

或者使用 `tail` 自動即時顯示最新的輸出：

```bash
tail -f nohup.out
```

我們也可以把錯誤訊息分開成另一個檔案

```bash
nohup /path/my_program > my.out 2> my.err &
```

## Screen 用法

下次使用再補充