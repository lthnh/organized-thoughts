# Định nghĩa
Xét từ định nghĩa của xác suất điều kiện, chúng ta có thể viết công thức cho hai biến cố như sau
$$
P(A|B)=\dfrac{P(B|A)P(A)}{P(B)} \quad \text{với} \quad P(B)>0
$$

Từ đó, ta có thể suy ra định lý Bayes (Bayes' Theorem):
Cho $A_i \space (i=1, ..., n)$ là hệ đầy đủ biến cố, $B$ là một biến cố nào đó liên quan tới hệ sao cho $P(B)>0$. Khi đó với mọi $i \space (i=1, ..., n)$
$$
\begin{align}
P(A_i|B)
=\dfrac{P(B|A_i)P(A_i)}{P(B)}
=\dfrac{P(B|A_i)P(A_i)}
	{\sum_{i=1}^n P(B|A_i)P(A_i)}
\quad \text{với} \quad P(B)>0
\end{align}
$$

[[Xác suất điều kiện (Conditional Probability)#Định nghĩa|Xác suất điều kiện]]