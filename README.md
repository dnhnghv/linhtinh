# linhtinh
%% Use Case Diagram: Phần mềm đặt lịch khám bệnh trực tuyến
%% Copy đoạn này vào trình hỗ trợ Mermaid để hiển thị
%% Actor: Patient (Bệnh nhân), Admin (Quản trị viên), Doctor (Bác sĩ)
%% Use Cases: Register/Login, Search Doctor, Book Appointment, Manage Appointment, Receive Reminder, Manage Schedule

%% Khai báo sơ đồ
  %% Sử dụng graph TD với Mermaid Use Case style
  %% Các actor
actor Patient as "Bệnh nhân"
actor Admin as "Quản trị viên"
actor Doctor as "Bác sĩ"

%% Các use case
usecase UC1 as "Đăng ký / Đăng nhập"
usecase UC2 as "Tìm kiếm bác sĩ"
usecase UC3 as "Đặt lịch khám"
usecase UC4 as "Quản lý lịch hẹn"
usecase UC5 as "Nhận nhắc lịch"
usecase UC6 as "Quản lý lịch làm việc"

%% Quan hệ
Patient --> UC1
Patient --> UC2
Patient --> UC3
Patient --> UC4
Patient --> UC5

Admin --> UC6
Admin --> UC4

Doctor --> UC6
Doctor --> UC4
