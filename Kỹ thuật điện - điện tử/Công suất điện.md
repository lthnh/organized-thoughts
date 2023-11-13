# Định nghĩa
Là công mà mạch điện thực hiện trong một đơn vị thời gian. Đơn vị của công là watt (W).
# Trong AC
## Năng lượng tức thời (Instantaneous power)
$$
p(t) = v(t)i(t)
$$
## Năng lượng trung bình (Average power)
Là độ lớn trung bình của năng lượng tức thời trong một chu kì.
$$
P = \frac{1}{2} \mathrm{Re}[\mathbf{VI*}] = \frac{1}{2} V_m I_m \cos(\theta_v-\theta_i)
$$
Tải điện trở (resistive load - R) thì luôn luôn hấp thụ năng lượng còn tải phản kháng (reactive load - L hoặc C) thì có năng lượng trung bình bằng không.
## Năng lượng biểu kiến (Apparent power)
$$
P = V_{rms} I_{rms} \cos(\theta_v - \theta_i) = S \cos(\theta_v - \theta_i)
$$
Trong đó S là năng lượng biểu kiến. Đơn vị là VA.
$$
S = V_{rms} I_{rms}
$$
### Hệ số công suất
$$
\mathrm{pf} = \frac{P}{S} = \cos(\theta_v - \theta_i)
$$
Góc $\theta_v - \theta_i$ được gọi là góc hệ số công suất (power factor angle)
Còn có thể tính hệ số góc theo điện trở
$$
\mathrm{pf} = \frac{R}{Z}
$$
Trong đó $Z$ là tổng trở.
## Năng lượng phức (Complex power)
$$
\boldsymbol{\mathrm{S}} = \frac{1}{2} \mathbf{VI*} 
= \mathbf{V_{rms} I^*_{rms}}
= V_{rms} I_{rms} \angle \, (\theta_v - \theta_i)
$$
Thay $\boldsymbol{\mathrm{V_{rms}}} = \mathbf{Z I_{rms}}$ vào, ta được
$$
\boldsymbol{\mathrm{S}} = I^2_{rms} \boldsymbol{\mathrm{Z}} = \frac{V^2_{rms}}{\boldsymbol{\mathrm{Z^*}}}  
$$
==**Lưu ý:** Số phức được viết in đậm và không in nghiêng.==

Lại có $\boldsymbol{\mathrm{Z}} = R + jX$,  năng lượng phức trở thành
$$
\displaylines{
\boldsymbol{\mathrm{S}} = I^2_{rms}(R+jX) = P + jQ \\
P = \mathrm{Re}(\boldsymbol{\mathrm{S}}) = I^2_{rms}R \\
Q = \mathrm{Im}(\boldsymbol{\mathrm{S}}) = I^2_{rms}X
}
$$
Trong đó $P$ là năng lượng trung bình (hay năng lượng thật - real power) và nó phụ thuộc vào tính trở $R$ của tải. $Q$ phụ thuộc vào tính phản kháng $X$ của tải và được gọi là công suất phản kháng.

==**Lưu ý:** $P$ là phần năng lượng có ích duy nhất.== $Q$ là phần năng lượng do phần tử điện cảm và tụ điện trao đổi với mạch. Ở điều kiện lý tưởng hai phần tử này không phát năng lượng ra bên ngoài nên chúng không có ích.

Từ nhận định trên ta thấy
$$
\displaylines{
P = V_{rms} I_{rms} \cos(\theta_v - \theta_i) \\
Q = V_{rms} I_{rms} \sin(\theta_v - \theta_i)
}
$$
Thành phần $P$ mang đơn vị watt. Còn thành phần $Q$ mang đơn vị volt-ampere reactive (VAR) để phân biệt với thành phần $P$.

**Nhận xét**:
- $Q$ = 0 nếu tải mang tính trở (unity pf - điện áp và dòng điện cùng pha)
- $Q$ < 0 nếu tải mang tính dung (leading pf - dòng điện nhanh pha hơn điện áp)
- $Q$ > 0 nếu tải mang tính cảm (lagging pf - dòng điện chậm pha hơn điện áp)

## Bảo toàn năng lượng (Conservation of AC power)
Dù tải được đấu trực tiếp hay song song, tổng năng lượng được cung cấp bởi nguồn bằng tổng năng lượng được đưa tới tải
$$
\boldsymbol{\mathrm{S}} = \sum_{i=1}^n \boldsymbol{\mathrm{S}}_i
$$
## Điều chỉnh hệ số công suất (Power factor correction)
Là quá trình điều chỉnh hệ số công suất sao cho độ lệch pha của điện áp và dòng điện càng nhỏ *(make power factor closer to unity)* mà không thay đổi điện áp hay cường độ dòng điện qua mạch. Do đó cách để điều chỉnh hệ số công suất đó chính là thêm các phần tử phản kháng (L hoặc C)
Mục đích của quá trình này là tăng năng lượng có ích.

[[Nguyên tắc dấu thụ động (Passive sign convention)]]