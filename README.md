<p align="center">
  <a href="https://hcmus.edu.vn//" title="Trường Đại học Khoa Học Tự Nhiên " style="border: none;">
    <img src="https://fetel.hcmus.edu.vn/wp-content/uploads/2022/09/logo-fetel.png" alt="rường Đại học Khoa Học Tự Nhiên | University of Science">
  </a>
</p>

# Thiết kế mạch Analog Two-Stage Opamp trên công nghệ 90nm

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/circuit.png)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/gain.png)

## Giới thiệu

* Đây là bài tập được sử dụng làm đồ án cuối kì cho môn Thiết kế vi mạch .
* Bài tập được xây dựng trên phần mềm Synopsys Custom Compiler , sử dụng công nghệ 90nm.
* Thiết kế mạch Two-Stage Opamp theo spec yêu cầu cụ thể .
* Thiết kế full flow custom IC design (schematic - simulation - layout - check DRC,LVS)
### Giảng viên hướng dẫn

* ThS. Nguyễn Thị Thiên Trang- Khoa Điện Tử - Viễn Thông , Trường Đại Học Khoa Học Tự Nhiên - ĐHQGHCM

### Sinh viên thực hiện

|**STT**|**MSSV**|  **Họ và tên**  |       **Email**      |
|-------|--------|-----------------|----------------------|
|   1   |21207077|Tran Thien Phuc  |21207077@hcmus.edu.vn |

## Chạy thử project

### Yêu cầu để thực thi project

* Synopsys Custom Compiler

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/custom_compiler.png)


* Thiết kế theo spec đã đưa ra  

### Bước 1: Thực hiện theo flow . Xử lí spec và tính W/L    

* Phân tích mạch current mirror sử dụng chức năng của Diode-Connected
  
![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/current.png)
  
* Đưa NMOS và PMOS về vùng sat ( region 2 )
  
![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/diode.png)

* Khảo sát operating point đưa ra được các thông số cần thiết để tính W/L của từng stage
  
![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/OP.png)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/op1.png)


* Sau khi có được các thông số bắt đầu tính toán theo yêu cầu của spec 

### Bước 2: Vẽ schematic . sympol 

* Sau khi có được các W/L cần thiết tiến hành vẽ schematic và sympol

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/schematic.jpg)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/symbol.jpg)

### Bước 3 : Tiến hành lập các testbench để mô phỏng AC , trans 
* Testbench mô phỏng AC

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/testbench_ac.jpg)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/ac.jpg)

* Testbench mô phỏng trans

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/testbench_trans.jpg)

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/trans.jpg)

* Sau khi mô phỏng dạng sóng ở mode AC và trans thấy được :
- Ở mode AC tần số và độ lợi thi theo mức mong muốn gần đúng với spec
- Ở mode Trans tín hiệu đã khuếch đại ra ở Vout

### Bước 4 : Vẽ layout , check DRC LVS 

* Hình ảnh layout 

![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/layout.jpg)

* Check DRC
  
![Alt text](https://raw.githubusercontent.com/tthphuc1810/twostageopamp/master/pic/drccheck.png)
