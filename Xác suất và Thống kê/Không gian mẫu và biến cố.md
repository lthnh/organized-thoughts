# Định nghĩa
**Phép thử** (*Random experiment*) là một thí nghiệm có thể dẫn đến nhiều kết quả khác nhau. Dù chúng được lặp lại nhiều lần trong cùng điều kiện.

Mỗi kết quả của phép thử ngẫu nhiên được gọi là một **biến cố sơ cấp** (*simple event*). Kí hiệu là $\omega$. ^56b8b6

**Không gian mẫu** (*Sample space*) hay không gian các biến cố sơ cấp là tập hợp tất cả các khả năng có thể xảy ra của phép thử. Kí hiệu là $\Omega$.
Nó có thể mang tính rời rạc (*discrete*) hoặc tính liên tục (*continuous*). Nó mang tính rời rạc khi nó gồm một số hữu hạn (hoặc vô hạn nhưng đếm được) tập. 

**Biến cố** (*Event*) là tập con của không gian mẫu của một phép thử.

## Quan hệ giữa các biến cố
### Sự kéo theo
A kéo theo B, kí hiệu là $A \subset B$. Nếu A xảy ra thì B xảy ra. Ta nói A là biến cố thuận lợi cho B

### Sự tương đương
A tương đương tới B, kí hiệu là $A = B$. Nếu A xảy ra thì B xảy ra và ngược lại.

## Phép toán trên biến cố
- **Tổng** (*Union*): Tất cả các khả năng của hai biến cố.
	- Kí hiệu: $A\cup B$ or $A+B$
- **Hiệu** (*Difference*): Khả năng chỉ có ở một biến cố.
	- Kí hiệu: $A\setminus B$
- **Giao** (*Intersection*): Khả năng có ở cả hai biến cố.
	- Kí hiệu: $A \cap B$ or $A.B$
- **Bù** (*Complement*) của một biến cố: Khả năng có ở trong không gian mẫu nhưng không có ở biến cố đó.
	- Kí hiệu: $\bar{A}$
	- Để là phần bù của $A$, $\bar{A}$ cần phải thỏa mãn điều kiện sau: 

$$
\begin{cases}
A \cup \bar{A} = \Omega \\
A \cap \bar{A} = \emptyset \end{cases}
\quad or \quad
\bar{A} = \Omega \setminus A
$$

Nếu **giao** của hai biến cố đó là rỗng thì hai biến cố đó xung khắc nhau (*mutually exclusive*) ^fb75a9

Đây cũng là các phép toán trên xác suất.

[[Định lý De Morgan (De Morgan's Laws)]]
[[Xác suất]]