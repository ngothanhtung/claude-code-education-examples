# Chuyển Động Ma Sát — PixiJS

Mô phỏng tương tác cho Vật lý 10 về lực ma sát nghỉ, lực ma sát trượt và lực ma sát lăn.

## Cách chạy

Mở trực tiếp `chuyen-dong-ma-sat.html` trong trình duyệt, hoặc dùng một web server tĩnh nếu bạn muốn tránh giới hạn khi mở file cục bộ.

Ví dụ với Python:

```bash
python -m http.server 8000
```

Sau đó mở:

```text
http://localhost:8000/chuyen-dong-ma-sat.html
```

## Tính năng

- Chọn chế độ trượt hoặc lăn.
- Điều chỉnh khối lượng, lực tác dụng và các hệ số ma sát.
- Xem trực quan lực tác dụng, lực ma sát và trạng thái chuyển động.
- Chọn các preset để so sánh ba tình huống điển hình.

## Preset mẫu

- `Giữ đứng yên`: lực chưa vượt ngưỡng ma sát nghỉ.
- `Trượt`: lực kéo đủ lớn để vật bắt đầu trượt.
- `Lăn`: dùng ma sát lăn nhỏ để quan sát chuyển động nhẹ hơn.

## Checklist kiểm thử nhanh

1. Mở trang và xác nhận canvas hiển thị bên trái, bảng điều khiển ở bên phải.
2. Chọn preset `Giữ đứng yên` rồi nhấn `Bắt đầu`, vật phải giữ nguyên.
3. Chọn preset `Trượt` rồi nhấn `Bắt đầu`, vật phải tăng tốc và hiện trạng thái trượt.
4. Chọn preset `Lăn` rồi nhấn `Bắt đầu`, vật phải lăn với lực cản nhỏ hơn.
5. Thử kéo thanh lực tác dụng để vượt hoặc không vượt ngưỡng ma sát nghỉ.

## Ghi chú kỹ thuật

- Demo dùng PixiJS v7 được ghim phiên bản để tránh thay đổi hành vi từ CDN `release`.
- Nếu mở trực tiếp bằng `file://` và trình duyệt chặn tài nguyên nào đó, hãy chuyển sang chạy bằng web server cục bộ.
