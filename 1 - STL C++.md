# 📅 19/08/2025
# 📚 Ghi chú

Dữ liệu trong máy tính lưu dưới dạng nhị phân (dãy số 01)
Mỗi ô nhớ là 1 bit, 8 bit = 1 byte, máy tính tổ chức dữ liệu theo byte
Kiểu dữ liệu int có 4 byte = 32 bit -> int có thể biểu diễn $2^{32}$ giá trị khác nhau

Con trỏ là biến lưu địa chỉ của biến khác được biểu diễn dưới dạng hexa
Khai báo và lấy giá trị con trỏ
```cpp
int a = 2025;
int *p = &a;
cout << p; // giá trị CỦA con trỏ
cout << (*p); // giá trị TẠI con trỏ
```

Biến gồm 2 loại: Toàn cục và cục bộ
- Toàn cục: Lưu tại heap và có giá trị mặc định 
- Cục bộ: Lưu tại stack và không có giá trị mặc định

Mảng là tập hợp các biến có cùng kiểu dữ liệu có địa chỉ liên tiếp
Địa chỉ của mảng là tên mảng và = địa chỉ của biến đầu tiên trong mảng

STL (Standard Template Library) là thư viện các CTDL và thuật toán phổ biến
STL bao gồm: pair, vector, set, map, stack, queue, ...
Xem thêm về các CTDL trên qua 2 trang dưới
# 🔗 Link liên quan

https://cplusplus.com/
https://en.cppreference.com/