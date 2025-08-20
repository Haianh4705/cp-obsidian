# 📅 19/08/2025
# 📚 Ghi chú

Số nguyên tố là số >= 2 chỉ có ước là 1 và chính nó

Ước chung lớn nhất của a và b là số lớn nhất là ước của a và b: $(a, b) = g$

Thuật toán Euclid: $(a, b) = (a\%b, b)$

Công thức đếm ước:
$$
N = p_1^{a_1} \times p_2^{a_2} \times ... \times p_k^{a_k}
\Rightarrow d(N) = (a_1+1) \times (a_2+1) \times ... \times (a_k+1)
$$
Sàng số nguyên tố:
```cpp
int d[n];
d[0] = d[1] = 1;
for (int i = 2; i*i<n; i++) if (!d[i])
	for (int j = i*i; j<n; j+=i)
		d[j] = 1;
```
Euclid mở rộng:
Tìm cặp $x, y$ thỏa mãn:
$$
a \times x + b \times y = (a, b)
$$
```cpp
int x, y, cnt = 0;
void ext_euclid(int a, int b) {
	if (b == 0) {
		cnt++;
		return;
	}
	ext_euclid(b, a%b);
	cnt++;
	x[cnt] = y[cnt-1];
	y[cnt] = x[cnt-1] - y[cnt-1] * (a/b);
}
```
# 🔗 Link liên quan

