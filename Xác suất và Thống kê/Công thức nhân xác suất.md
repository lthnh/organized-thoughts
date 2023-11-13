# A, B tùy ý
$$P(AB)=P(A|B)P(B)=P(B|A)P(A)$$
# A1, A2, A3, ... , An
$$P(A_1A_2...A_n)=P(A_1)P(A_2|A_1)P(A_3|A_1A_2)...P(A_n|A_1A_2...A_{n-1})$$
# Sự độc lập giữa các biến cố
Hai biến cố được gọi là độc lập với nhau nếu một trong các điều kiện sau đúng:
$$\displaylines{
P(A|B)=P(A) \\ 
P(B|A)=P(B) \\
P(AB)=P(A)P(B)}
$$

Trường hợp tổng quát có $A_1, A_2, ... , A_n$ độc lập với nhau nếu
$$P(A_{i_1}A_{i_2}...A_{i_k})=P(A_{i_1})P(A_{i_2})...P(A_{i_k})$$
cho mọi tổ hợp chập k của n chương trình con này.

Nếu biến cố $\text{A}$ độc lập với biến cố $\text{B}$ thì biến cố $\text{A}$ cũng độc lập với biến cố $\overline{\text{B}}$.

[[Xác suất điều kiện (Conditional Probability)]]