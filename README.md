# 桃園機場B類駕照推薦碼

這個 repo 的 `codes.txt` 是 Android APP 的線上推薦碼清單。

APP 會讀取：

```text
https://raw.githubusercontent.com/Chu0019/codes.txt/main/codes.txt
```

## 格式

一行一組推薦碼。以 `#` 開頭的行會被忽略。

```text
# 永久有效
VIP2026

# 永久有效，也可以明確寫 permanent
VIP2026,permanent

# 有效到 2026-12-31 當天
AIRPORT2026,2026-12-31
```

也支援以下分隔方式：

```text
AIRPORT2026|2026-12-31
AIRPORT2026 2026-12-31
```

## 注意

- 日期格式固定為 `yyyy-MM-dd`。
- 到期日當天仍有效，隔天開始無效。
- 推薦碼不分大小寫。
- APP 也有內建備援推薦碼；GitHub 連不上時會使用內建清單。
