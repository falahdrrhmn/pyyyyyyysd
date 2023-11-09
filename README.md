# Python Collections

- List
- Tuple
- Set
- Dictionaries

## List 

```py
my_list = [1, 2, 3, 'a', 'b', 'c']
```

List adalah koleksi data yang dapat diubah (mutable) dan diurut. Ini berarti elemen-elemennya dapat dimodifikasi setelah pembuatan. Dapat berisi berbagai jenis data dan memungkinkan duplikasi.


## Tuple 

```py
my_tuple = (1, 2, 3, 'a', 'b', 'c')
```

Tuple adalah koleksi data yang tidak dapat diubah (immutable) dan diurut. Elemen-elemennya tidak dapat diubah setelah pembuatan tuple. Dapat berisi berbagai jenis data dan memungkinkan duplikasi.



## Set

```py
my_set = {1, 2, 3, 'a', 'b', 'c'}
```

Set adalah kumpulan data yang tidak diurut dan tidak mengizinkan duplikasi. Elemen-elemennya tidak memiliki indeks dan urutannya bisa berubah.



## Dict 

```py
my_dict = {
                'nama': 'John',
                'usia': 30,
                'kota': 'Jakarta'
            }
```

Dictionary adalah koleksi data yang diurut (mulai dari Python 3.7) dan dapat diubah. Setiap elemen dalam dictionary terdiri dari pasangan kunci-nilai (key-value pair). Kunci harus unik dan nilai bisa berupa objek apa pun.



## Perbedaan

- List memungkinkan perubahan nilai elemen, dapat diurut, dan memungkinkan duplikasi.
- Tuple bersifat immutable (tidak dapat diubah setelah dibuat), dapat diurut, dan memungkinkan duplikasi.
- Set tidak memiliki urutan (tidak diindeks), tidak mengizinkan duplikasi, dan digunakan untuk operasi matematika set.
- Dictionary terdiri dari pasangan kunci-nilai, kunci unik, dan dapat diubah (mulai dari Python 3.7, dictionary dianggap terurut).

# Python Data Structure

## Recursion

```py
# Recursion 
# example 
# 5! = 5 * 4 * 3 * 2 * 1

def recursion(nilai):
    if nilai == 0 or nilai == 1:
        return 1
    else:
        return nilai * recursion(nilai - 1)
   
print(recursion(5))
```
