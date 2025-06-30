# 🧠 42 Piscine - C String Functions

Bu repoda, 42 okulunun *piscine* döneminde C diliyle geliştirilen bazı temel string fonksiyonlarının kendi implementasyonları yer almaktadır. Bu alıştırmalar sayesinde, C dilinde diziler, karakter işlemleri ve göstericiler (pointers) gibi temel kavramlarda derinlemesine pratik yapılmıştır.

## 🔧 Fonksiyonlar

### 1. `ft_strncpy`
```c
char *ft_strncpy(char *dest, char *src, unsigned int n);
```
- `strncpy` fonksiyonunun birebir karşılığıdır.
- `src` dizisinden `n` karakter kopyalar.
- Eğer `src` daha kısa ise kalan alanları `'\0'` ile doldurur.

---

### 2. `ft_str_is_alpha`
```c
int ft_str_is_alpha(char *str);
```
- Verilen string yalnızca harf içeriyorsa `1` döner.
- Aksi halde `0` döner.
- Boş string geçerli kabul edilir ve `1` döner.

---

### 3. `ft_str_is_numeric`
```c
int ft_str_is_numeric(char *str);
```
- String yalnızca sayısal karakterlerden oluşuyorsa `1`, aksi halde `0` döner.

---

### 4. `ft_str_is_lowercase`
```c
int ft_str_is_lowercase(char *str);
```
- Tüm karakterler küçük harfse `1`, değilse `0`.

---

### 5. `ft_str_is_uppercase`
```c
int ft_str_is_uppercase(char *str);
```
- Tüm karakterler büyük harfse `1`, değilse `0`.

---

### 6. `ft_str_is_printable`
```c
int ft_str_is_printable(char *str);
```
- Karakterler yazdırılabilir ASCII karakterlerse (32-126 arası) `1`, aksi halde `0`.

---

### 7. `ft_strupcase`
```c
char *ft_strupcase(char *str);
```
- Tüm küçük harfleri büyük harfe dönüştürür.
- Orijinal string üzerinde değişiklik yapar.

---

### 8. `ft_strlowcase`
```c
char *ft_strlowcase(char *str);
```
- Tüm büyük harfleri küçük harfe çevirir.

---

## 📌 Amaç

Bu projede amaç, standart kütüphane fonksiyonlarının nasıl çalıştığını anlamak ve kendi versiyonlarını sıfırdan yazarak pointer işlemlerine hakimiyet kazanmaktır.

## 🛠️ Derleme

Tüm dosyaları tek bir `.c` dosyasına ekleyerek GCC ile derleyebilirsiniz:

```bash
gcc -Wall -Wextra -Werror main.c ft_str*.c -o string_tests
./string_tests
```

> `main.c` test dosyanız olmalıdır. Her fonksiyonu ayrı ayrı test etmeniz önerilir.

## 👩‍💻 Geliştirici

**Sude İlhan**  
[GitHub Profili](https://github.com/sudeilhn)

---

## 📄 Lisans

Bu proje eğitim amaçlıdır. 42 Network / Piscine kapsamında hazırlanmıştır.
