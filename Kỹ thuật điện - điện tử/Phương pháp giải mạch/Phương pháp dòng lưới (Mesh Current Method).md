Đây là phương pháp dựa vào định luật Kirchoff 2.
Phương pháp này chỉ áp dụng được với mạch phẳng (planar circuit). Loại mạch có thể vẽ được trên một mặt phẳng mà không có phần tử hoặc dây nối nào cắt nhau.
# Phương pháp xác định
1. Xác định các mắt lưới.
2. Chọn tùy ý một chiều cố định cho mắt lưới (cùng chiều hay ngược chiều kim đồng hồ). Suy ra điện áp trên mỗi phần tử tương ứng với dòng nhánh^[Dòng qua từng phần tử] đã chọn. 
3. Áp dụng định luật Kirchoff 2 cho từng mắt lưới và giải hệ phương trình thu được.^[Số phương trình bằng số mắt lưới]
# Dạng chính tắc
Trường hợp tổng quát khi mạch có n mắt lưới. Trong mạch chỉ có nguồn áp và điện trở.
1. Xác định số mắt lưới và đánh số từ 1 tới n. 
2. Gọi $i_1, i_2, i_3 ... i_n$ là dòng lưới tương ứng với các lưới^[Quy ước mắt thứ k có dòng $i_k$]. Các dòng điện này được chọn theo cùng hướng là cùng chiều kim đồng hồ.
3. Viết hệ phương trình tuyến tính có n ẩn số $i_1, i_2, i_3 ... i_n$ theo dạng chính tắc.
$$
\left\{
\begin{align*}
	+ R_{11}i_1 - R_{12}i_2 - R_{13}i_3 \, ... - R_{1n}i_n &= V_1 \\
	- R_{21}i_1 + R_{22}i_2 - R_{23}i_3 \, ... - R_{2n}i_n &= V_2 \\
	- R_{31}i_1 - R_{32}i_2 + R_{33}i_3 \, ... - R_{3n}i_n &= V_3 \\
	... \\
	- R_{n1}i_1 - R_{n2}i_2 - R_{n3}i_3 \, ... + R_{nn}i_n &= V_n
\end{align*}
\right.
$$
Trong đó:
$R_{ij}$ là tổng điện trở chung của mắt lưới i và mắt lưới j.
$V_{k}$ là tổng đại số của các điện áp trong mắt lưới k theo hướng của $i_k$.
%%
**Khi dùng môi trường {array}**
@{command} xác định số khoảng trống trước và sau một cột. Ví dụ: @{} sẽ làm khoảng trống biến mất, @{bar} sẽ thay khoảng trống bằng chữ 'bar'.
!{command} định dạng đường ngăn cách trong bảng. Ví dụ: !{foo} thay đường kẻ dọc bằng foo.
%%