# Robot Làm Sạch ROS

## Giới Thiệu
Dự án này triển khai mô phỏng robot làm sạch sử dụng TurtleBot3 trong ROS Noetic. Robot được thiết kế để thực hiện công việc làm sạch trong một môi trường ảo.

## Cài Đặt

### 1. Cài Đặt ROS và TurtleBot3 Gói
```bash
sudo apt-get update
sudo apt-get install ros-noetic-turtlebot3 ros-noetic-navigation ros-noetic-dwa-local-planner ros-noetic-slam-karto
sudo apt-get install ros-noetic-slam-gmapping
sudo apt-get install ros-noetic-move-base

2. Tạo Workspace và Cài Đặt Gói

bash

mkdir -p clean_robot_ws/src
cd clean_robot_ws/src
git clone https://github.com/Meliodax17/Robot_clean.git
cd ..
catkin_make
source devel/setup.bash

3. Thiết Lập Biến Môi Trường

bash

export TURTLEBOT3_MODEL=burger

Chạy Mô Phỏng

bash

roslaunch clean_robot clean_work.launch

Các Bước Thực Hiện

    Cài Đặt ROS và TurtleBot3: Cài đặt ROS Noetic và các gói TurtleBot3 cần thiết.
    Tạo Workspace và Cài Đặt Gói: Tạo một workspace mới và cài đặt gói từ repository.
    Thiết Lập Biến Môi Trường: Đặt mô hình TurtleBot3 thành "burger".
    Chạy Mô Phỏng: Sử dụng lệnh roslaunch để khởi chạy mô phỏng làm sạch.

Đóng Góp
Nếu bạn muốn đóng góp vào dự án, vui lòng mở một issue hoặc gửi pull request.
Giấy Phép
Dự án này được phân phối dưới Giấy phép MIT.
Trong mẫu này, bạn có thể thấy cách sử dụng Markdown để tạo nội dung dễ đọc và tổ chức. Hãy thay đổi thông tin và mô tả dự án sao cho phù hợp với nhu cầu của bạn.
