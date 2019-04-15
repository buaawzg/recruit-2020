# bytedance 04.14

## Test2 - 建筑物 玩游戏 能量值
能量值 `e`, 高度 `h`
```  
1. e > h: e += e - h  
2. e < h: e -= h - e  
3. 1 and 2  ==> e = e + e - h
```  
***从后往前: 最终状态 `e = 0`, 状态前移 `e >= 下一个 (e + h) / 2`***  
*ps: 程序中多加一个 `1` ,是为了奇数除以 `2`*