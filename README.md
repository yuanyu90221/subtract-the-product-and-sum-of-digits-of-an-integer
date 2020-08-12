# subtract-the-product-and-sum-of-digits-of-an-integer

## 題目解讀：

### 題目來源:

[subtract-the-product-and-sum-of-digits-of-an-integer](https://leetcode.com/problems/subtract-the-product-and-sum-of-digits-of-an-integer/)

### 原文:
Given an integer number n, return the difference between the product of its digits and the sum of its digits.

### 解讀：

給定一個正整數 n

回傳 n的每個digit相乘 減去 n的每個digit相加的結果

舉例來說:

n = 234

f(n) => 2 * 3 * 4 - 2+3+4= 24 - 9 =15

## 初步解法:
### 初步觀察:

首先是每個digit取得可以透過 %10得到的結果

然後在用/10 去shift到下一個digit

n = 234 => check n > 0 , n % 10 = 4, n /= 10 
n = 23 => check n > 0 , n % 10 = 3, n /= 10
n = 2 => check n > 0, n % 10 = 2, n /= 10
n = 0
### 初步設計:

given an integer n

step 0: let a integer sum = 0, a integer product = 1

step 1: if n <= 0 go to step 3

step 2:  sum += n%10, product*= n%10, n/=10, go to step1

step 3: return product - sum
## 遇到的困難
### 題目上理解的問題
因為英文不是筆者母語

所以在題意解讀上 容易被英文用詞解讀給搞模糊

### pseudo code撰寫

一開始不習慣把pseudo code寫下來

因此 不太容易把自己的code做解析

### golang table driven test不熟
對於table driven test還不太熟析

所以對於寫test還是耗費不少時間
## 我的github source code

## 測資的撰寫



## 參考文章

[golang test](https://ithelp.ithome.com.tw/articles/10204692)