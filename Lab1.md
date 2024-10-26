1. Phân tích kiến trúc.
1.1. Phân tích yêu cầu.
    - Tính năng:
        + Ghi nhận thẻ chấm công điện tử.
        + Tính toán lương tự động dựa trên giờ làm, doanh số và loại hình hợp đồng.
        + Quản lý thông tin nhân viên (thêm, xóa, cập nhật).
        + Quản lý các phương thức thanh toán đa dạng.
        + Tạo báo cáo chi tiết cho nhân viên và quản lý.
        + Tích hợp với cơ sở dữ liệu quản lý dự án hiện có (DB2).

    - Yêu cầu kỹ thuật: 
        + Giao diện người dùng thân thiện, dễ sử dụng
        + Bảo mật thông tin nhân viên
        + Tính ổn định, độ tin cậy cao
        + Tự động hóa quy trình tính lương
        + Khả năng mở rộng để đáp ứng nhu cầu tăng trưởng của công ty  
        
1.2. Đề xuất kiến trúc hệ thống.
    - Đề xuất kiến trúc 3 lớp(three-layer):
        + Presentation Layer: Cung cấp giao diện cho nhân viên nhập liệu, quản lý và xem báo cáo.
        + Business Logic Layer: Xử lý các quy tắc kinh doanh, tính toán lương, xác thực dữ liệu, tương tác với cơ sở dữ liệu.
        + Data Access Layer: Truy xuất, cập nhật dữ liệu từ các cơ sở dữ liệu.
    
    - Giải thích lý do lựa chọn:
        + Đáp ứng yêu cầu: Kiến trúc này đáp ứng đầy đủ các yêu cầu về tính năng, hiệu suất và bảo mật của hệ thống bảng lương.
        + Tính linh hoạt: Dễ dàng mở rộng và tùy chỉnh để đáp ứng các yêu cầu mới.
        + Tính hiệu quả: Tối ưu hóa việc sử dụng tài nguyên hệ thống và giảm thiểu chi phí.
        + Tính bảo mật: Bảo vệ thông tin nhạy cảm của nhân viên.
        + Tích hợp hệ thống: Dễ dàng tích hợp với các hệ thống khác như hệ thống kế toán.

    - Biểu đồ package mô tả kiến trúc:
        ![Package](https://www.planttext.com/api/plantuml/png/T591RW8n3Bpd5L7kNFg02YWjgWHIoweFi8m5KRF9okiWBQWlwu4dyOMci8Ymk-Je6S-CxPn-Z-DQW2MMJbM0tx0XRRxUZJuedHuwg6jjbc2zVWjSchpwMbOkD4HzP4LLO6dhF-gcF8srzPGeYx2ns77vW8Q3So_WC3gGm8DkI_19YWVyvkI9Btsvvmm4z0GnsNOCYyz5GRmZ_gUqZ1oVJPzo91SjS4lhw5AEmHbky7qNOMGhJQTf4cLBNYo2sE1D5mfizosInCxN6OsUUyjKlUsUMVdu3oXPsWU4Qsur9hzEV-KF003__mC0)

2. Cơ chế phân tích.
2.1. Quản lý thông tin nhân viên:
    - Để đảm bảo rằng tất cả thông tin nhân viên luôn chính xác và cập nhật, từ đó đảm bảo thanh toán đúng đắn và theo quy định.
    - Đề xuất cơ chế:
        + Transaction management: Đảm bảo các giao dịch liên quan đến thông tin nhân viên được thực hiện một cách chính xác và an toàn.

2.2. Tính toán Lương:
    - Tính toán lương cho nhân viên dựa trên loại hình (theo giờ, cố định, hoa hồng), bao gồm cả giờ làm thêm.
    - Đề xuất cơ chế:
        + Transaction management: Đảm bảo các giao dịch liên quan đến lương được thực hiện một cách chính xác và an toàn.

2.3. Báo cáo: 
    - Cung cấp các báo cáo cho nhân viên như số giờ làm việc, tổng số tiền lương, thời gian nghỉ phép còn lại.
    - Đề xuất cơ chế:
        + Error detection / handling / reporting: Cung cấp các cơ chế để phát hiện lỗi trong hệ thống và báo cáo cho người quản lý, 
                                                    để kịp thời xử lý các vấn đề, đảm bảo tính chính xác và tin cậy của hệ thống.

2.4. Bảo mật: 
    - Cung cấp sự bảo mật cho thông tin của hệ thống.
    - Đề xuất cơ chế:
        + Security: Cơ chế bảo mật giúp hệ thống bảo vệ thông tin người dùng, thông tin giao dịch của người dùng.

2.5. Tích hợp với cơ sở dữ liệu hiện có:
    - Hệ thống mới cần truy cập thông tin từ Cơ sở Dữ liệu Quản lý Dự án mà không cần thay thế.
    - Đề xuất cơ chế:
        + Legacy Interface: Cung cấp khả năng tích hợp và tương tác với các hệ thống cũ mà không cần phải thay thế hoàn toàn.

3. Phân tích ca sử dụng Payment.
3.1. Xác định các lớp phân tích.
    - Boundary:  
        + Select Payment Method Form.
    - Control: 
        + Payment Method Control.
    - Entity: 
        + Employee

3.2. Sequence Diagram.
    ![Sequence Diagram](https://www.planttext.com/api/plantuml/png/Z9EzJiCm4CTtFyKf4qZm0XrGfLAOg11z0YSv6gl-IEspK6O69WRU08cv4gpDq074U_W9U0MID07rWnOFaPNxtTt_VxQ_ocNV4RVabMGy8MDXg79f2aGM6wzJRWk8nYWn8RZcXK9DS8MKcHGkZ5KHSDTiM68qMICXsg06g_yDsEuPwth0wLcJtOCRd7bq16J0hRhbRHtLr64rLkDjZHwS2vTBNcnmO78IHZlMShyTnfcvww9m58soi9Xh81lAjmH8XCKoZquWkWpbNC3CSuW_NpryF8bGFkWwCiXy4Sfx3TFCXCNBPkxn3bVZ_raP6HAtHMiSquvZN18Cib0-QkZqPk_FUX8nXjBXJ-mFpGogjJM7RjAA2odq17YQMdIkWJjbdPCU33MXtSdkSEjZ9ROBhqazCCJzacEkfw2vGk0w1PuarGqbq5x5QFVgRn9Jf4hP0V5h9Ehg4FhLjtuTtm000F__0m00)

3.3. Class Diagram. 
    ![Class Diagram](https://www.planttext.com/api/plantuml/png/T5DBRi8m4Dtd55u6gLm0HH6bi2ke4bBtGpm2g_wazWGfgdg4dgAhNg6ewg8duGIzGWr9J0pK6zipp_FUFDk_k--n8x1KAPaK4fnZCrLAKoEoB9jf4bJd-Kl23aDeOe8twoLPeTTCWy8eK4AjKDCSQMDYg08X_NpBkKNdejGAzDFYl18KXQaqBIgrGjjajaPmLfKS21_wF6b7STmDUc27D8zuEoWqspFin0kP8laJ0TXfkxcgQv2y9grlaI9ltiIZEDYJVP78YtOvkiAAaeJHKNoDD3sbqbRmoXY9e9bmZo05lsv3aBQi7Q7ockwC9cjaa7Gl76NTXUSCsvNhPQEsylX-NSyzRsXNA0rFg2lOjzcYCbiCsEPH3Vvdz0P44PSUEmiSms5-vls85PlzxaspF6axFs32WH5xhlQVxvh9dwyOSgtC1tZC63K__90_0000__y30000)

4. Phân tích ca sử dụng Maintain Timecard.
4.1. Xác định các lớp phân tích.
    - Boundary:  
        + Payroll Form
        + Employee Form
    - Control: 
        + System    
    - Entity: 
        + Employee
        + Payroll
4.2. Sequence Diagram.
    ![Sequence Diagram](https://www.planttext.com/api/plantuml/png/T5DBRi8m4Dtd55u6gLm0HH6bi2ke4bBtGpm2g_wazWGfgdg4dgAhNg6ewg8duGIzGWr9J0pK6zipp_FUFDk_k--n8x1KAPaK4fnZCrLAKoEoB9jf4bJd-Kl23aDeOe8twoLPeTTCWy8eK4AjKDCSQMDYg08X_NpBkKNdejGAzDFYl18KXQaqBIgrGjjajaPmLfKS21_wF6b7STmDUc27D8zuEoWqspFin0kP8laJ0TXfkxcgQv2y9grlaI9ltiIZEDYJVP78YtOvkiAAaeJHKNoDD3sbqbRmoXY9e9bmZo05lsv3aBQi7Q7ockwC9cjaa7Gl76NTXUSCsvNhPQEsylX-NSyzRsXNA0rFg2lOjzcYCbiCsEPH3Vvdz0P44PSUEmiSms5-vls85PlzxaspF6axFs32WH5xhlQVxvh9dwyOSgtC1tZC63K__90_0000__y30000)
4.3. Class Diagram. 
    ![Class Diagram](https://www.planttext.com/api/plantuml/png/T5DBRi8m4Dtd55u6gLm0HH6bi2ke4bBtGpm2g_wazWGfgdg4dgAhNg6ewg8duGIzGWr9J0pK6zipp_FUFDk_k--n8x1KAPaK4fnZCrLAKoEoB9jf4bJd-Kl23aDeOe8twoLPeTTCWy8eK4AjKDCSQMDYg08X_NpBkKNdejGAzDFYl18KXQaqBIgrGjjajaPmLfKS21_wF6b7STmDUc27D8zuEoWqspFin0kP8laJ0TXfkxcgQv2y9grlaI9ltiIZEDYJVP78YtOvkiAAaeJHKNoDD3sbqbRmoXY9e9bmZo05lsv3aBQi7Q7ockwC9cjaa7Gl76NTXUSCsvNhPQEsylX-NSyzRsXNA0rFg2lOjzcYCbiCsEPH3Vvdz0P44PSUEmiSms5-vls85PlzxaspF6axFs32WH5xhlQVxvh9dwyOSgtC1tZC63K__90_0000__y30000)