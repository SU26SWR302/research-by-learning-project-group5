# Hướng dẫn: Flow Zotero → Overleaf cho nhóm JAEN

> SWD392 – Group 5 – SU26 | Cập nhật: June 2026

LINK OVERLEAF EDIT : https://www.overleaf.com/4497129322htpwwdtqcgfx#3fb35e

LINK OVERLEAF VIEW : https://www.overleaf.com/read/vtkgtzwpbhgp#2c21c0

LINK ZOTERO GROUP : https://www.zotero.org/groups/6586964/jaen-swd392-group5/library

(Bật extension zotero collect papers rồi lưu vào link này)

LINK GITHUB : https://github.com/SU26SWR302/research-by-learning-project-group5

LINK JIRA : https://vaanthanh2005.atlassian.net/jira/software/projects/SCRUM/summary?atlOrigin=eyJpIjoiZDg4NjQ3NTNlZWMwNDg2Nzg2MTVhZmMxNjQ2ZjgwYTgiLCJwIjoiaiJ9

---

## TỔNG QUAN FLOW

```
Google Scholar / Springer
        ↓  (1 click - Zotero Connector)
   Zotero Library
        ↓  (Export → BibTeX)
   references.bib
        ↓  (Upload / sync lên)
   Overleaf Project
        ↓  (\cite{key} trong .tex)
   PDF paper hoàn chỉnh
```

---

## PHẦN 1 — ZOTERO: TÌM VÀ LƯU PAPER

### 1.1 Tìm paper ở đâu?

Dùng các nguồn sau theo thứ tự ưu tiên:

| Nguồn                   | Link                | Ưu điểm                     |
| ----------------------- | ------------------- | --------------------------- |
| **Google Scholar**      | scholar.google.com  | Tìm nhanh, bao quát         |
| **Springer**            | link.springer.com   | Paper LNCS/CCIS chính thống |
| **IEEE Xplore**         | ieeexplore.ieee.org | Mảng kỹ thuật, AI           |
| **ACM Digital Library** | dl.acm.org          | CS research                 |
| **Semantic Scholar**    | semanticscholar.org | Có PDF miễn phí nhiều       |
| **arXiv**               | arxiv.org           | Preprint mới nhất           |

**Từ khóa gợi ý cho paper JAEN:**

```
automated essay scoring deep learning
automated speaking assessment LLM
AI language assessment feedback generation
GPT writing evaluation education
automatic speech recognition language learning
e-learning platform AI assessment
prompt engineering LLM evaluation
```

---

### 1.2 Lưu paper bằng Zotero Connector (1 click)

**Bước 1:** Mở trang paper trên trình duyệt  
(vd: trang Google Scholar, trang Springer của paper đó)

**Bước 2:** Bấm icon **Zotero** trên thanh toolbar Chrome  
→ Zotero tự nhận diện metadata (tên tác giả, năm, journal, DOI)  
→ Paper được lưu vào thư viện ngay lập tức

> ⚠️ Nếu Connector không nhận → vào trang paper gốc (không phải Google Scholar)  
> hoặc dùng "Add by DOI" trong Zotero Desktop

**Bước 3:** Kiểm tra trong Zotero Desktop  
→ Mở thư mục collection **"JAEN Paper"** (tạo riêng cho dự án)  
→ Xác nhận đủ: Title, Author, Year, Journal/Conference, DOI

---

### 1.3 Tổ chức thư viện Zotero

Tạo cấu trúc collection như sau:

```
My Library/
└── JAEN - SWD392/
    ├── 1. AI Assessment
    ├── 2. Automated Essay Scoring
    ├── 3. Speaking Assessment / ASR
    ├── 4. E-Learning Platforms
    └── 5. LLM & Prompt Engineering
```

**Cách tạo:** Chuột phải vào "My Library" → "New Collection"

---

### 1.4 Export ra file .bib (để dùng trong Overleaf)

**Khi cần cập nhật references.bib:**

1. Chọn collection **"JAEN - SWD392"** (hoặc chọn tất cả paper)
2. Chuột phải → **"Export Collection..."**
3. Format: chọn **BibTeX**
4. ✅ Tick **"Export Notes"** nếu muốn giữ ghi chú
5. Lưu file tên: `references.bib`
6. Upload lên Overleaf (xem Phần 2)

> 💡 **Mẹo:** Zotero tự sinh **citation key** theo format `TacGia_Nam`  
> Vd: `Radford_2022`, `Brown_2020`  
> Đây chính là key bạn dùng khi `\cite{Radford_2022}` trong LaTeX

---

## PHẦN 2 — OVERLEAF: VIẾT VÀ COMPILE PAPER

### 2.1 Truy cập project nhóm

Link Overleaf nhóm: https://www.overleaf.com/read/rdfyhdcmtfnm#0aeaa9

> Nếu chỉ có quyền **read**, nhờ Leader (Vân Thanh) share link **edit**

---

### 2.2 Cấu trúc file cần biết

```
main.tex          ← ĐỪNG SỬA trừ khi là Leader
sections/
  abstract.tex    ← Vân Thanh
  introduction.tex ← Lê Đức Sự
  related_work.tex ← Lê Viết Mạnh
  method.tex       ← Hoàng Thủy Nguyên
  experiment.tex   ← Huỳnh Tấn Vinh
  conclusion.tex   ← Vân Thanh
references.bib    ← Huỳnh Tấn Vinh cập nhật chính
figures/          ← Ảnh/biểu đồ
```

**Nguyên tắc vàng:** Mỗi người chỉ mở và sửa file của mình.

---

### 2.3 Upload references.bib lên Overleaf

Sau khi export từ Zotero:

1. Vào Overleaf project
2. Bấm icon **upload** (mũi tên lên) ở cột File Tree bên trái
3. Chọn file `references.bib` vừa export
4. Overleaf hỏi "File already exists, overwrite?" → bấm **Overwrite**
5. Bấm **Recompile** để kiểm tra

---

### 2.4 Cách cite tài liệu trong bài viết

Sau khi `references.bib` đã có trong project, cite trong file `.tex` như sau:

```latex
% Cite 1 paper
AI assessment has shown promising results~\cite{Radford_2022}.

% Cite nhiều paper cùng lúc
Several studies~\cite{Brown_2020, Vaswani_2017, Liu_2023} demonstrate...

% Cite tên tác giả tự nhiên trong câu
\citeauthor{Brown_2020} propose a method that...
```

> 💡 Overleaf có **autocomplete**: gõ `\cite{` rồi chờ 1 giây  
> → Overleaf gợi ý danh sách key từ references.bib của bạn

---

### 2.5 Viết nội dung trong file .tex của mình

**Cấu trúc cơ bản một section:**

```latex
\section{Introduction}

Đây là đoạn văn đầu tiên. Không cần indent, LaTeX tự căn chỉnh.

Đây là đoạn văn thứ hai. Để xuống dòng mới thì để trống 1 dòng.

\subsection{Background}

Nội dung subsection ở đây~\cite{key}.

\subsubsection{Specific Topic}

Nội dung subsubsection (không được đánh số, chỉ in đậm).
```

**Các lệnh hay dùng:**

```latex
% In đậm
\textbf{từ quan trọng}

% In nghiêng
\textit{thuật ngữ kỹ thuật}

% Danh sách có số
\begin{enumerate}
    \item Mục thứ nhất
    \item Mục thứ hai
\end{enumerate}

% Danh sách không số
\begin{itemize}
    \item Điểm thứ nhất
    \item Điểm thứ hai
\end{itemize}

% Chèn hình ảnh
\begin{figure}[t]
    \centering
    \includegraphics[width=0.8\textwidth]{figures/ten_hinh.png}
    \caption{Mô tả hình}
    \label{fig:ten_nhan}
\end{figure}

% Refer đến hình trong bài
như được minh họa trong Hình~\ref{fig:ten_nhan}

% Bảng đơn giản
\begin{table}[t]
    \caption{Tiêu đề bảng (đặt TRÊN bảng theo chuẩn Springer)}
    \centering
    \begin{tabular}{lcc}
    \hline
    Method & Accuracy & F1 \\
    \hline
    Baseline & 0.75 & 0.72 \\
    JAEN (Ours) & 0.89 & 0.87 \\
    \hline
    \end{tabular}
    \label{tab:results}
\end{table}
```

---

### 2.6 Compile và kiểm tra lỗi

**Compile:**

- Mở file `main.tex`
- Bấm nút **Recompile** (hoặc Ctrl+Enter)
- PDF hiển thị bên phải

**Đọc lỗi khi compile fail:**

- Lỗi hiện ở tab **Logs & output** phía dưới
- Dòng lỗi có dạng: `! Undefined control sequence` hoặc `! Missing $ inserted`
- Lỗi thường gặp và cách sửa:

| Lỗi                          | Nguyên nhân                             | Cách sửa                               |
| ---------------------------- | --------------------------------------- | -------------------------------------- |
| `Undefined control sequence` | Gõ sai lệnh LaTeX                       | Kiểm tra chính tả lệnh                 |
| `Citation key not found`     | Key trong `\cite{}` không có trong .bib | Kiểm tra key trong references.bib      |
| `File not found`             | Tên file hình ảnh sai                   | Kiểm tra tên file trong `figures/`     |
| `Missing $ inserted`         | Có ký tự đặc biệt chưa escape           | Thêm `\` trước: `\_`, `\%`, `\&`, `\#` |

---

### 2.7 Các ký tự đặc biệt cần escape trong LaTeX

Những ký tự này có ý nghĩa đặc biệt trong LaTeX, phải thêm `\` phía trước:

```latex
% SAI              % ĐÚNG
100%          →    100\%
A & B         →    A \& B
file_name     →    file\_name
#hashtag      →    \#hashtag
$dollar       →    \$dollar
{ }           →    \{ \}
```

---

## PHẦN 3 — QUY TRÌNH LÀM VIỆC HÀNG NGÀY

### Flow chuẩn mỗi khi ngồi viết:

```
1. Mở Zotero → Tìm thêm paper liên quan đến phần mình viết
2. Lưu paper bằng Zotero Connector
3. Export .bib → Upload lên Overleaf (nếu có paper mới)
4. Mở Overleaf → vào đúng file .tex của mình
5. Viết nội dung, cite bằng \cite{key}
6. Bấm Recompile → kiểm tra PDF
7. Nếu lỗi → đọc Logs → sửa
8. Báo nhóm khi xong 1 đoạn lớn
```

---

## PHẦN 4 — CHECKLIST TRƯỚC KHI NỘP

- [ ] Compile thành công, không có lỗi đỏ
- [ ] Tất cả `\cite{}` đều có trong references.bib
- [ ] Tất cả `\ref{}` đều có label tương ứng
- [ ] Không còn dòng `TODO` nào trong file
- [ ] Abstract đủ 150–250 từ
- [ ] Keywords có 5–7 từ khóa
- [ ] Tên tác giả và email đã điền đúng trong main.tex
- [ ] Hình ảnh có caption và được cite trong bài
- [ ] References đủ ít nhất 15–20 paper

---

## PHỤ LỤC — PHÍM TẮT HỮU ÍCH

| Tác vụ                               | Phím tắt                |
| ------------------------------------ | ----------------------- |
| Compile                              | `Ctrl + Enter`          |
| Comment/Uncomment dòng               | `Ctrl + /`              |
| Tìm & thay thế                       | `Ctrl + H`              |
| Autocomplete cite                    | Gõ `\cite{` rồi chờ     |
| Xem PDF tương ứng với dòng đang viết | `Ctrl + Click` vào text |
| Từ PDF nhảy về dòng tex              | `Ctrl + Click` vào PDF  |

---

_Tài liệu này do nhóm JAEN – SWD392 Group 5 biên soạn | June 2026_
