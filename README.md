# 🎯 Đề tài: Thiết kế kho dữ liệu cho nghiệp vụ cho thuê đĩa DVD

## 🌐 Giới thiệu dự án

- Cơ sở dữ liệu **tSakila** là một phân hệ duy nhất, mô phỏng lại các hệ thống cửa hàng cho thuê DVD cùng một thương hiệu.
- Kho dữ liệu **tSakila** bao gồm các bảng **Dim** gồm dim_staff, dim_customer, dim_store, dim_date, dim_product; và một bảng **Fact** gồm fact_rental.
- Bảng **dim_date** được sinh ra bởi các câu lệnh SQL raw, các bảng còn lại được đổ dữ liệu bởi SSIS.
- Bảng **dim_staff** được tải dữ liệu (data loading) từ nguồn vào bảng DIM thông qua **SCD Type 2**, thực hiện trên SSIS. 