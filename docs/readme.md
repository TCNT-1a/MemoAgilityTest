# BOT lấy dữ liệu điểm thi học sinh và tạo báo cáo.

Link web

```
https://lookerstudio.google.com/u/0/reporting/6a99f06c-f0a9-4aa8-8d68-058b1afdb6a5/page/cOHMD?s=pKnsq0u7hHc
```

# Phần 1: Cài đặt môi trường

- Phiên bản Bot được phát triển ở phiên bản UiPath 2024.10.0

![alt](uipath.png)

- Máy tính cần cài đặt Uipath, Google chrome, và Microsoft Office Excel.

# Phần 2: Cấu trúc thư mục

Một số thư mục và file quan trọng
![alt](folder-structure.png)

## **Main.xaml** file mở Project Bot

## **assest** là thư mục chứa macro xữ lý report và template report

- **Macro.xlsm** là file chứa macro và cấu hình:

- bạn có thể thay đổi config **all** thành **5** để giới hạn số lượng dữ liệu lấy về

  ![alt](config.png)

- Cấu hình benchmarks

  ![alt](benchmarks.png)

## **output** là thư mục file đầu ra

- data-source.xlsx chứa nội dung dữ liệu
- Các thư mục còn lại tương ứng số báo danh từng thí sinh
  ![alt](output.png)

# Phần 3: Các trường hợp của report

- Trường hợp thiếu thông tin

  Thí sinh **230548**

- Trường hợp pass

  Thí sinh **230001**, **230009**

- Trường hợp đủ thông tin nhưng fail

  Thí sinh **230003**

- Trường hợp vừa pass môn này, vừa fail môn kia

  Thí sinh **230393**
