---
layout: post
title: Length of Last Word
tags: [thuật toán, leetcode, xử lí xâu, mức dễ]
---

Thuật toán giải bài Length of Last Word bằng ngôn ngữ lập trình Python với thời gian chạy 8ms nhanh hơn 99.58% người dùng khác trên Leetcode.

### Đề bài 
### Tìm độ dài của từ cuối cùng trong xâu.

[Length of Last Word - Leetcode](https://leetcode.com/problems/length-of-last-word/)

Cho bạn một xâu S bao gồm các kí tự thường/viết hoa và các khoảng trắng ' '.
Yêu cầu bạn trả về độ dài của từ cuối cùng trong xâu S đã cho ban đầu.

Nếu từ cuối cùng không tồn tại trả về 0.

####   Chú ý
* Từ cuối cùng là từ được tính từ trái sang phải của xâu.
* Một chuỗi con tối đa được định nghĩa không bao gồm các kí tự khoảng trắng ' '.

### Ý tưởng thuật toán

Vấn đề ở đây là cần tìm vị trí dấu cách đừng trước từ cuối cùng. Để làm được điều này ta cần phải xoá những dấu cách thừa ở cuối xâu ([`rstrip()`](https://python-reference.readthedocs.io/en/latest/docs/str/rstrip.html)).

Sau đó dùng ([`rfind()`](https://python-reference.readthedocs.io/en/latest/docs/str/rfind.html)). để tìm vị dấu cách cuối cùng.

Độ dài cần tìm chính là khoảng cách từ sau vị trí đó đến cuối xâu.

![alt text](https://i.ibb.co/VmSvxkg/white.png "Length of Last Word")

### Solution in Python


```python
def lengthOfLastWord(s):
    s = s.rstrip()
    x = s.rfind(' ')
    return len(s)-x-1
```