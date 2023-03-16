### BÀI TẬP 1:
1. Tạo project mới: tree-management với package default: **vn.sunasterisk.treemanagement**
2. Tạo class Main trong package **vn.sunasterisk.treemanagement**. bên trong class Main có một phương thức: `public static void main (String []args)` để chạy chương trình
3. Tạo package model bên trong package **vn.sunasterisk.treemanagement**
4. Trong package **vn.sunasterisk.treemanagement**.model tạo class Flower
    + Thuộc tính: `name (String) , color (String)`
    + Hàm khởi tạo có đối `Flower(String name, String color)`
    + Phương thức: `displayInformation()` hiển thị thông tin name và color của flower. Yêu cầu hiển thị theo định dạng:
       Thông tin flower: [name] - [color]
    + Phương thức `changeName(String name)` dùng để đổi tên của hoa.
    + Phương thức `changeColor(String color)` để thay đổi màu sắc của hoa.
5. Trong package **vn.sunasterisk.treemanagement**.model tạo class Tree
    + Thuộc tính: `name (String), height (double), flower (Flower)`
    + Hàm khởi tạo có đối `Tree(String name, double height, Flower flower)`
    + Phương thức: `displayInformation()` hiển thị thông tin name , height và flower. Yêu cầu hiển thị theo định dạng:
       Thông tin tree: [name] - [height] - ([thông tin flower khi gọi `flower.displayInformation()`])
    + Phương thức `changeName(String name)` dùng để đổi tên của cây.
    + Phương thức `changeHeight(double)` để thay đổi độ cao của cây.
    + Phương thức `changeFlower(Flower)` để thay đổi loại hoa của cây.
6. Trong hàm main của class Main
    + Khởi tạo biến flower1 từ class Flower với giá trị truyền vào: name: "Hoa hồng", color: "Màu đỏ"
    + Khởi tạo biến tree1 từ class Tree với giá trị truyền vào: name: "Cây hồng", height: 1.2, flower: flower1
    + Hiển thị thông tin tree1 ra màn hình bằng cách gọi phương thức `tree1.displayInformation();`
    + Thay đổi name của tree1 từ "Cây hồng" -> "Cây hoa hồng" bằng cách gọi hàm `changeName`
    + Hiển thị thông tin tree1 ra màn hình bằng cách gọi phương thức `tree1.displayInformation();`
    + Thay đổi chiều cao của tree1 từ 1.2 -> 1.3 bằng cách gọi hàm `changeHeight`
    + Khởi tạo biến flower2 từ class Flower với giá trị truyền vào: name: "Hoa hồng", color: "Màu trắng"
    + Thay đổi flower của tree1 từ flower1 -> flower2 bằng cách gọi hàm changeFlower
    + Hiển thị thông tin tree1 ra màn hình bằng cách gọi phương thức `tree1.displayInformation();`

### BÀI TẬP 2:
1. Viết chương trình kiểm tra số nhập vào là số dương, số âm, hay là 0
2. Viết chương trình cho phép nhập vào số bất kì và hiển thị ra tương ứng 1 là thứ 2 và 8 là chủ nhật, nếu ko thuộc phạm vi 1 đến 8 thì hiển thị là **Data invalid**
3. Viết một chương trình Java để nhập vào điểm của một sinh viên và in ra xếp loại của sinh viên đó dựa trên bảng điểm sau:
- Điểm từ 0-49: F
- Điểm từ 50-59: D
- Điểm từ 60-69: C
- Điểm từ 70-79: B
- Điểm từ 80-100: A

(Nhập từ bàn phím:  `Scanner: Scanner sc = new Scanner(System.in); sc.nextLine();`)

Một số lưu ý:
1. Khi nào nên dùng if-else, switch-case?
- Sử dụng **switch-case**: Khi điều kiện cần check là đơn giản và  có **nhiều hơn 3 trường hợp kết quả cho điều kiện**
- Sử dụng **if-else**: Khi điều kiện cần check **phức tạp** hoặc Khi điều kiện cần check không phải là kiểu **so sánh bằng**
2. Chú ý khi dùng switch case phải có break trong các case nếu không chương trình sẽ chạy từ trên xuống dưới
3. Loop
- **While**: Dùng khi không biết về số lần lặp
- **For**: Khi xác định được số lần lặp
- **do-while**: Khi không biết được số lần lặp nhưng phải có tối thiểu 1 lần được run code bên trong vòng lặp
- **for-each**: Dùng để duyệt từng item qua 1 mảng đã có (không thông qua index)
4. jump
- **return**: dùng để dừng vòng lặp và thoát khỏi method chưa vòng lặp đó nếu có. Và trả về kết quả cho method.
- **break**: Thoát khỏi vòng lặp hiện tại gần nó nhất
- **continue**: Bỏ qua các dòng lệnh chưa được chạy của vòng lặp hiện tại và bắt đầu vòng lặp mới
