## Find minimum number of coins that make a given value
![werwer](https://github.com/mohammad-hasan-shahroodi/coins/assets/140893151/1578e7be-b284-41ae-8fb8-8cb7b262056b)
######
#### In this algorithm you find minimum number of coins that make a given value .
- ##### you should type your money at first:
  - ```python
    money = int(input())
    ```
- ##### After that you should type your type of your coins: #Example : 1 2 5 7 (it means you have only 1 , 2 , 5 , 7)
  - ```python
    coins = [int(i) for i in input().split()]
    ```
- ##### The principle of the algorithm is this piece
  - ```python
    for i in range(1,money+1):
    for j in coins:
        if j <= i :
            k = i - j
            if s[k]+1 < s[i]:
                s[i]=s[k]+1
    ```
