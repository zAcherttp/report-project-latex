# UIT Course Project LaTeX Template

Template này đã được chỉnh lại để nhìn giống `Template_Do_An_Mon_Hoc_VN.docx` trong repo tham chiếu:

- Font Times-style (`newtx`)
- Lề trang 2.54 cm
- Bìa có khung đôi màu xanh và logo UIT
- Header trái/phải theo môn học và số nhóm
- Footer số trang căn giữa
- Chương theo dạng `Chương I. ...`
- Mục lục 3 cấp, caption nghiêng ở giữa

## File quan trọng

- `main-report.tex`: file build chính
- `uitcourseproject.cls`: class chứa layout và cover
- `config/project-info.tex`: sửa thông tin đề tài, môn học, nhóm, GVHD
- `config/listings.tex`: style cho code block
- `chapters/`: các file nội dung mẫu
- `bibliography/main.bib`: tài liệu tham khảo mẫu

## Cách dùng

1. Sửa `config/project-info.tex`
2. Thay nội dung các file trong `chapters/`
3. Cập nhật `bibliography/main.bib`
4. Build bằng `latexmk -pdf main-report.tex`

## Ghi chú

- Template hiện tại ưu tiên `pdflatex + biber` để dễ chia sẻ và để giữ bộ gõ tiếng Việt ổn định.
- `latexmk -pdf main-report.tex` là lệnh build nên dùng mặc định vì nó tự chạy đủ các vòng compile cần thiết.
- Trong môi trường hiện tại, binary LaTeX không có sẵn trong `PATH`, nên chưa thể compile để verify trực tiếp.
