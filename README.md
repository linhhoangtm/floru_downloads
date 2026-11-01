# Floru Studio — tệp tải thêm

App Floru Studio tự tải các tệp ở đây khi người dùng bấm cài. Không cần tải tay.

- `vieneu-v2/` — Giọng Việt trên máy, bản đọc được giọng mẫu riêng (nhân bản giọng từ đoạn ghi âm vài giây). App bản mới tải ở đây.
- `vieneu-v1/` — Giọng Việt trên máy (bản đầu, giữ cho app cũ) (công cụ đọc VieNeu-TTS, Apache-2.0). Mã nguồn công cụ: thư mục `tools-python/vieneu_helper` của Floru Studio.
- `depth-v1/` — Ảnh 3D chuyển động (công cụ đo độ sâu ảnh, chạy model Depth-Anything-V2-Small, Apache-2.0). Mã nguồn công cụ: thư mục `tools-python/depth_helper` của Floru Studio.
- `echocoach-phoneme-v1/` — Model chấm phát âm từng âm cho app EchoCoach (chạy trên điện thoại). Gốc: mrrubino/wav2vec2-large-xlsr-53-l2-arctic-phoneme (Apache-2.0), đã chuyển ONNX và nén int8. File zip chia 3 phần (`.001`–`.003`, mỗi phần dưới 100MB); app tải, nối lại, kiểm tra `SHA256SUMS.txt` rồi giải nén.
