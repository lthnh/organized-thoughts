Định luật Ohm
$$
v(t) = R i(t)
$$
Công suất tức thời trên điện trở R
$$
	p(t) = v(t)i(t) = Ri^2(t) = \frac{v^2(t)}{R}
$$
Điện dẫn $G$ là nghịch đảo của điện trở. Có đơn vị là Siemens (S). Được kí hiệu là $\mho$.
$$
G = \frac{1}{R}
$$
**Ngắn mạch** là sự kiện mà tại vị trí ngắn mạch điện trở coi như bằng không.
**Hở mạch** là sự kiện mà tại vị trí hở mạch điện trở coi như bằng vô cùng.
# Điện trở tương đương
## Điện trở mắc nối tiếp
![[Điện trở nối tiếp.excalidraw|center]]
$$
\displaylines{
i=i_1=i_2 \\
u=u_1+u_2 \\
R = R_1 + R_2
}
$$
## Điện trở mắc song song
![[Điện trở song song.excalidraw|center]]
$$
\displaylines{
i = i_1 + i_2 \\
u = u_1 = u_2 \\
\frac{1}{R} = \frac{1}{R_1} + \frac{1}{R_2}
}
$$
## Dạng Y - $\Delta$
![[Wye - Delta.excalidraw|center]]
### Từ Y sang $\Delta$
$$
\displaylines{
R_a = R_2 + R_3 + \frac{R_2 R_3}{R_1} \\
R_b = R_1 + R_3 + \frac{R_1 R_3}{R_2} \\
R_c = R_1 + R_2 + \frac{R_1 R_2}{R_3}
}
$$
Trường hợp đặc biệt tải đấu Y cân bằng $R_1 = R_2 = R_3 = R$
$$
R_a = R_b = R_c = 3R
$$
### Từ $\Delta$ sang Y
$$
\displaylines{
R_1 = \frac{R_b R_c}{R_a + R_b + R_c} \\
R_2 = \frac{R_a R_c}{R_a + R_b + R_c} \\
R_3 = \frac{R_a R_b}{R_a + R_b + R_c}
}
$$
Trường hợp đặc biệt tải đấu $\Delta$ cân bằng $R_a = R_b = R_b = R$
$$
R_1 = R_2 = R_3 = \frac{R}{3}
$$