# Lab 3: Identify Design Elements

## 1. Subsystem Context Diagrams

### 1.1. BankSystem Subsystem Context Diagram

![SCD](https://www.planttext.com/api/plantuml/png/l9BDIiGm4CVlUOhGayf-wBMKigohu4M4VO9fTbQ2oMJ9JC0YFfa77ybNC6sNKYjUlKm-vZ_p_p79ryVdXWMY9E-KSS2idw2DmRdRGDAj67LLcV5Gr_fDQRq-nM2GEOizagpLkrAM1ECH3Eg7BT3BlcL1twib0l4HutsY0r-0CI6HF2RVO2prNgAbvuK6tzsMUXTIut0n584H6sW7WZcHusMfjo4u1EeS1-29MLLnQdZOPyBNDkDQVtBOGV8_Szrbuz0YdcUKuNAqqlOZ75NdSOzKEV7x1PRB-WVy7vAvevhMT89fYxcuk5wjhefULjmKCowrGJhaF_8D003__mC0)

**Mô tả:**
- `PayrollController`: Thực hiện xử lý thanh toán qua hàm `//processPayment`, sử dụng giao diện `IBankSystem`.
- `IBankSystem`: Giao diện định nghĩa phương thức `transferFunds` để chuyển khoản, được triển khai bởi `BankSystem (proxy subsystem)`.
- `EmployeePayment`: Thực thể lưu thông tin thanh toán, được cập nhật bởi `PayrollController`.
- `PayrollSystem`: Xử lý nhiều thực thể `EmployeePayment`.
### 1.2. PrintService Subsystem Context Diagram

![SCD](https://www.planttext.com/api/plantuml/png/l95DJWCn38NtEOKrAq3zWUreDAeAc-ugzGJfZ46HFCaGEqWHucGiE19Nm1bAHLlMhA9dV_PxSZxVFrOiDaeQo7HacM5hSmn4zy5BUJ52qtH7qRRmQW2M4PyJiYZCvCQbUJF6US7uQ3k4pJQgs65ySQeAFvR20Rx2OQIG4JTz3JlHpjCCs9ADkOQ7aFQ4C-YnJvsuuFcdTbt3EWH2wulP8UjldwRXjEVCWeEcT6g20thXVupplL6JgA-JF1rBkvSddS_RirX_GDLTDO7LxM9nKnstczF1Gbnici3p-HDeXRxNJ_y2003__mC0)

**Mô tả:**
- `PayrollController`: Điều khiển quy trình `//requestPayslip`, tạo và sử dụng phiếu lương.
- `Payslip`: Thực thể chứa thông tin phiếu lương, được tạo bởi `PayrollController` và in bởi `PrintService`.
- `IPrintService`: Giao diện định nghĩa phương thức `printPayslip` để in phiếu lương, được triển khai bởi `PrintService`.
- `PrintService`: Subsystem đảm nhận in phiếu lương thông qua giao diện `IPrintService`.

### 1.3. ProjectManagementDatabase Subsystem Context Diagram
![SCD](https://www.planttext.com/api/plantuml/png/r5EnJiCm5Dpz5K-TAA8jSrL55HI93aYL69XVaqS8E7wHxGmHwfSny4dy0hQJHcdJXgvCIUxktPqT--VhUsaiQblcKiGIZO4DLfgbl6Tb_PCqB1Pn-n55y2a0PhEKx4DUIAw8DfhVAROhj1YeiaZGxj57BhKHEo4oPKc_OaomRgWdL9XIJYgCRj5Gy7RE7SShQbBMoHoUhSvKEfx3OMG_yCJK3HIre0kzUV4Bwmzou8hBhIJdViSi2PLltUp9sSAPomc8-OVBQdyWLhwkgzcdQlDJL1SxaFLFq6GIzSBEo0PsyI_ZUb0SLn_TJgVNeo1jNjiLNA3TCsAWc9SFr5wIIjpz-WK00F__0m00)


**Mô tả:**
- `PayrollSystem` gửi yêu cầu Store Timecard để lưu thông tin bảng chấm công vào ProjectManagementDatabase.
- `PayrollSystem` sau đó gửi yêu cầu Retrieve Timecard Data để lấy dữ liệu bảng chấm công từ ProjectManagementDatabase.

## 2. Analysis Class to Design Element Map

|  Analysis Class           | Design Element           |  
|---------------------------|--------------------------|
| LoginForm                 | LoginForm                |
| MaintainTimecardForm      | MainEmployeeForm         |
| TimecardController        | TimecardController       |
| PayrollController         | PayrollController        |
| PayCheck                  | PayCheck                 |
| BankService               | BankService              |
| SystemClockInterface      | SystemCLockInterface     |
| PayrollController         | PayrollControllerImpl    |
| Employee                  | EmployeeEntity           |
| Timecard                  | TimecardEntity           |
| Payroll                   | PayrollProcessor         |
| BankTransaction           | BankTransactionProcessor |
| PaymentUI                 | PaymentUIComponent       |
| PrintService              | PrintServiceProcessor    |

## 3. Design Element to Owning Package Map

| Design Element           | Owning Package                        |
|--------------------------|---------------------------------------|
| LoginForm                | Middleware::Security::GUIFramwork     |
| MainEmployeeForm         | Applications::Employee Activities     |
| TimecardController       | Applications::Employee Activities     |
| SystemClockInterface     | Applications::Payroll                 |
| PayrollController        | Applications:: Payroll                |    
| PayCheck                 | Business Services::Payroll Artifacts  |
| BankService              | Business::Banking                     |
| EmployeeEntity           | Data Access::Employee Management      |
| TimecardEntity           | Data Access::Employee Management      |
| PayrollProcessor         | Business Services::Payroll Processing |
| BankTransactionProcessor | Business Services::Banking            |
| PaymentUIComponent       | Middleware::User Interface Components |
| PaymentUIComponent       | Middleware::Print Services            |

## 4. Architectural Layers and Dependencies

![ARL](https://www.planttext.com/api/plantuml/png/V591QiCm4Bph5Vv0lb2Ik2a44WWaVS2otgR2qgvOAIccz6Kzz4dzGkKIsueBlGdDxCpiID-VNykOGDF5EnC0MpXJjGh1MOHaXNVGaLRlfghGGOpL7YnlV73I4Js9-X4uMKy8sjJ2ISKvqX4wTZ6HhvrWk-L4-W988tY0hgSNOnzc3BAtJUFe3PIA23ivMxxppXgUE3rlQ_51E1__WmhzzILQfXYFf5UBfKcUmrV2ThnO0xStsZpxGGMpYEWT-QJ04R0lSI8Kte-GO8Nz_Q_jC3gKk-5aKrS0Gy4t82lzUQR5uc6-afcls7EcMatHS8zCeOnP4ZVvL_m0003__mC0)
