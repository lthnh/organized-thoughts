# Khái niệm
Xác suất của biến cố A là một con số đặc trưng cho khả năng xuất hiện của A trong phép thử tương ứng. Kí hiệu là $P(A)$.
# Định nghĩa
## Quan điểm cổ điển
Cho một phép thử có $\large n$ biến cố sơ cấp đồng khả năng, trong đó có $\large m$ biến cố thuận lợi cho A thì xác suất của A là $\dfrac{m}{n}$.
Kí hiệu là $P(A) = \dfrac{|A|}{|\Omega|} = \dfrac{m}{n}$.
## Quan điểm thống kê
Thực hiện phép thử $\large n$ lần thì biến cố A xuất hiện $\large m$ lần. Khi đó $\large m$ là tần số xuất hiện biến cố A trong $\large n$ phép thử. Tỉ số $\dfrac{m}{n}$ được gọi là tần suất xuất hiện biến cố A trong $\large n$ phép thử. 
Kí hiệu là $f_n(A)= \dfrac{m}{n}$.
Khi thực hiện phép thử càng nhiều ($\begin{aligned} n \rightarrow \infty \end{aligned}$), tần suất của biến cố A tiến tới một số xác định. Đó là xác suất của biến cố A.$$P(A) = \lim_{n \to \infty} f_n(A) = \lim_{n \to \infty} \dfrac{m}{n}$$
## Quan điểm hình học
Xét một phép thử có vô hạn biến cố sơ cấp đồng khả năng. Không gian mẫu có vô hạn phần tử và được biểu diễn thành miền hình học $\Omega$. Biến cố $A \cup \Omega$ được biểu diễn thành miền hình học A. Xác suất xảy ra biến cố A là $$P(A) = \dfrac{\text{Độ đo của miền a}}{\text{Độ đo của miền} \space \Omega}$$
# Tiên đề của xác suất
Xác suất là con số được gán cho từng biến cố sơ cấp trong tập những biến cố. Xác suất thỏa điều kiện sau:
- $P(\Omega) = 1$ với $\Omega$ là không gian mẫu
- $0 \leq P(A) \leq 1$ với mọi biến cố A
- Với hai biến cố A và B với $A \cap B = \emptyset$
$$P(A \cap B) = P(A) + P(B)$$

[[Công thức cộng xác suất]]
[[Xác suất điều kiện (Conditional Probability)]]