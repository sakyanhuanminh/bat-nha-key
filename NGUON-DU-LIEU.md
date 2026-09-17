# Nguồn dữ liệu và giấy phép — Bát Nhã Key

```
Từ điển lexicon.sqlite trong app này ghép từ các nguồn mở sau. Mã nguồn app là phần mềm đóng,
miễn phí; phần DỮ LIỆU mang giấy phép của từng nguồn như ghi dưới đây.

1. CC-CEDICT — Community maintained free Chinese-English dictionary. Published by MDBG.
   https://www.mdbg.net/chinese/dictionary?page=cc-cedict
   Giấy phép: Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)
   https://creativecommons.org/licenses/by-sa/4.0/
   Tham chiếu: CEDICT © 1997–1998 Paul Andrew Denisowski.
   Dùng để suy cột `pinyin` (pinyin không dấu thanh) của từ điển. Cột ấy là tác phẩm phái sinh
   ĐÃ SỬA ĐỔI (bỏ dấu thanh, ghép liền âm tiết, áp quy ước Phật học 阿 a / 乘 sheng / 迦葉
   jiashe, thêm bảng ghi đè do chủ dự án duyệt) và được phát hành theo cùng giấy phép CC BY-SA 4.0.

2. Unicode Unihan Database — https://www.unicode.org/charts/unihan.html
   Giấy phép: Unicode License v3 (https://www.unicode.org/license.txt)
   Dùng: kVietnamese (âm Nôm), kMandarin (âm quan thoại), kSimplifiedVariant/kTraditionalVariant,
   kDefinition, kHanyuPinlu (tần suất).

3. Hán Việt – Pinyin wordlist — Phong Phan, https://github.com/ph0ngp/hanviet-pinyin-wordlist
   Giấy phép: MIT © 2024 Phong Phan. Dùng: âm Hán–Việt chữ đơn và pinyin theo từng âm.

4. Hán Việt tự điển — Thiều Chửu (Nguyễn Hữu Kha), Đuốc Tuệ 1942; bản số hoá catusf/tudien
   https://github.com/catusf/tudien — bản in hết hạn bản quyền tại Việt Nam (tác giả mất 1954);
   bản số hoá CC0 1.0. Dùng: nghĩa tiếng Việt.

5. Thuật ngữ Phật học Bát Nhã Key — do Không Hoa biên soạn và duyệt. Sở hữu của
   tác giả.

Bảng `source` bên trong lexicon.sqlite lặp lại các thông tin này để giấy phép đi cùng dữ liệu.
```
