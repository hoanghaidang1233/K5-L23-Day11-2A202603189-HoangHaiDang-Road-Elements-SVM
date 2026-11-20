# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): Nguyễn Thiện Phúc        Người kiểm (học viên): Hoàng Hải Đăng  
Ngày: 20/11/2026                          Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest): `NguyenThienPhuc-front.zip`, `NguyenThienPhuc-fisheye.zip` — revision 1  
Số ảnh kiểm: 6 (A01, A03, A04, A06, A08, B02) (+ 0 ảnh thêm, ghi riêng)   Số nhãn đã kiểm (shape + tag): 88  

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 6 | Không có | Đạt|
| QC1-02 đủ L1, R1 | bỏ sót | 12 | Không có |Đạt |
| QC1-03 position | sai thuộc tính / thừa |Thừa | 1 Lane 74 đang có 2 lane R2| nhẹ  |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 14 | Không có | Đạt |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 14 |  Không có| Đạt |
| QC1-06 style, color, kind | sai thuộc tính | 14 |Không có | Đạt |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 15 |Không có | Đạt|
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 16 | Không có | Đạt |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 29 | Không có | Đạt|
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | Bỏ sót| A01, A03,A06,A08  |Nặng |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 6 | KHông có| Đạt|
| QC1-12 file | lỗi file | 2 | Không có | Đạt |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-03 | A04 | lane, id 74 | nhẹ | Ảnh có 2 lane cùng `position = R2` (thừa một R2) |
| 2 | QC1-10 | A01 | traffic_sign (thiếu) | Nặng | Bỏ sót biển chỉ dẫn xanh nhỏ ở xa, khoảng (432,463)–(452,478) |
| 3 | QC1-10 | A03 | traffic_sign (thiếu) | Nặng | Bỏ sót biển vàng báo trường học, khoảng (1002,285)–(1040,325) |
| 4 | QC1-10 | A03 | traffic_sign (thiếu) | Nặng | Bỏ sót biển cam hình thoi, khoảng (797,315)–(828,345) |
| 5 | QC1-10 | A06 | traffic_sign (thiếu) | Nặng | Bỏ sót biển cam hình thoi dưới gầm cầu, khoảng (563,305)–(590,333) |
| 6 | QC1-10 | A08 | traffic_sign (thiếu) | Nặng | Bỏ sót biển phụ "PASSENGER CARS ONLY" trên biển xanh lớn, khoảng (778,38)–(855,62) |

## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |

## Quyết định
Lỗi nặng: 5   Lỗi chính: 0 / 88 nhãn = 0 %   Lỗi nhẹ: 1   Ca chờ lead: 0  
Quyết định (Release / Hold / Rework): Rework  
Lý do (theo luật của phiếu): Còn 5 lỗi nặng (QC1-10 bỏ sót biển ở A01, A03, A06, A08); có ít nhất một lỗi nặng là Rework.

Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](../docs/qc_severity_road_v1.0.md).
