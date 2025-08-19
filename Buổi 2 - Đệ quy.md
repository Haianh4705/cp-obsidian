# 📅 19/08/2025
# 📚 Ghi chú

> **Đệ quy là hàm gọi lại chính nó**

2 bài toán sử dụng đệ quy:
- Chia để trị (tính lũy thừa)
- Quay lui (sinh xâu nhị phân)
### VD tính lũy thừa:
```cpp
int binpow(int a, int n) {
	if (n == 0) return 1;
	int tmp = binpow(a, n/2);
	tmp = tmp * tmp;
	if (n%2) tmp = tmp * a;
	return tmp;
}
```

### VD sinh xâu nhị phân:
```cpp
int n = 20, a[n+1];
void backtrack(int i) {
	if (i == n+1) {
		...
		return;
	}
	a[i] = 0;
	backtrack(i+1);
	a[i] = 1;
	backtrack(i+1);
}
```

> **Lưu ý: ** Nên đặt điều kiện dừng tại đầu hàm đệ quy
# 🔗 Link liên quan

