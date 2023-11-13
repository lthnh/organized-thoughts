## Pixel
- Pixel là đơn vị cơ bản của ảnh
- Mỗi pixel được đặc trưng bởi một hay nhiều con số để diễn tả một màu sắc nhất định
- Xuất phát từ cụm từ PICture ELement
## Độ phân giải (resolution)
- Kích thước của một ảnh được xác định bởi số lượng pixel theo hai chiều ngang dọc
- Độ phân giải của ảnh là số lượng pixel trên một đơn vị dài (pixels per inch - PPI)
- DPI là khái niệm tương tự nhưng cho giấy in (hay số lượng hạt mực trên một inch giấy)
	- Số lượng DPI luôn nhiều hơn hay bằng số lượng PPI
## Mức xám (gray scale)
- Mức xám của một pixel là cường độ sáng của nó
- Có $2^n$ thang xám với n là số bit biểu diễn
- Ảnh nhị phân (binary) là ảnh có hai giá trị 1 (trắng) và 0 (đen)
- Ảnh đen trắng và ảnh có hai màu đen, trắng và các màu xám trung gian
## Dải tần nhạy sáng (dynamic range)
- Hay còn gọi là tỉ lệ tương phản
- Mô tả tỉ lệ giữa cường độ sáng nhất và tối nhất có thể đo được
- Đặc trưng cho thiết bị thu nhận, thiết bị hiện thị và chính bản thân vật $\rightarrow$ mỗi thiết bị có một dải riêng
- Khi chuyển ảnh từ thiết bị này sang thiết bị khác có thể tác động lên thang xám của hình ảnh
## Lược đồ xám (histogram)
- Mô tả số lần xuất hiện của các pixel cùng mức xám tương ứng trên miền ảnh
- Giúp ta xác định ảnh sáng, tối hay bình thường; ảnh có độ tương phản cao hay thấp...
- Nếu ta thấy đồ thị dàn trải trên toàn mức xám ta sẽ thấy độ tương phản cao hơn
## Không gian màu (color space)
Sử dụng lý thuyết màu (color theory).
### RGB
- **Không gian màu RGB**: một màu bất kỳ là tổ hợp tuyến tính của ba màu cơ bản đỏ (R), xanh lá (G) và xanh dương (B)
- Ba trục màu vuông góc với nhau từng đôi một tạo thành không gian màu
- Mỗi pixel được đặc trưng bởi ba giá trị R-G-B (ba kênh màu); mức thang sáng mỗi kênh có $2^n$ giá trị (thông thường từ 0 tới 255 do có 8 bits)
- Là không gian màu cơ bản của ảnh phát xạ
### HSV
 **Không gian màu HSV**: một màu bất kỳ được biểu diễn bởi ba thành phần H (sắc thái), S (độ bão hòa) và V (độ sáng chói).
 Trong đó: 
- H: hue
- S: saturation
- V: value
### CMYK
- **Không gian màu CMYK**: một màu bất kỳ được biểu diễn bởi bốn thành phần C (lục lam), M (đỏ hồng), Y (vàng) và K (đen)
	- Ba trục C, M, Y vuông góc với nhau từng đôi một
	- K biểu diễn độ tối của màu
- Dùng trong in ấn
### RGB vs. CMYK
- RGB là màu mà mắt nhìn thấy trực tiếp từ nguồn sáng
- CMYK là màu mắt mắt nhìn thấy sau khi ánh sáng phản xạ từ vật do nguồn sáng chiếu vào
## Độ sâu màu (color depth)
- Mỗi pixel màu được biểu diễn bằng các kênh màu xác định
- Độ sâu màu là số bits dùng để biểu diễn cường độ màu tại điểm đó
	- (số lượng kênh) $\times$ n bits
	- n bits này dùng để biểu diễn $2^n$ thang xám
## Nhiệt độ màu
Nhiệt độ màu mô tả quang phổ phát ra từ một vật đen tuyệt đối khi bề nó mặt nó đạt một nhiệt độ nhất định.