# Dữ liệu tập 2: nguồn và giấy phép

Tạo ngày 22/11/2026. Bộ ảnh nằm ở `du-lieu/` và đóng gói thành `du-lieu.zip` (3.933.577 byte, 112 file). Notebook tải zip từ `https://raw.githubusercontent.com/ngocnguyen88/AI-from-Zero/main/tap02/du-lieu.zip`, nên trước khi đăng phải chép `du-lieu.zip` (và tap02.ipynb, DU-LIEU.md) vào `repo-github/tap02/` rồi đẩy lên. CHƯA đẩy.

## Cấu trúc

| Thư mục | Số ảnh | Nguồn |
|---|---|---|
| du-lieu/100-anh/mat-truoc | 33 | Tự vẽ: THẺ MẪU mặt trước (sinh_the.py, hạt giống 2026) |
| du-lieu/100-anh/mat-sau | 33 | Tự vẽ: THẺ MẪU mặt sau (sinh_the.py) |
| du-lieu/100-anh/khong-phai-the | 34 | Ảnh chụp thật từ Wikimedia Commons, chỉ lấy CC0 / phạm vi công cộng / CC BY (bảng dưới) |
| du-lieu/anh-kho | 12 | 8 thẻ tự vẽ ở kiểu khó (xoay, tối, nhỏ trên bàn, bị che), 1 thẻ của tập 1 (the-mau-tap1.png = tap01/anh/the-mau.png), 3 ảnh phong bì Wikimedia Commons CC0 |

## Thẻ mẫu tự vẽ

- Không phải giấy tờ thật: thông tin bịa (họ tên kiểu "NGUYỄN VĂN MẪU", số bắt đầu bằng 0000000), chữ "THẺ MẪU" và dấu "MẪU" đỏ chéo trên cả hai mặt, không quốc huy, không theo mẫu căn cước thật. Ô vuông kiểu mã QR ở mặt sau là ô ngẫu nhiên, không mã hoá gì. 3 dòng ký tự máy đọc là chữ giả ("IDMAU...").
- Vẽ bằng `sinh_the.py` (Pillow), chạy lại ra đúng bộ ảnh này: `python sinh_the.py <thư mục font> <thư mục nền> du-lieu`. Font Be Vietnam Pro và JetBrains Mono (cả hai SIL Open Font License 1.1, lấy từ `../thu-1-phut/canh/fonts/`). Nền ảnh khó: 2 ảnh "(nền)" ở bảng dưới.
- Ảnh tự vẽ: kênh tự tạo, phát hành cùng repo theo MIT như code (đề xuất; chủ quyết khi đẩy repo).
- Ảnh học: thẻ gần ngay ngắn (lệch tối đa 6 độ), chiếm khoảng 55-70% bề ngang, nền màu trơn có vân nhẹ, 480x360. Ảnh khó cố tình khác ảnh học: xoay 90 / 180 / 35 độ, tối còn 30%, thẻ nhỏ (130 px) đặt trên ảnh chụp bàn, nửa thẻ bị tờ giấy che.

## Ảnh chụp từ Wikimedia Commons

Tải bản thu nhỏ 480 px qua API Commons ngày 22/11/2026, lọc giấy phép ngay lúc tải (chỉ nhận CC0, Public domain, CC BY; không nhận CC BY-SA để khỏi ràng buộc chia sẻ tương tự). Thay đổi đã làm: thu nhỏ và cắt giữa về 480x360, lưu JPEG chất lượng 90. Bỏ các ảnh có người nhận diện được, ảnh quân sự / điều tra, ảnh ví có thể chứa thẻ.
Ảnh CC BY: phải ghi tác giả như cột dưới khi dùng lại (mô tả repo / video ghi "ảnh: Wikimedia Commons, xem tap02/DU-LIEU.md").

| File trong bộ | Tên gốc trên Commons | Tác giả | Giấy phép | Trang gốc |
|---|---|---|---|---|
| 100-anh/khong-phai-the/khac-01.jpg | Tiệm153+xeĐạp&cây.jpg | Thong Vo, Titi Wanderer | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Ti%E1%BB%87m153%2Bxe%C4%90%E1%BA%A1p%26c%C3%A2y.jpg |
| 100-anh/khong-phai-the/khac-02.jpg | Road in Tan Vinh Commune of Luong Son District.jpg | Obakeneko | CC BY 3.0 (https://creativecommons.org/licenses/by/3.0/) | https://commons.wikimedia.org/wiki/File:Road_in_Tan_Vinh_Commune_of_Luong_Son_District.jpg |
| 100-anh/khong-phai-the/khac-03.jpg | Xe đạp ơi - 271220092455.jpg | Newone | CC BY 3.0 (https://creativecommons.org/licenses/by/3.0/) | https://commons.wikimedia.org/wiki/File:Xe_%C4%91%E1%BA%A1p_%C6%A1i_-_271220092455.jpg |
| 100-anh/khong-phai-the/khac-04.jpg | Aaron Burden 2016-12-28 (Unsplash).jpg | Aaron Burden aaronburden | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Aaron_Burden_2016-12-28_(Unsplash).jpg |
| 100-anh/khong-phai-the/khac-05.jpg | Antique-books-woodward.jpg | Liam Quin | Public domain | https://commons.wikimedia.org/wiki/File:Antique-books-woodward.jpg |
| 100-anh/khong-phai-the/khac-06.jpg | 19th century tea- and coffee-cups anaglyph.jpg | Koperczak | Public domain | https://commons.wikimedia.org/wiki/File:19th_century_tea-_and_coffee-cups_anaglyph.jpg |
| 100-anh/khong-phai-the/khac-07.jpg | 9494Coffee cups of the Philippines.jpg | Judgefloro | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:9494Coffee_cups_of_the_Philippines.jpg |
| 100-anh/khong-phai-the/khac-08.jpg | Afternoon Coffee.jpg | tritra tralala | Public domain | https://commons.wikimedia.org/wiki/File:Afternoon_Coffee.jpg |
| 100-anh/khong-phai-the/khac-09.jpg | Albert computer keyboard front.JPG | Snuci | Public domain | https://commons.wikimedia.org/wiki/File:Albert_computer_keyboard_front.JPG |
| 100-anh/khong-phai-the/khac-10.jpg | Amtelco Unified keyboard top.jpg | snuci | Public domain | https://commons.wikimedia.org/wiki/File:Amtelco_Unified_keyboard_top.jpg |
| 100-anh/khong-phai-the/khac-11.jpg | DG 東莞 DongGuan 南城區 Nancheng 鴻福路 HongFu Road 東莞京東商場 JD Shopping Mall Electronics Showroom December 2024 R12S 22 Keyboards.jpg | NAS 238 WMMNO | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:DG_%E6%9D%B1%E8%8E%9E_DongGuan_%E5%8D%97%E5%9F%8E%E5%8D%80_Nancheng_%E9%B4%BB%E7%A6%8F%E8%B7%AF_HongFu_Road_%E6%9D%B1%E8%8E%9E%E4%BA%AC%E6%9D%B1%E5%95%86%E5%A0%B4_JD_Shopping_Mall_Electronics_Showroom_December_2024_R12S_22_Keyboards.jpg |
| 100-anh/khong-phai-the/khac-12.jpg | 031 Theresianism Style - Interiors.jpg | Scan and postprocessing by Hubertl | Public domain | https://commons.wikimedia.org/wiki/File:031_Theresianism_Style_-_Interiors.jpg |
| 100-anh/khong-phai-the/khac-13.jpg | 082 Josepinism Style Furniture.jpg | Scan and postprocessing by Hubertl | Public domain | https://commons.wikimedia.org/wiki/File:082_Josepinism_Style_Furniture.jpg |
| 100-anh/khong-phai-the/khac-14.jpg | A fresh, ripe Pineapple.jpg | VickyOmondi | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:A_fresh,_ripe_Pineapple.jpg |
| 100-anh/khong-phai-the/khac-15.jpg | Andrew Branch 2017-05-25 (Unsplash 8F73TXwfttU).jpg | Andrew Branch denae_andrew | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Andrew_Branch_2017-05-25_(Unsplash_8F73TXwfttU).jpg |
| 100-anh/khong-phai-the/khac-16.jpg | 20250710 Fruits at the market in Khimki (28842).jpg | SergeyA-Russia (người tải lên, ghi "Own work") | CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/) | https://commons.wikimedia.org/wiki/File:20250710_Fruits_at_the_market_in_Khimki_(28842).jpg |
| 100-anh/khong-phai-the/khac-17.jpg | Achimenes cettoana in cultivation.jpg | SiGarb | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Achimenes_cettoana_in_cultivation.jpg |
| 100-anh/khong-phai-the/khac-18.jpg | Achimenes pedunculata in cultivation.jpg | SiGarb | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Achimenes_pedunculata_in_cultivation.jpg |
| 100-anh/khong-phai-the/khac-19.jpg | Debian Swirl Logo coded for Debian Day 2025.jpg | Aman03062006 | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Debian_Swirl_Logo_coded_for_Debian_Day_2025.jpg |
| 100-anh/khong-phai-the/khac-20.jpg | Dell Latitude 7400 Keyboard.jpg | Jackedak | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Dell_Latitude_7400_Keyboard.jpg |
| 100-anh/khong-phai-the/khac-21.jpg | 2015-365-19 It is Time to Write (16323898735).jpg | cogdogblog | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:2015-365-19_It_is_Time_to_Write_(16323898735).jpg |
| 100-anh/khong-phai-the/khac-22.jpg | A pen writing "Example".jpg | Jiafei Slay Queen | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:A_pen_writing_%22Example%22.jpg |
| 100-anh/khong-phai-the/khac-23.jpg | A simple sketch on a TWA napkin by NASA Dryden engineer Frank W "Bill" Burcham led to development and validation of the Propulsion-Controlled Aircraft concept (EC94-42805-1).jpg | NASA Armstrong Flight Research Center / NASA/Dennis Taylor | Public domain | https://commons.wikimedia.org/wiki/File:A_simple_sketch_on_a_TWA_napkin_by_NASA_Dryden_engineer_Frank_W_%22Bill%22_Burcham_led_to_development_and_validation_of_the_Propulsion-Controlled_Aircraft_concept_(EC94-42805-1).jpg |
| 100-anh/khong-phai-the/khac-24.jpg | Ambérieu-en-Bugey en janvier 2018 - 4.JPG | Benoît Prieur | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Amb%C3%A9rieu-en-Bugey_en_janvier_2018_-_4.JPG |
| 100-anh/khong-phai-the/khac-25.jpg | 11-11-11 11-11 example.jpg | Nad at English Wikipedia | Public domain | https://commons.wikimedia.org/wiki/File:11-11-11_11-11_example.jpg |
| 100-anh/khong-phai-the/khac-26.jpg | 1868 to 1872 School Revenue in Bulletin of Kentucky Department of Education v.7, no. 4.jpg | Barksdale Hamlett | Public domain | https://commons.wikimedia.org/wiki/File:1868_to_1872_School_Revenue_in_Bulletin_of_Kentucky_Department_of_Education_v.7,_no._4.jpg |
| 100-anh/khong-phai-the/khac-27.jpg | 1894-11-12 Goodyear India Rubber Glove Manufacturing Company receipt.jpg | không rõ tác giả | Public domain | https://commons.wikimedia.org/wiki/File:1894-11-12_Goodyear_India_Rubber_Glove_Manufacturing_Company_receipt.jpg |
| 100-anh/khong-phai-the/khac-28.jpg | 2007.08.15.Kassazettel.WienerWasser.JPG | Anton-kurt at German Wikipedia | Public domain | https://commons.wikimedia.org/wiki/File:2007.08.15.Kassazettel.WienerWasser.JPG |
| 100-anh/khong-phai-the/khac-29.jpg | 21 MDS offers virtual appointments (3713414).jpeg | U.S. Space Force image by 2nd Lt. Scarlett Trujillo | Public domain | https://commons.wikimedia.org/wiki/File:21_MDS_offers_virtual_appointments_(3713414).jpeg |
| 100-anh/khong-phai-the/khac-30.jpg | Acoustic sensor technology tested at Ramstein AB (8565998).jpg | U.S. Air Force photo by Airman 1st Class Tabatha Chapman | Public domain | https://commons.wikimedia.org/wiki/File:Acoustic_sensor_technology_tested_at_Ramstein_AB_(8565998).jpg |
| 100-anh/khong-phai-the/khac-31.jpg | -087 365- ibokeh (3900140178).jpg | Leland Francisco from Dededo, Guam | CC BY 2.0 (https://creativecommons.org/licenses/by/2.0/) | https://commons.wikimedia.org/wiki/File:-087_365-_ibokeh_(3900140178).jpg |
| 100-anh/khong-phai-the/khac-32.jpg | Banhcanhcua.jpg | bánh canh cu | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Banhcanhcua.jpg |
| 100-anh/khong-phai-the/khac-33.jpg | Saigon Street Corner Dining (at noon).jpg | Alan Turkus from Hopewell, New Jersey, USA | CC BY 2.0 (https://creativecommons.org/licenses/by/2.0/) | https://commons.wikimedia.org/wiki/File:Saigon_Street_Corner_Dining_(at_noon).jpg |
| 100-anh/khong-phai-the/khac-34.jpg | Street vendor pho ga Hanoi.jpg | Original uploaded by Schellack (Transfered by Alison) | CC BY 3.0 (https://creativecommons.org/licenses/by/3.0/) | https://commons.wikimedia.org/wiki/File:Street_vendor_pho_ga_Hanoi.jpg |
| anh-kho/phong-bi-1.jpg | Eddie ó Neil Record Sleeve APR 7 1945.jpg | Back ache | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Eddie_%C3%B3_Neil_Record_Sleeve_APR_7_1945.jpg |
| anh-kho/phong-bi-2.jpg | Letter pro.jpg | Jotahin | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Letter_pro.jpg |
| anh-kho/phong-bi-3.jpg | Starcraft cheat.jpg | Ninoeil | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Starcraft_cheat.jpg |
| (nền) ban.jpg | Always, Together (Unsplash).jpg | Takahiro Sakamoto takahiro | CC0 (https://creativecommons.org/publicdomain/zero/1.0/) | https://commons.wikimedia.org/wiki/File:Always,_Together_(Unsplash).jpg |
| (nền) ban2.jpg | A clear glass of water sits next to a laptop.jpg | Shixart1985 | CC BY 2.0 (https://creativecommons.org/licenses/by/2.0/) | https://commons.wikimedia.org/wiki/File:A_clear_glass_of_water_sits_next_to_a_laptop.jpg |

Hai ảnh "(nền)" không nằm trong bộ; chỉ dùng làm nền cho `anh-kho/truoc-nho-tren-ban.jpg` (nền ban.jpg, CC0) và `anh-kho/sau-nho-tren-ban.jpg` (nền ban2.jpg, CC BY 2.0, tác giả Shixart1985; ảnh ghép đã thu nhỏ, cắt, dán thẻ mẫu lên).

## Mô hình

ResNet-18, trọng số `ResNet18_Weights.IMAGENET1K_V1` của torchvision (thư viện BSD-3-Clause), như tập 1. Trọng số học trên ImageNet-1k; điều khoản ImageNet chưa đối chiếu (đã ghi ở tap01/SO-DO.md).
