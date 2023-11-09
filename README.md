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

## Dictionaries 

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


## Akses Elemen List, Tuple, Set, Dictionaries

### List:
1. **Mengakses Elemen**:
   - Untuk mengakses elemen berdasarkan indeks, gunakan `list[index]`.

Contoh:
```python
my_list = [1, 2, 3, 4, 5]
print(my_list[2])  # Output: 3
```

2. **Menambah Elemen**:
   - Untuk menambahkan elemen ke akhir list, gunakan `append()`.
   - Untuk menyisipkan elemen di indeks tertentu, gunakan `insert(index, element)`.

Contoh:
```python
my_list = [1, 2, 3]
my_list.append(4)    # Menambahkan 4 ke akhir list
my_list.insert(1, 5)  # Menyisipkan 5 di indeks 1
print(my_list)  # Output: [1, 5, 2, 3, 4]
```

3. **Menghapus Elemen**:
   - Untuk menghapus elemen berdasarkan nilai, gunakan `remove(value)`.
   - Untuk menghapus elemen berdasarkan indeks, gunakan `pop(index)`.

Contoh:
```python
my_list = [1, 2, 3, 4, 3]
my_list.remove(3)  # Menghapus nilai 3 pertama yang ditemukan
my_list.pop(1)     # Menghapus elemen di indeks 1
print(my_list)  # Output: [1, 4, 3]
```

4. **Menggabungkan List**:
   - Untuk menggabungkan dua list, gunakan operator `+` atau `extend()`.

Contoh:
```python
list1 = [1, 2, 3]
list2 = [4, 5, 6]
combined_list = list1 + list2  # Menggabungkan list1 dan list2
print(combined_list)  # Output: [1, 2, 3, 4, 5, 6]
```

### Tuple:
Operasi pada tuple serupa dengan list, tetapi elemen-elemen dalam tuple tidak dapat diubah setelah pembuatan.

### Set:
1. **Mengakses Elemen**:
   - Karena set tidak memiliki indeks, Anda dapat menggunakan loop atau mengonversinya ke list untuk mengakses elemen.

Contoh:
```python
my_set = {1, 2, 3}
for element in my_set:
    print(element)

# Mengonversi set ke list untuk mengakses elemen
my_list = list(my_set)
print(my_list[1])  # Output: 2
```

2. **Menambah Elemen**:
   - Untuk menambah elemen ke set, gunakan `add(element)`.

Contoh:
```python
my_set = {1, 2, 3}
my_set.add(4)  # Menambahkan 4 ke set
print(my_set)  # Output: {1, 2, 3, 4}
```

3. **Menghapus Elemen**:
   - Untuk menghapus elemen, gunakan `remove(value)` atau `discard(value)`. Perbedaannya adalah `remove()` akan menimbulkan KeyError jika elemen tidak ada, sedangkan `discard()` tidak akan menimbulkan error.

Contoh:
```python
my_set = {1, 2, 3}
my_set.remove(2)  # Menghapus nilai 2
my_set.discard(4)  # Tidak akan menimbulkan error karena 4 tidak ada dalam set
```

### Dictionary:
1. **Mengakses Elemen**:
   - Untuk mengakses nilai berdasarkan kunci, gunakan `dict[key]`.

Contoh:
```python
my_dict = {'nama': 'John', 'usia': 30}
print(my_dict['nama'])  # Output: 'John'
```

2. **Menambah Elemen**:
   - Untuk menambah pasangan kunci-nilai, gunakan `dict[key] = value`.

Contoh:
```python
my_dict = {'nama': 'John', 'usia': 30}
my_dict['kota'] = 'Jakarta'  # Menambah pasangan kunci-nilai baru
print(my_dict)  # Output: {'nama': 'John', 'usia': 30, 'kota': 'Jakarta'}
```

3. **Menghapus Elemen**:
   - Untuk menghapus pasangan kunci-nilai, gunakan `del dict[key]`.
   - Untuk menghapus semua elemen dalam dictionary, gunakan `clear()`.

Contoh:
```python
my_dict = {'nama': 'John', 'usia': 30}
del my_dict['usia']  # Menghapus pasangan kunci-nilai 'usia'
my_dict.clear()     # Menghapus semua elemen dalam dictionary
```

Demikianlah beberapa operasi umum pada list, tuple, set, dan dictionary beserta contoh-contohnya. Semoga ini membantu Anda memahami cara menggunakan dan memanipulasi struktur data tersebut dalam Python.

<br>
<br>
<br>



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
