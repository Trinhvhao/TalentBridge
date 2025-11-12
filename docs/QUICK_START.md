# ⚡ Quick Start - Bài Báo IEEE TalentBridge

## 🎯 Mục Tiêu
Compile bài báo IEEE conference paper về TalentBridge thành PDF để submit.

---

## 📦 Bạn Đã Có Gì?

✅ **TalentBridge_IEEE_Paper.tex** - Bài báo hoàn chỉnh với:
- 8 sections đầy đủ
- 7 diagrams/charts (TikZ + PGFPlots)
- 4 tables kết quả
- 1 algorithm
- 8 references

✅ **4 Guide Files** - Hướng dẫn chi tiết:
- `PAPER_README.md` - Tổng quan
- `LATEX_COMPILE_GUIDE.md` - Compile LaTeX
- `SCREENSHOT_GUIDE.md` - Thêm screenshots
- `FIGURES_AND_DIAGRAMS.md` - Danh sách figures

---

## 🚀 3 Cách Compile (Chọn 1)

### ⭐ Cách 1: Overleaf (EASIEST - Khuyến nghị)

```
1. Truy cập: https://www.overleaf.com
2. Đăng ký/Đăng nhập (free)
3. Click "New Project" → "Upload Project"
4. Upload file: TalentBridge_IEEE_Paper.tex
5. Overleaf tự động compile
6. Click "Download PDF"
```

**Ưu điểm:**
- ✅ Không cần cài đặt gì
- ✅ Tự động compile
- ✅ Xem PDF real-time
- ✅ Dễ share với coauthors

**Thời gian:** 2 phút

---

### 🔧 Cách 2: Local (Windows)

#### Bước 1: Cài MiKTeX
```
1. Download: https://miktex.org/download
2. Chạy installer
3. Chọn "Install missing packages: Yes"
```

#### Bước 2: Compile
```powershell
cd docs
pdflatex TalentBridge_IEEE_Paper.tex
pdflatex TalentBridge_IEEE_Paper.tex
```

**Output:** `TalentBridge_IEEE_Paper.pdf`

**Thời gian:** 10 phút (cài đặt) + 1 phút (compile)

---

### 🍎 Cách 3: Local (Mac)

#### Bước 1: Cài MacTeX
```bash
brew install --cask mactex
```

#### Bước 2: Compile
```bash
cd docs
pdflatex TalentBridge_IEEE_Paper.tex
pdflatex TalentBridge_IEEE_Paper.tex
```

**Thời gian:** 15 phút (cài đặt) + 1 phút (compile)

---

## 📸 Thêm Screenshots (Optional)

### Nếu Muốn Bài Báo Đẹp Hơn:

#### Bước 1: Chụp Screenshots
```bash
# Chạy server
python main.py

# Mở browser và chụp 3 ảnh:
1. http://localhost:9990/cv-analysis.html
   → Upload CV → Chụp interface
   → Save as: cv_analysis_interface.png

2. Sau khi upload CV, click "Việc Làm Phù Hợp"
   → Chụp top 5 jobs với explanations
   → Save as: job_matching_results.png

3. http://localhost:9990/dashboard.html
   → Chụp charts với AI insights
   → Save as: dashboard_analytics.png
```

#### Bước 2: Copy Ảnh
```bash
# Tạo folder
mkdir docs/screenshots

# Copy ảnh (Windows)
copy Downloads\*.png docs\screenshots\

# Copy ảnh (Mac/Linux)
cp ~/Downloads/*.png docs/screenshots/
```

#### Bước 3: Uncomment Code
Mở `TalentBridge_IEEE_Paper.tex`, tìm và bỏ dấu `%`:

```latex
% Line ~430 - Bỏ dấu % ở 6 dòng này:
\begin{figure}[htbp]
\centering
\includegraphics[width=0.48\textwidth]{screenshots/cv_analysis_interface.png}
\caption{CV Analysis Interface showing parsed information and quality scores}
\label{fig:cv_examples}
\end{figure}

% Line ~485 - Bỏ dấu % ở 6 dòng này:
\begin{figure}[htbp]
\centering
\includegraphics[width=0.48\textwidth]{screenshots/job_matching_results.png}
\caption{Job Matching Results with AI-generated explanations and match scores}
\label{fig:job_matching_demo}
\end{figure}
```

#### Bước 4: Compile Lại
```bash
pdflatex TalentBridge_IEEE_Paper.tex
pdflatex TalentBridge_IEEE_Paper.tex
```

**Chi tiết:** Xem `SCREENSHOT_GUIDE.md`

---

## 📊 Kết Quả

### Bài Báo Sẽ Có:

**Pages:** 6-7 pages (IEEE 2-column format)

**Sections:**
1. Abstract + Keywords
2. Introduction
3. Related Work
4. System Architecture (với diagram)
5. Methodology (với flowcharts + algorithm)
6. Implementation
7. Experimental Results (với charts + tables)
8. Discussion
9. Conclusion
10. References

**Visual Elements:**
- 3 TikZ diagrams (Architecture, CV Parsing, Matching)
- 4 PGFPlots charts (Dataset, Accuracy, Ratings, Performance)
- 4 Tables (Parsing, Matching, Performance, Comparison)
- 1 Algorithm (Semantic Matching)
- 3 Screenshots (nếu thêm)

---

## ✅ Checklist

### Trước Khi Submit:
- [ ] PDF compile thành công (no errors)
- [ ] Tất cả figures hiển thị
- [ ] Tất cả tables hiển thị
- [ ] References đúng (no "??")
- [ ] Author info đã update
- [ ] Abstract < 250 words
- [ ] Page count: 6-8 pages
- [ ] Spell check
- [ ] Grammar check

---

## 🆘 Troubleshooting

### Error: "Package not found"
```
→ MiKTeX sẽ tự động hỏi install
→ Click "Install" → "OK"
```

### Error: "File not found" (screenshots)
```
→ Check file path: screenshots/xxx.png
→ Hoặc comment out \includegraphics lines
```

### Warning: "Reference undefined"
```
→ Compile 2 lần:
pdflatex file.tex
pdflatex file.tex
```

### PDF không mở được
```
→ Close PDF reader
→ Compile lại
→ Mở PDF
```

**Chi tiết:** Xem `LATEX_COMPILE_GUIDE.md`

---

## 📚 Đọc Thêm

| File | Nội Dung | Khi Nào Đọc |
|------|----------|-------------|
| `PAPER_README.md` | Tổng quan bài báo | Muốn hiểu structure |
| `LATEX_COMPILE_GUIDE.md` | Compile chi tiết | Gặp lỗi compile |
| `SCREENSHOT_GUIDE.md` | Thêm screenshots | Muốn thêm ảnh demo |
| `FIGURES_AND_DIAGRAMS.md` | Danh sách figures | Muốn sửa charts/diagrams |

---

## 🎯 Recommended Workflow

### Workflow 1: Submit Nhanh (30 phút)
```
1. Upload lên Overleaf (2 phút)
2. Download PDF (1 phút)
3. Review PDF (5 phút)
4. Update author info (2 phút)
5. Compile lại (1 phút)
6. Final check (5 phút)
7. Submit! ✅
```

### Workflow 2: Professional (2 giờ)
```
1. Chụp 3 screenshots (30 phút)
2. Xử lý ảnh (resize, compress) (15 phút)
3. Copy vào docs/screenshots/ (2 phút)
4. Uncomment code trong .tex (5 phút)
5. Compile local hoặc Overleaf (5 phút)
6. Review PDF kỹ (20 phút)
7. Update author, acknowledgments (10 phút)
8. Spell check + Grammar check (20 phút)
9. Final compile (2 phút)
10. Submit! ✅
```

---

## 💡 Tips

### Tip 1: Dùng Overleaf
- Dễ nhất, không cần cài đặt
- Tự động compile
- Dễ share với advisor/coauthors

### Tip 2: Compile 2 Lần
- Lần 1: Tạo .aux files
- Lần 2: Resolve references
- Nếu có bibliography: compile 4 lần

### Tip 3: Screenshots Không Bắt Buộc
- Bài báo vẫn đẹp và đầy đủ không có screenshots
- Có 7 diagrams/charts vẽ bằng TikZ/PGFPlots
- Screenshots chỉ là bonus

### Tip 4: Customize Sau
- Submit version đầu tiên với data mặc định
- Sau đó customize author, data, colors
- Xem `FIGURES_AND_DIAGRAMS.md` để sửa

---

## 🎉 Kết Luận

Bạn đã có:
- ✅ Bài báo IEEE hoàn chỉnh (27KB .tex file)
- ✅ 7 diagrams/charts đẹp
- ✅ 4 tables kết quả
- ✅ 4 guide files chi tiết
- ✅ Sẵn sàng compile và submit

**Next Step:**
1. Chọn 1 trong 3 cách compile ở trên
2. Compile thành PDF
3. Review PDF
4. Submit to conference! 🚀

---

**Good luck! 🍀**

*Nếu cần help, xem các guide files hoặc mở GitHub Issues.*

