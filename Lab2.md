1.Create Employee
1.1. Xác định các lớp phân tích 
- Boundary: 
    - ReportSelectionForm. 
    - ProjectDatabaseInterface. 
- Control: 
    - ReportController. 
- Entity: 
    - Employee. 
    - Report. 
    - ProjectManagementDatabase. 

1.2 Sequence Diagram
![SD](https://www.planttext.com/api/plantuml/png/d5IzQXj14ExtAGPN4YWlu28OImc4n2R4AjAkJfkx2tkxOZLhScL8uI84aY9bmCA4WC4u8TrTuM9DtcEV8A-GEKctTx9r1gNGeVsPx_jclfdzMzuSp94Rj9baF49ju4asapeNWasqLLDkSdWbPjhWYP0YmbIhfzfaBD8AZPRhi-5g9OLfebuQ_PO2HXpvXC_5CuN2lE6HO49XYk7yY2iUYumswvlrXHKqOxIG0iQ-M6WuTUVmMcHmw6WHqOUnMYyyUhnDAUn3bFZoamAf2IA5IHFA9SAnBsviimcI6FR6llogOeXJNtwhTZB2q33rvIzm2xN7O2jJ4D2KWzXpTsaXyiKF2xZC8N3rLeggN8Rq6u2AtNb-w8jhlFrS1QntdfD472UkYFg1kKL1j5sr9dhfY-_vYAlan2sYvCXTZ2WBzrxrAgpEk0RplZy4YiRcyCuID0uJRc9nRBE9CFCbg15eZO9fpRbneoE1xSObLFyF2f3y-xZ4Wta529cx26Rq-ZkviUg5EsNOiQInBw_I5aGM_lQfTwUCTMUueULEEp2bKO19umJNPtLdxDue0sYBgXtnvVKBAkcPhP4UalgW6SsyL8CHdenceC9KriFtvsTholvtW3fGjiclMfzkXn9MFhSBN1tsJYcNiN5N0q1tgMZgpsOR5jwJ5zBQXzilxZUz4Qtdv80YwHtz1m00__y30000)

1.3 Class Diagram
![CD](https://www.planttext.com/api/plantuml/png/f5DRIiGm5FtFAl8vGcSBCb0L11t4SGDtqbkDv6LoEr34bVdXajo2QHhwS5eG_ChbFiuvzoJv_lpQ1G9FZLPCA0Y1NskdR8l8tndd0HKAUaHdFJsr3ZSNG_B1szTubBRginxV6WnqW1Fs_J7xmJ9edpcaGMdDZVLw7R-ImIbe9mHtCj2qb0byEgw0O4r0P6YEMix4kZ4-KrXQGzugXJx9ov2bHo2SaNPY2vwiY_mnH5DrGKTP8ucN9VNYxpW5dycCUopwcbaw2uuGyDOG-Xe4PlNa9Pvm8YKi3D-3WMVKQ0QODEtc2_nsAlNyTw6DiWAw1r7mMYhSW-wlvEmojjlBpBjSM_E1hHeqcJetW2szrr73ICw6tp9MPrDi5_UFd-i7003__mC0)

2. Maintain Employee Information
2.1 Xác định các lớp phân tích 
Boundary class: 
    - EmployeeUI
Control Class: 
    - EmployeeController
Entity Class: 
    - Employee

2.2 Biểu đồ Sequence
![SD](https://www.planttext.com/api/plantuml/png/x5LBJjn04DttAKgiG88SO1OHY47HB93uY0Cqxe9fqQusvJB8rqbsMRCYYhAOa-G4kKBACvvf3CDWis639Ll-z7lrwhso_U_Nd_rIB4kL1sCpYGmdjkOOme7BFVbIsEfDSnahSfPhECgB46l4Yud98eckNDqwN5m7P8CaNj9YO_Go89nMVnz_48JPRv3fx86kGJm1JMVV2Uxyx2SPiwuwx7rzKdS4vurWs3gsdaJtrJEOq5Nat8gFj6KIei6lunt12SUy450KQFCAW-q3vtRXed1MS1V6651mnnWR1FG9s5JDW6wzv2f99cs1EQgFj2CIPC1bQmwrrL32DjbSXKbTw14b-xBJIqVAfj53xWLnHrTQ_PHZ18UCQWiGtYSyOnRPTU2l5Vw6XDmGhC2JSO-wZOTZNnR1rjtIpz2Rt3oVnliNO0mbjb5_NB1j4qC2FCFR2aj975xd7YxhVdOsU66FTzWbw1MXGYkc3S2t8tmTkycrDgQrOpju-AivsJjVWkTA1hm0UdxbEM_hB-PlyOdvdB-FcR_vfpzRn687sRZCqZNvBO53NEmG92zwENXi-IOrqlImag7pRSo-7lMF_Xy00F__0m00)

2.3 Biểu đồ Lớp

![CD](https://www.planttext.com/api/plantuml/png/V59HJiCm3FtFAV897xr0XQOX5QHA32461_0QhukKEbNY84M8a_71aRW2AMkdZAxyHF9xzdjsxE_FhxLdS1mw8ne3tiidYCuQSwiwJTgp0xPElWif2yYXkYgb9XvmWWvBkMMdgKsnz6YmuVj03MjBLzUbVBDQYGynEjnrlR4HyRK-wXxpKKqLcLQXgGzS0KDkeBJl3SH9fwQzFRaa6edHJUHGcvEDfRrsNPKy_-zk0mGjZgFZ23wayKivl3TJtcfG1QMcE3SBlGB6IumQ_EVCh8jp--LFFwMynFuCJvqvz3w7l6qqc2qsmMcEZw7ReSlv_c09v_311cVYSngebCg6dS5VCJ3WOeR85dbfCtw1IcDVFBkYM6NN8hB3oPbnK-Blvl8SiKPIwSX_0000__y30000)

3. Run Payroll
3.1 Xác định các lớp phân tích
Boundary: 
    - PayrollUI.
Entity:
    - Employee
    - Timecard
    - Payroll
    - BankTransaction
Controller: 
    - PayrollController.

3.2 Biểu đồ Sequence
![SD](https://www.planttext.com/api/plantuml/png/V5EzRi8m4Dxz5ATC89KNOAXG2rKPYgXArTbrBiJAnOxEbu77wTvAtJjqGE9r-Wfr805Ke8lb--w-7vsJdw_lKH3DKfUaj17FCDShzaJFKsMyatZjaDjTISWAdLXPmQIioAyGktfXIpIQqwvkYLrversnOEr2DBBUAHLHGdYiLo2yVdSvoFeZdhJvtBovfLBxA32uFaqn1AvTY_RwwgJVaBg4GrYYJCWkxIjX1uR8OfIQ7P0D0Zu3R4S0kncboFiAihWPr2RVDnIS9ZfnlFSrXrv7cQRzo6eTywRruhd0z99K2mx1Q38rQS4PIWGRmQdB_DMno96qsqx5MfCq8cNSFvGekK_11aZ6bj48ZB7omKeI1oy4-FDWGwZO6mpX23jasRdsjsfj43dCFOcMEiGcKi1peHwqfGJYbfEvDSMWhlx9jLzCnTOrhYP7KvoBWkxYTWyFLMekxZoFaR29EircY2ccyUjew6eKp_Xx_0800F__0m00)

3.3 Biểu đồ Lớp

![CD](https://www.planttext.com/api/plantuml/png/Z5H1Ri8m4Bpd5Ju62JuGLGZHK1MfHPL0wdbhBs3Xs96zgHHLVLaFVLA_K3l4912AUY5aTdTsPhtEpzVtp15OgWgLS0NEiHUehL6AVIICCLlfzZqTPUpTI17GqafD7kTxv8SKYtAfjoPZYw9KfaOSCuqXdB47PO1wXKAwKa7TKgu9g7AfQnuPMvEdtSNip-HSpxtH59veRodR8IsKtCatXL6D2_4dwUWk8jEZ1yFHkOXvhc2a-TyvwJ4NO0yFnkQeaAJHo-qAKQ2uKNHo40EDy4aiM8feEQ0E5DWuiG2KK1UewHbfRyuoWn0KFIaPcnkZ47IGALtqxpFYW7XbhUVAWRpCy3jcg4NtEZgZs3M75vhdI21LCy0MwKnjP84ShBXbQcygwrvDqDjp9avzsswF8IqTKenYqUKk73U0W-ALyZIhHl2rFHmA67L269IbgdCK5GzZT4E2eO0vwCF6WdRGr1pDKmUS-uV2L9fw7Tkbwp7yv_R4i_4guW0ca-dmOYJ3gnBo8l4VuNYGryAd9jU35zD8Pdwh_8Va5m00__y30000)

4. Create Administrative Report
4.1. Xác định các lớp phân tích
Boundary:
    - ReportSelectionForm.
Control:
    - ReportController.
Entity:
    - Report.
    - Employee.
    - ReportDatabase.
4.2. Biểu đồ Sequence
![SD](https://www.planttext.com/api/plantuml/png/d5GxRjj04Ett55DAWdC15O4DosbY2q7a2uoMOscHvIwp7mCyWMiVmN1dm402f38B5mHo3vuWLyY87z2MQGboivWXEU_Ds_V0VyNpiG_eGaorG1ciWs-OEwlrIP8getnmo0_5qaQJeClXEsNMXGLfaa5PyyMwL4Xh0e-qxqwRJfCJP88AtSphReO1b-X927we2IQJMLNyXlBEGAYUxYmiIpua7vE944CxmQVFGzjCWNd8jRiunRN2aQlRopoZ8rZIIXdcvv9CqXPffcrEDCUK_5WCuFPqlS0fEFePoOUEZN3p-Q5i0dM0UVNq726eyY62N9UFiAwA-mnqLTm8UCFSRpC5kQ6bfZkKkaCULhSYGtpNbBGExjfZouH4-KnZtcwr1SII0NhHhRlmsjuqLiMj0VttL-p3m7CmHBZJdGLUqum2Akr7uyCGwYozdBzIkhwx8zXKvrRMZhz47RgSBkrJy8mrV2aDucxi3kSzkRKgPaZsx3DirgBUpKSTHZvAIRuE26dc6trTbt_CQikDVRBVqaXqhTpQ2OwbQF0l--3_QAZw_8y_4BmpvwoxO0cu8gRQ48bZFla_zny00F__0m00)
4.3. Biểu đồ Lớp
![CD](https://www.planttext.com/api/plantuml/png/d5F1QiCm3BtxAtHSeFc1K4gXtM1GTbZt0sgY1ODZ1rihXB4lss6Vj5-O7QT9t6o7xX8KwUcz9qNv_lpQEaRBRuqIfKBdu9bQO_b8YagMHZyOsy2x003IJ3PMTrRwMEATxLzVkfPMSA9QwZso3qbNGz2qodH4JzYGom9B9Lshi8iyGtycFaIYlZEQhL6AR9GkBNcwfESMJOVdj7a5hrBrW1WTJ8bXs1vzHYMhKUw_ervDv35uGaTndjiCrSG9-76_eEzfyybY0KUsKjSXEvej83n3QZ0zIypD5t2GZjUHOHFAVXque_IEDDdfYsHZRRHrFn16OzhJflqSbDB6tmulppUBan2B6vbGbpMBgwrFYA42wpp_Yxb7NmOGMxyi_tVy0000__y30000)

5. Login
5.1. Xác định các lớp phân tích
Boundary:
    - EmployeeLoginForm
    - PayrollAdminLoginForm
Control:
    - LoginController
Entity:
    - User
    - UserDatabase
5.2. Biểu đồ Sequence
![SD](https://www.planttext.com/api/plantuml/png/x5IzJiCm4Dxz53Us4hn01rGeC25K8M1tawEnwjZXV0PbPc3c6HYO40jJEdIWBv8du1LmsaB_WbfLZ6H8xZwVl-z-x7mEHst7ajYdMiY8BS59cccR8yxShip9QdqOfyeenoG3A7hMcrXI_XDyPllAd5fAvqkB6-VBaJKSO9WWdQcZaKGiMVQaGxXoICSpHw1XnVa44oAO6k6eBDuOnazbyUB3P_nW-c2IidZDXFZE1lOFLWLQ4BYGEeHnHIgrQnYPuXvaqhbxIt5Jr5Mw6vEGck6yB4OUEFbu3ncoCf2Km-SCT3by512U5TfAQR7s5X3UUdGyYLkJg1WMmsiJlPDQXSPY5LWHxCOI9HWDkhCz3MKopzqb1aBsP42vwqhlDwYcthNJqu9OkKpB_0ATrznmFehGkQP07PAxdFToC3KtjtIZn8rKsXC62HF_3sxBmTNUxRyVtbOoomDiXtVubtq1003__mC0)

5.3. Biểu đồ lớp

![CD](https://www.planttext.com/api/plantuml/png/l5DBJiD03DtFARmC4hb05wXGOCKYQiK1JCOg8-OJF4vHX3WP2ux45SYaBOGqWaX5hERZz_p6VfxtrxTv56IfdLMbnHZXobKsD4Jmh01oZuvci18sVftELGjv2gnxTq1UY1TCkjqOj37haqvXI3cPmIOOhLxKJh70XeErvzePRw8mIk3_Kz_NUnFMnby7TfqqQ1ChYysIOcqbuswPLC4nUJhk8dX9sMZR161wh2bA5vjONClQe3KQXMuZSIBzphm8mHBwhzSawYKAtc7SJiDV9PrkRdbFvKEn2sJ6LxKKFufyJc-UdnrQgqP7BK577LI7iv6m0vVKkFjZoA6_2TFlilhMydrKpSdhzeD-0000__y30000)

6. Maintain Purchase Order
6.1 Xác định các lớp phân tích
Boundary Classes:
    - PurchaseOrderForm
Control Class:
    - PurchaseOrderController
Entity Classes:
    - CommissionedEmployee
    - PurchaseOrder
    - PurchaseOrderDatabase

6.2 Biểu đồ Sequence
![SD](https://www.planttext.com/api/plantuml/png/f58zImCn6DxpAzvHeTAzWnJEhw6WWuDhcekzm2Kf-G1lTd0G1sS7FQG8Ib7GwJ8uNEd_o2_mBvXKwbsBkhZaJTuypvFdIVBXtllQO6Kipn4cHYf89ETCQoO5JNVvE9S5fO0rM4qL6aehKgmAEBAAP5ZJGvLIjISLZv3JK16HmYYPhoAIhsPELSIHxnMYmZ2p9XSXCavGYWqUXlRg_iwo6t1B14BH7snjBqpq8Ccykn9WCYp1r2M1ZMDVbR83YQ-cOn1PAAO39_KhtaIH4gcDhnxiUpTbKDIF5eYl7YoOoE-I5hrx5jWmkvwN0hBwJenG8z0uEM3UdKSdtbs6iNuJ8p1CjAJNQCj8FHZuQbAqESQx9o3p4hHtjv1wzmnvaB-mFqPO9Ews0xUrVlVT6FWFTp1_iNy0utE50snG39Sm6GElxzjmuDxTCDId8Wr_ynC00F__0m00)

6.3 Biểu đồ lớp

![CD](https://www.planttext.com/api/plantuml/png/Z5DBJiCm4Dtd55PM1T55jnMgMZKWLKAYWXEuza0jsPxWJr65E1aBZiGLcAHfSDAcOXDvnlFUctcU_7nzpttWBaIZCw6vzso9nYZl5LgGTwRKk0TW7nbZq0IhOigUWrFsbPAM6qX2WJPm4PHzmJRxcJNCw-Z4bdjuT1BSFJfJquejeeS5WT2EhgPiXqfIMYfVQhvV4LEIzLjyh-6heisUvrzI9mwr1bUhb0u5UFy4Rn5yI1Y50nwW0nrXhK3AVsMnb0DbnKrpARi82He649Sxh_jjAbDhemze3eEHnSdDHcbDfuMKZaPCBcXe6KMWr8FouNPz26T7-eAQdhBgctHog3bwLfqllNVfbAWuC6uq3Cn30dn3GStfWA2mE_6ZWwWUcdTgUWLzbuVSFRlB-IHdu_6CvTTvp_ZiT4FRuaa-j5_PqDxzL-WSf2_NcjY5TZMQjylcO2NzqBy0003__mC0)

## Code java mô phỏng ca sử dụng Maintain Timecard.
```package maintain;

import java.time.LocalDate;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;

 Class đại diện cho timecard
class Timecard {
    private int employeeId;
    private LocalDate startDate;
    private LocalDate endDate;
    private LocalDate submittedDate;
    private boolean isSubmitted;
    private Map<Integer, Map<LocalDate, Double>> hoursPerChargeNumber; // Charge number -> Date -> hours
    private static final int MAX_HOURS_PER_DAY = 24;
    private static final int MAX_HOURS_PER_WEEK = 40;

    public Timecard(int employeeId) {
        this.employeeId = employeeId;
        this.startDate = LocalDate.now().minusDays(LocalDate.now().getDayOfWeek().getValue() - 1);
        this.endDate = startDate.plusDays(6);
        this.isSubmitted = false;
        this.hoursPerChargeNumber = new HashMap<>();
    }

    public boolean addHours(int chargeNumber, LocalDate date, double hours) {
        if (isSubmitted) {
            System.out.println("Timecard đã được submit, không thể thay đổi.");
            return false;
        }
        
        if (hours > MAX_HOURS_PER_DAY) {
            System.out.println("Số giờ làm việc trong ngày không thể vượt quá 24 giờ.");
            return false;
        }

        if (date.isBefore(startDate) || date.isAfter(endDate)) {
            System.out.println("Ngày không nằm trong khoảng thời gian của timecard.");
            return false;
        }

        // Tính tổng số giờ trong ngày
        double totalHoursForDay = hoursPerChargeNumber.values().stream()
            .mapToDouble(dateMap -> dateMap.getOrDefault(date, 0.0))
            .sum() + hours;

        if (totalHoursForDay > MAX_HOURS_PER_DAY) {
            System.out.println("Tổng số giờ làm việc trong ngày vượt quá 24 giờ.");
            return false;
        }

        hoursPerChargeNumber.computeIfAbsent(chargeNumber, k -> new HashMap<>())
                           .put(date, hours);
        return true;
    }

    public void displayTimecard() {
        System.out.println("\n=== Thông tin Timecard ===");
        System.out.println("Employee ID: " + employeeId);
        System.out.println("Thời gian: " + startDate + " đến " + endDate);
        System.out.println("Trạng thái: " + (isSubmitted ? "Đã gửi" : "Nháp"));
        if (isSubmitted) {
            System.out.println("Ngày gửi: " + submittedDate);
        }
        System.out.println("\nSố giờ làm việc:");
        hoursPerChargeNumber.forEach((chargeNumber, dateMap) -> {
            System.out.println("\nCharge Number: " + chargeNumber);
            dateMap.forEach((date, hours) -> 
                System.out.println(date + ": " + hours + " giờ"));
        });
    }

    public boolean submit() {
        if (isSubmitted) {
            System.out.println("Timecard đã được submit trước đó.");
            return false;
        }

        // Validate total hours per week
        double totalHours = hoursPerChargeNumber.values().stream()
            .flatMap(dateMap -> dateMap.values().stream())
            .mapToDouble(Double::doubleValue)
            .sum();

        if (totalHours > MAX_HOURS_PER_WEEK) {
            System.out.println("Tổng số giờ làm việc trong tuần vượt quá " + MAX_HOURS_PER_WEEK + " giờ.");
            return false;
        }

        this.submittedDate = LocalDate.now();
        this.isSubmitted = true;
        System.out.println("Timecard đã được gửi thành công.");
        return true;
    }

    public boolean isSubmitted() {
        return isSubmitted;
    }
}

 Class quản lý Project Management Database
class ProjectManagementDB {
    private boolean isAvailable;
    private List<Integer> chargeNumbers;

    public ProjectManagementDB() {
        this.isAvailable = true;
        this.chargeNumbers = new ArrayList<>(Arrays.asList(1001, 1002, 1003, 1004));
    }

    public List<Integer> getChargeNumbers() throws DatabaseUnavailableException {
        if (!isAvailable) {
            throw new DatabaseUnavailableException("Project Management Database không khả dụng.");
        }
        return new ArrayList<>(chargeNumbers);
    }

    public void setAvailable(boolean available) {
        this.isAvailable = available;
    }
}

class DatabaseUnavailableException extends Exception {
    public DatabaseUnavailableException(String message) {
        super(message);
    }
}

Main class để demo với user input
public class Maintain {
    private static Scanner scanner = new Scanner(System.in);
    private static Map<Integer, Timecard> timecards = new HashMap<>();
    private static ProjectManagementDB projectDB = new ProjectManagementDB();

    public static void main(String[] args) {
        System.out.println("Chào mừng đến với Hệ thống Timecard");
        
        while (true) {
            try {
                System.out.println("\n=== Menu ===");
                System.out.println("1. Xem Timecard");
                System.out.println("2. Thêm Giờ");
                System.out.println("3. Gửi Timecard");
                System.out.println("4. Thoát");
                System.out.print("Chọn một tùy chọn: ");

                int choice = Integer.parseInt(scanner.nextLine());
                
                switch (choice) {
                    case 1:
                        viewTimecard();
                        break;
                    case 2:
                        addHours();
                        break;
                    case 3:
                        submitTimecard();
                        break;
                    case 4:
                        System.out.println("Tạm biệt!");
                        return;
                    default:
                        System.out.println("Tùy chọn không hợp lệ. Vui lòng thử lại.");
                }
            } catch (NumberFormatException e) {
                System.out.println("Vui lòng nhập một số hợp lệ.");
            }
        }
    }

    private static void viewTimecard() {
        System.out.print("Nhập Employee ID: ");
        int employeeId = Integer.parseInt(scanner.nextLine());
        
        Timecard timecard = timecards.get(employeeId);
        if (timecard == null) {
            System.out.println("Không tìm thấy timecard. Đang tạo timecard mới...");
            timecard = new Timecard(employeeId);
            timecards.put(employeeId, timecard);
        }
        
        timecard.displayTimecard();
    }

    private static void addHours() {
        System.out.print("Nhập Employee ID: ");
        int employeeId = Integer.parseInt(scanner.nextLine());
        
        Timecard timecard = timecards.computeIfAbsent(employeeId, Timecard::new);
        
        try {
            List<Integer> chargeNumbers = projectDB.getChargeNumbers();
            System.out.println("Các charge number có sẵn: " + chargeNumbers);
            
            System.out.print("Nhập charge number: ");
            int chargeNumber = Integer.parseInt(scanner.nextLine());
            
            System.out.print("Nhập ngày (YYYY-MM-DD): ");
            LocalDate date = LocalDate.parse(scanner.nextLine());
            
            System.out.print("Nhập số giờ làm việc: ");
            double hours = Double.parseDouble(scanner.nextLine());
            
            if (timecard.addHours(chargeNumber, date, hours)) {
                System.out.println("Giờ đã được thêm thành công.");
            }
        } catch (DatabaseUnavailableException e) {
            System.out.println(e.getMessage());
            System.out.print("Bạn có muốn tiếp tục mà không có charge numbers không? (y/n): ");
            if (scanner.nextLine().toLowerCase().equals("n")) {
                return;
            }
        }
    }

    private static void submitTimecard() {
        System.out.print("Nhập Employee ID: ");
        int employeeId = Integer.parseInt(scanner.nextLine());
        
        Timecard timecard = timecards.get(employeeId);
        if (timecard == null) {
            System.out.println("Không tìm thấy timecard cho nhân viên này.");
            return;
        }
        
        timecard.submit();
    }
}
```

