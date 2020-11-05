# midas-test

1. ตั้งนาฬิกาทรายอันที่ 2 ให้เหลือครึ่งนึงก่อน จากนั้นเริ่มต้มไข่ พออันที่ 2 หมด ก็ให้ตั้งอันแรก
1. โต๊ะ = 150 cm, แมวสูงกว่าเต่า 20 cm
1. เล่นบาคาร่าตาละ 10 บาทแทงฝั่งเดียวตลอด ถ้าแพ้ให้เพิ่มเงิน 2.35 เท่า ถ้าชนะให้กลับมาเริ่มที่ 10 บาทเหมือนเดิม แล้วทำอย่างงี้ไปเรื่อยๆ ซึ่งจะสามารถแพ้ได้ติดต่อกัน 8 ครั้ง ซึ่งโอกาสเกิดเท่ากับ 0.390625%

1. (โจทย์น่าจะลืมบอกว่าความเร็วจะอิงจากคนที่ช้าที่สุดรึป่าวครับ)
    1. A ไปกับ B เวลา = 2
    1. A กลับมา เวลา = 1
    1. C ไปกับ D เวลา = 8
    1. B กลับมา เวลา = 2
    1. A ไปกับ ฺB เวลา = 2
เวลาทั้งหมด = 15

1. axios javascript เพราะ javascript เป็นภาษาที่เหมาะกับการจัดการ website อยู่แล้ว และ axios ก็เป็น tool พื้นฐานที่ใช้กับ javascript farmwork ได้ทุกอัน

1. Python และ Java\
Python เป็นภาษาที่ง่ายเพราะ dynamic type ซึ่งเหมาะสำหรับการใช้งานทางด้าน data science\
Java เป็นภาษา OOP และ เป็น static type ซึ่งเหมาะสำหรับพัฒนาโปรเจคใหญ่ๆ

1. ถ้าทาง Web ผมคงยกให้ javascript เพราะถนัดแค่ภาษาเดียวก็เขียนได้ทั้ง front-end และ back-end แต่ถ้าเป็นอนาคตผมยกให้ Kotlin เพราะเป็นภาษาที่พัฒนามาจาก Java แต่เขียนง่ายขึ้นและยังคงข้อดีของ Java ไว้

1.  

```python
def extract(text):
    target_first = 'Hello'
    target_last = 'world'
    len_tf = len(target_first)
    len_tl = len(target_last)
    index_first = 0
    index_last = 0
    if len(text) > len_tf + len_tl + 2:
        for i in range(len(text)-len_tf+1):
            if text[i] == target_first[0] and text[i+1] == target_first[1] and text[i+2] == target_first[2] and text[i+3] == target_first[3] and text[i+4] == target_first[4] and text[i+5] == ' ':
                index_first = i+6
            elif text[i] == ' ' and text[i+1] == target_last[0] and text[i+2] == target_last[1] and text[i+3] == target_last[2] and text[i+4] == target_last[3] and text[i+5] == target_last[4]:
                if index_first != 0:
                    index_last = i-1
            if index_first != 0 and index_last != 0:
                return text[index_first:index_last+1]
    return 'cannot extract'
```

1.  

```python
def primeAt(n):
    num = 2
    list_prime = []
    while len(list_prime) != n:
        for i in range(2,(num//2)+1):
            if (num % i) == 0:  
                break
        else:
            list_prime.append(num)
        num += 1
    return list_prime[n-1]
```
