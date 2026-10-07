# Hadoop Ecommerce Lab

## 1. Giới thiệu

Bài thực hành triển khai Apache Hadoop Streaming trên Google Colab để phân tích dữ liệu đơn hàng thương mại điện tử.

Mục tiêu của bài là tính tổng doanh thu theo từng nhóm sản phẩm (category), trong đó chỉ tính các giao dịch có trạng thái `SUCCESS`.

Quy trình xử lý:

CSV → Mapper → Shuffle/Sort → Reducer → Output → Top 3

---

## 2. Môi trường thực hiện

- Google Colab
- Python
- Apache Hadoop 3.3.6
- Hadoop Streaming
- HDFS
- Dữ liệu: `orders_2026_09.csv`

---

## 3. Các file trong bài

```text
Hadoop_Ecommerce_Lab/
│
├── README.md
├── Bao_cao_Hadoop.docx
├── mapper_revenue.py
├── reducer_revenue.py
├── part-00000
├── orders_2026_09.csv
│
└── Anh_chup/
    ├── 01_hadoop_version.png
    ├── 02_hdfs_running.png
    ├── 03_hdfs_input.png
    ├── 04_mapper_reducer.png
    ├── 05_pipeline_test.png
    ├── 06_hadoop_streaming.png
    ├── 07_part00000.png
    └── 08_top3.png