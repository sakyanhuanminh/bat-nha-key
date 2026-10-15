# Bảng âm đọc Hán Nôm của Bát Nhã Key — bản 1.3.0

Tệp `bat-nha-key-am-doc.tsv` là **bảng dữ liệu đã chuyển thể** mà bộ gõ
[Bát Nhã Key](https://khonghoa.vn/projects/bat-nha-key/) dùng: **39254 dòng**, mỗi dòng là
một âm đọc của một chữ (hoặc một cụm). Từ điển trong bộ gõ có 76176 dòng; phần không có ở
đây được kể rõ ở mục *Những gì không có trong bảng này*.

Công bố tệp này là **nghĩa vụ của giấy phép**: dữ liệu của Hội Nghiên cứu và Ứng dụng Hán Nôm
mang điều khoản *Chia sẻ tương tự*, buộc phần đã sửa đổi phải được phát hành theo cùng giấy phép.

## Giấy phép

**CC BY-NC-SA 4.0** — Ghi công · Phi thương mại · Chia sẻ tương tự
<https://creativecommons.org/licenses/by-nc-sa/4.0/deed.vi>

Bạn được chép, chia sẻ và sửa đổi tệp này, với ba điều kiện: **ghi công** (xem phần dưới),
**không dùng vào mục đích thương mại**, và **chia sẻ phần đã sửa theo cùng giấy phép này**.

## Ghi công

Bảng này ghép và chuyển thể từ:

| Nguồn | Cột `nguon` | Giấy phép |
|---|---|---|
| **Bộ gõ Hán Nôm Uy-xơn** — Keepout2010 và 学习之云, [Hội Nghiên cứu và Ứng dụng Hán Nôm](https://www.hannom-rcv.org) | `hannom-rcv` | CC BY-NC-SA 4.0 |
| **Hán Việt tự điển** — Thiều Chửu (Nguyễn Hữu Kha), Đuốc Tuệ 1942; bản số hoá [catusf/tudien](https://github.com/catusf/tudien); hiệu đính Đặng Thế Kiệt, Lê Văn Đặng, Nguyễn Hữu Vinh | `thieuchuu-readings` | Hết bản quyền tại VN; bản số hoá CC0 1.0 |
| **Hán Việt – Pinyin wordlist** — [Phong Phan](https://github.com/ph0ngp/hanviet-pinyin-wordlist) | `hanviet-ph0ngp` | MIT |
| **Unicode Unihan Database** (`kVietnamese`, `kIRG_VSource`) | `unihan-vietnamese` | Unicode License v3 |

Số dòng theo nguồn (đếm trên chính tệp này):

| Nguồn (`nguon`) | Số dòng trong bảng |
|---|---:|
| `hannom-rcv` | 21360 |
| `hanviet-ph0ngp` | 11288 |
| `thieuchuu-readings` | 2430 |
| `unihan-vietnamese` | 4176 |

## Những gì **không** có trong bảng này

| Lớp | Số dòng trong từ điển của bộ gõ | Vì sao không có trong bảng |
|---|---:|---|
| `thivien` | 5354 | Thi Viện cho phép DÙNG chữ và âm trong bộ gõ (thư 13-10-2026), không cho công bố lại danh sách của họ |
| `chunom-org` | 29374 | chunom.org không công bố giấy phép nào — dùng trong bộ gõ với ba điều tự ràng buộc, không phát hành lại dữ liệu của họ |
| `bnk-buddhist` | 1883 | thuật ngữ Phật học do Không Hoa biên soạn — tác phẩm riêng của tác giả, không phải phần chuyển thể từ nguồn CC BY-NC-SA |
| `bnk-bien-the` | 311 | lối đọc song hành của chính các thuật ngữ Phật học ấy (ví dụ Kim cương kinh → Kim cang kinh) — cùng là phần riêng của tác giả, đi theo lớp `bnk-buddhist` |

Ngoài ra không có:

* **Cột pinyin.** Nó suy từ CC-CEDICT, giấy phép **CC BY-SA 4.0** — bản không có điều khoản
  Phi thương mại. Trộn dữ liệu BY-SA vào một bản phát hành BY-NC-SA là tự thêm một hạn chế mà
  BY-SA cấm thêm, nên cột ấy phải ở ngoài.
* **Cột nghĩa** (Thiều Chửu, tiếng Anh, nghĩa máy soạn) — bỏ cho gọn.

## Các cột

| Cột | Nghĩa |
|---|---|
| `chu` | chữ Hán hoặc chữ Nôm (một chữ, hoặc một cụm nhiều chữ) |
| `he_chu` | `hanviet` = tra bằng âm Hán–Việt · `nom` = tra bằng âm Nôm |
| `am_doc` | âm đọc, đủ dấu thanh |
| `nguon` | nguồn của chính dòng ấy — dùng cột này để lọc theo nguồn |
| `trong_so` | điểm xếp hạng của Bát Nhã Key, 0–100 (càng cao càng hiện sớm) |
| `co_nhan` | `1` = nguồn ghi rõ đây là âm Hán–Việt hay âm Nôm. **Mọi dòng trong bảng này đều là `1`** |
| `kho_chu_VN` | `1` = chữ thuộc kho chữ Việt Nam của Unicode (`kIRG_VSource`) |

## Không có dòng nào là âm đoán

Nguồn của Hội có 17.100 dòng mà chính họ đánh dấu *không chuẩn hoặc không thông dụng* và **không
nói là âm Hán–Việt hay âm Nôm**. Bát Nhã Key đã thử phân loại bằng máy, đọc tay 45 dòng mẫu để
kiểm, thấy khoảng một phần ba sai theo cả hai chiều — và **bỏ hẳn cả lớp ấy**. Bảng này vì vậy
chỉ chứa những âm mà một nguồn khẳng định rõ thuộc hệ chữ nào. Ai muốn phần bị bỏ thì lấy thẳng
từ nguồn gốc của Hội.

---

© dữ liệu thuộc các nguồn ghi ở trên; phần chuyển thể © 2026 Không Hoa — khonghoa.vn,
phát hành theo CC BY-NC-SA 4.0.