# Python Temel Eğitimi Proje Ödevi 
>**[patika.dev](https://app.patika.dev/courses/python-temel/proje) platformu bitirme projesidir.**
Profil için tıklayınız: [app.patika.dev/nmelihkutlu](https://app.patika.dev/nmelihkutlu)

## Soru

![](https://raw.githubusercontent.com/nmelihkutlu/python-temel-proje--devi/main/ProjeSoru.png)

```
1- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. Örnek olarak:

input: [[1,'a',['cat'],2],[[[3]],'dog'],4,5]

output: [1,'a','cat',2,3,'dog',4,5]

2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün. Örnek olarak:

input: [[1, 2], [3, 4], [5, 6, 7]]

output: [[[7, 6, 5], [4, 3], [2, 1]]
```


## Cevaplar
1. Flatten Kodu:

    ```
    def flatten(i):
        for x in i:
            if (isinstance(x,list)): x = flatten(x)
            else: o.append(x)
        return o
    
    i = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
    o = []
    o = flatten(i)
    print(o)    
    ```
    
2. Reverse Kodu:
    ```
    def r(i):
        i = i[::-1]
        for x in range(0,len(i)):
            if (isinstance(i[x],list)): i[x] = i[x][::-1]
            o.append(i[x])
        return o
    
    i = [[1, 2], [3, 4], [5, 6, 7,]]
    o = []
    o = r(i)

    print(o)
```
