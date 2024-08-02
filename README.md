# Ad Effectiveness and Revenue Impact Project
![Uploading image.png…]()


 ### Data Source: 
  [marketing_AB.csv](https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing)

  ### Data Dictionary:
  **Index**: Chỉ số dòng

  **user id**: Mã người dùng (duy nhất)

  **test group**: Nếu là **"ad"** thì người đó **đã xem quảng cáo**, nếu là **"psa"** (public service announcement) thì họ **chỉ xem thông báo dịch vụ cộng đồng**

  **converted**: Nếu người đó mua sản phẩm thì là True, ngược lại là False

  **total ads**: Số lượng quảng cáo mà người đó **đã xem**

  **most ads day**: Ngày mà người đó xem số lượng quảng cáo lớn nhất

  **most ads hour**: Giờ trong ngày mà người đó xem số lượng quảng cáo lớn nhất
  
### Introduce:
Các công ty tiếp thị muốn thực hiện các chiến dịch thành công, nhưng thị trường rất phức tạp và có nhiều lựa chọn có thể hiệu quả. Vì vậy, thông thường họ điều chỉnh các thử nghiệm A/B, đó là một quy trình thử nghiệm ngẫu nhiên trong đó hai hoặc nhiều phiên bản của một biến (trang web, thành phần trang, biểu ngữ, v.v.) được hiển thị cho các phân khúc người khác nhau cùng một lúc để xác định phiên bản nào để lại tác động tối đa và thúc đẩy các số liệu kinh doanh.

### Goal:
  - **Phân tích các nhóm, xác định xem quảng cáo có thành công hay không?**
  
  - **Việc hiển thị quảng cáo cho người dùng có dẫn đến việc mua sắm nhiều hơn không?**
    
### 1. Import and clean data
### 2. Cân bằng dữ liệu
    - Mục đích của việc cân bằng dữ liệu giữa hai nhóm (trong trường hợp này là nhóm "ad" và nhóm "psa") bằng cách thực hiện undersampling nhóm lớn hơn là để giải quyết vấn đề mất cân bằng dữ liệu. Việc có số lượng mẫu tương đương từ cả hai nhóm sẽ giúp đảm bảo rằng các kết quả phân tích hoặc mô hình hóa không bị thiên lệch bởi nhóm có nhiều mẫu hơn.
    -  undersampling nhóm ad để cân bằng số lượng với nhóm psa 

