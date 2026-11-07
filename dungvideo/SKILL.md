---
name: dungvideo
description: "Dựng video dọc 9:16 (TikTok, Reels, Shorts) tự động từ A đến Z từ MỘT video quay người nói hoặc MỘT file giọng đọc: nghe lời, cắt chỗ vấp và khoảng lặng, tự chọn hiệu ứng keyword cho từng câu (62 hiệu ứng có code), tự viết nội dung hiệu ứng, phụ đề, nhạc nền, âm thanh, ảnh bìa, render MP4. Lệnh gọi tắt của mrtkeyword. Dùng khi người dùng gọi /dungvideo, $dungvideo, 'dựng video này', 'dựng video'."
---

# /dungvideo — Tự dựng video dọc 9:16 tự động (Bí danh của mrtkeyword)

Skill này là bí danh (alias) rút gọn của **mrtkeyword** giúp bạn gọi lệnh nhanh qua `/dungvideo` hoặc `$dungvideo`.

## Hướng dẫn thực thi

Mọi mã nguồn script, mô hình AI và template dựng video nằm trong thư mục:
- **Thư mục công cụ chính (SK):** `/Users/hoangdam/mrtkeyword/mrtkeyword`
- **Môi trường Python:** `/Users/hoangdam/mrtkeyword/mrtkeyword/tools/.venv/bin/python`
- **Tài liệu quy trình chi tiết:** Đọc trực tiếp file `/Users/hoangdam/mrtkeyword/mrtkeyword/SKILL.md`

Agent hãy thực hiện theo đúng 7 bước được định nghĩa trong `/Users/hoangdam/mrtkeyword/mrtkeyword/SKILL.md`:
1. **Chuẩn bị đầu vào**: `prep_input.py`
2. **Gợi ý keyword**: `suggest.py`
3. **Hoàn thiện kế hoạch**: tạo `work/plan.json` theo đúng lời thoại
4. **Nguyên liệu**: `prepare_assets.py` (tách người, nhạc nền ducking)
5. **Dữ liệu + SFX**: `build_data.py` & `sfx_plan.py`
6. **Kiểm ảnh tĩnh**: `npx remotion still`
7. **Render & giao file**: Xuất thành phẩm vào `~/Movies/Keyword FX/Thanh pham/` kèm tiêu đề, caption Facebook và TikTok.
