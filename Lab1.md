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
![Sequence Diagram](https://www.planttext.com/api/plantuml/png/b9DDJiCm48NtFiMeAv3A1Rf0bVZPKLLK761YJubLssFi2IXdOy6Hk09nIoHQ4aYpIppplVV6ay_tZsKMJD9ufr0B9xZpqN5Bf2fkWi7KmeOSQLbZwod80qdDvfwJLvg397PmT79p-AXKpu6hwp720XxffQ4i80nvNmFnK0H-NwL6EWjqI7O1cqZQRjiJ3d0Koo6heQO2wzqkuDRcw70C01VHwXqqSGuUhPk3iQdODXGvMxcSc7ip61QTzAbwMPjXzgquKz0z_mTOCQ0njjX51pPiEqKiRv2wQNTsZIANQKYfH9egqrzTwR7XkMWcoddVFMa6wyIlrj0lm9YvuqcVQxF2i8E0dW230TIwssw1qFYAqlcU_wHHC6h2eZr5Wq90lUxFctgpKeEkELCuNP9bXoz_wnS0003__mC0)



3.3. Class Diagram. 
![Class Diagram]([https://www.planttext.com/api/plantuml/png/f991JWCn34NtEOKlC1SOeQg5WeJKLaYLsBk9eL4JPnHxX2h4oLXm9AxG0AEedROhihFzdF_jvFlpQogAMViOZ0qe0ciAPFK9zv5ObwJRv1vIZl1ke9m6Nahmw5fOQ_RyEYIxOrnQM7ZHcpzYCY1UdZ7uqdYRKY1ays46nHEjkyIQKwXoyck7t0aqKe_eGubcpcKI6HKtoBiLHXgbqThKiwxwkA5SQzNJVUn2sXDL7pGapaRdyxkx_tYTanP4ZYrTUvAckRox5ZmhPRGgyEPrQovIfRjEsKBVELGICoLsFv_X0000__y30000](https://www.planttext.com/api/plantuml/png/f95B2i8m48RtEKKkq0k8Y6yGL8I2-x4PDPX7oKmNHJoP2u_a5OnQgjR7nkpcdp_vlycSZwSkCGGkh16P0IAPei6C5r1QT3n3tderzi7AlP3n978TYubgoPI3TfjAp9_jr99JJTo-EpgLHTCIZ8uN-zuR12SEeafyoHfuny6REevkEAXUJ8rq2zh4ggTKGA96SmLkDmUB3Hcop1UEvuLTOQXxDTF8viQNY3K7LiBRwExzxVmVrY5ojD0pqhUL9Cc3yvVfqmUBBZfrtVe5003__mC0))

4. Phân tích ca sử dụng Maintain Timecard.
4.1. Xác định các lớp phân tích.
    - Boundary:  
        + Submit TimeCard Form
    - Control: 
        + System    
    - Entity: 
        + Employee
        + TimeCard
4.2. Sequence Diagram.
![Sequence Diagram](https://www.planttext.com/api/plantuml/png/X9DDJiCm48NtFiLSe1Ve0XKLsB4XYFtKcJPM7Hl6uvQSZGL7uWfCqeJq9orPH8hopVFpy_FFr_SY2RBasXkq4XaUwtSV6oApYZcKo0qKULKxUNKrBP7BfyYriJ48Hmz5auHgGq6SD30WnWmYCBlhcJcyq4Uc960pimw0A6rR-W2qw23GmiAETdH9evUEQp-WZ9GWH07wT4aCw3EbjcH28GYq7tKe7Ayy69x3Wqll7fiHl4dP2dcZohbU4QVJVL_4DeU2F5avcm8C9UWUYQ6AMLKk9uzpB51ZaRy4K70omGxhLAdiTV-rDnoHH4ZTxwD3kktfd9umT9-IsuHUMAYpJfFaiiAWyMWn9QVHZCvCuc_eNQjrs2NW1br8vo5tlUb95riRrb9Aw-oljaOxg4gzwZxoLZslzOOGskfK_Qh4oLbTfPvnIw0LBMSn-CQGJtHiTOtEq_dqMCMYYdlOZJWnH-xgRHRwRc_sBm000F__0m00)


4.3. Class Diagram. 
![Class Diagram]([https://www.planttext.com/api/plantuml/png/R9BFQiCm3CRlVWgJOo5XlVPKjcviiCEWetUbqJQ3_nHRXfRH9-kXZxHNc1BifCGrnk2Vq2Vfi_ykrtKWy1ID5diD8SXjR8sYJsNm2NptuhoHlqBogkKNNzwwbToIL_OxGHLse1NJH-SqWXLdaPLEWN3AtaVlqT8625UoFnCtS7nrqOSFzBoLOwcDYwt6IUdP7BGx8OvQc43HZGM3CuG6b9wn7oxuhdZEibQUVAn52HIr1kEAST1s1Gk3fuHt8WGKmqoO784UFBbjxyx3r7KoMIIl6MIlRb3E4QEFrRBg0zL3qoogARxcvlkVy0y00F__0m00](https://www.planttext.com/api/plantuml/png/R9BFQW8n4CRlUOgmHs6blNeIjSM21y7YVNIdRI1_99c08dqo3pwIh-3iajsLpOOGcDyatsI-v76xpmE1fsYqE6e8GUxYmIZwLWQNuAjFvusy2icZb3ySV5KpkIElx6-2Akn1AwOBvpI25V-YLRe4mlxqCNgFbbP0E9FrchY1yzf57xReUIh7KYiN3nfxfGzpqkw2s6bX0jbjB1WS83IWz83zSS6DuZxpMctdNIrA8AlL69UrWxRAM6Wy9Hp9450C0s5o1BhnvFLwoSwo77aYaIFUrzesagrbsbXqzXRlHPqetgRJIT7dvznJ_K6U0000__y30000))

5. Hợp nhất.
![Class Diagram](https://www.planttext.com/api/plantuml/png/h5JRIiD047tFLuGy2YtwMaIgLb6efH3nVPECTd4lPMSMBEAN-U0d-GjEOh9Diwq86a9Wpypcp3adsS_tZocISEIrIaeb4DCS59Iq51iDXkw0LhQwjawdhqdAroXzvCLjDKbpSj8yjU2wtuwJT2wHJhyxpjeMYGz2ITvuOQq2OPAtf6NSuRgqXfnLWGwRSQ3QQHgmQo4LhywhoW7Ye5W8yxmG6WQmA4lh3IsyBi25MfZfIg-LtG24EQ058kacVlVwBxFEWBW5-oCTYcGqsklTJ_sThavdxWijwLvgk1Jk5q4VJZ7V8C5sT-cTO_QP87QdVWRzBpVMEro2urlM_ioiBnJya_TG6pp0LamubwmpvkgK1ovgWOYh-KqYEM2g2CF6K_vcume9yiFGoP9GZIVzyLexER8ueYI6-j7koPJBtJe9zcOdMLt8ZiVZesnRdxAc-ZZu0W00__y30000)

- SubmitTimeCardForm:
    Nhiệm vụ: Cung cấp giao diện cho nhân viên để nhập thông tin thời gian làm việc và kiểm tra tính hợp lệ.

- System:
    Nhiệm vụ: Xử lý logic nghiệp vụ cho việc tạo, lưu trữ và xác thực thời gian làm việc.

- Employee:
    Nhiệm vụ: Quản lý thông tin của nhân viên và gửi yêu cầu liên quan đến thời gian làm việc.
              Lưu trữ thông tin về phương thức thanh toán đã chọn và các thông tin liên quan.
  
- TimeCard:
    Nhiệm vụ: Lưu trữ thông tin về thời gian làm việc và thực hiện xác thực.

- SelectPaymentMethodForm:
    Nhiệm vụ: Cung cấp giao diện cho nhân viên để chọn phương thức thanh toán và kiểm tra tính hợp lệ.
  
- PaymentMethodControl:
    Nhiệm vụ: Xử lý logic liên quan đến lựa chọn phương thức thanh toán và cập nhật thông tin cho nhân viên.
  
