<!DOCTYPE html>
<html lang="vi">
<!--
=======================================================================
  HƯỚNG NGHIỆP ALPHA — Công cụ tra cứu tổ hợp môn lớp 10
  Phiên bản: 2.7  |  Ngày: 2026-06-12
  Tác giả: HNA (Trần Văn Đăng) — 096 937 4411
  Website: www.huongnghiepalpha.vn
=======================================================================

  LUỒNG 4 BƯỚC:
    B1. Hiểu mình  → chọn đặc điểm bản thân (20 mô tả Holland+Gardner)
    B2. Nhóm ngành → accordion Sông An style, chọn 1 ngành
    B3. Tổ hợp ĐH  → tổ hợp + trường đúng ngành
    B4. Môn lớp 10 → tìm trường, nhập tổ hợp, chọn môn thi TN, sơ đồ SVG

  CÁCH CẬP NHẬT DỮ LIỆU:
  ─────────────────────────────────────────────────────────────────────
  1. THÊM/SỬA NGÀNH → tìm "const NGANH=[" trong <script>
     Mỗi entry có: id, icon, ten, mo, tomtat, dh[], mon_txt[], 
                   tohop_l10[], truong, warn, traits[]
     - dh[0] phải là tổ hợp CHỦ LỰC của ngành (★ sẽ tự gán)
     - traits[] phải dùng đúng id trong TRAITS[]

  2. THÊM/SỬA TRƯỜNG ĐỒNG NAI → tìm "const ALL_SCHOOLS=["
     Thêm object {ten:'...', tohop:{A00:'...', B00:'...', ...}}

  3. THÊM TỔ HỢP MÔN → tìm "const CHUNG_TABLE=["
     Format: {dh:'X00', mon3:'...', l10:'...', nganh:'...'}

  4. SỬA THÔNG TIN LIÊN HỆ → tìm "096 937 4411" và thay toàn bộ

  5. GẮN GOOGLE FORM → tìm "GOOGLE_FORM_URL" và thay link

  LƯU Ý QUAN TRỌNG:
  ─────────────────────────────────────────────────────────────────────
  - File chạy OFFLINE hoàn toàn (không cần server, không cần internet)
    ngoại trừ font Google (Be Vietnam Pro) — nếu offline thì thêm
    font-family fallback: sans-serif
  - Mọi data đều trong file này, không có file phụ
  - Tương thích: Chrome, Firefox, Safari, Edge — desktop & mobile
  - Để chia sẻ qua Zalo: gửi file .html trực tiếp
    → người nhận mở bằng trình duyệt trên điện thoại/máy tính
  - Để đặt lên website: upload file lên hosting, link trực tiếp

=======================================================================
-->

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tra cứu hướng nghiệp — Hướng Nghiệp Alpha</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --navy:#142768;--navy-light:#1a3490;--amber:#FF9900;--amber-light:#FFF4D8;
  --green:#1a7a1a;--green-light:#eaf4ea;
  --bg:#f7f8fc;--card:#ffffff;--border:#e2e6f0;--border-strong:#c8d0e8;
  --text:#1a1d2e;--text2:#4a5068;--text3:#8892a8;
  --r:10px;--shadow:0 2px 12px rgba(20,39,104,.08);
}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:"Be Vietnam Pro",sans-serif;background:var(--bg);color:var(--text);min-height:100vh}

/* ── HEADER ── */
.hdr{background:var(--navy);padding:0 1.5rem;display:flex;align-items:center;justify-content:space-between;height:56px;position:sticky;top:0;z-index:100}
.hdr-brand{color:white;font-weight:700;font-size:15px;letter-spacing:.02em}
.hdr-sub{color:rgba(255,255,255,.55);font-size:12px;margin-top:1px}
.hdr-contact{color:var(--amber);font-size:12px;font-weight:600;text-decoration:none;display:inline-flex;align-items:center;gap:4px;cursor:pointer}
.hdr-contact:hover{text-decoration:underline}

/* ── MAIN ── */
.main{max-width:760px;margin:0 auto;padding:1.5rem 1rem 3rem}

/* ── HERO ── */
.hero{background:var(--navy);border-radius:var(--r);padding:1.5rem;margin-bottom:1.5rem;color:white}
.hero-tag{font-size:11px;font-weight:600;letter-spacing:.08em;text-transform:uppercase;color:var(--amber);margin-bottom:.5rem}
.hero-title{font-size:22px;font-weight:700;line-height:1.3;margin-bottom:.5rem}
.hero-desc{font-size:13px;color:rgba(255,255,255,.65);line-height:1.6}

/* ── FLOW BAR ── */
.flow{display:flex;align-items:center;gap:0;border-radius:var(--r);overflow:hidden;border:1.5px solid var(--border-strong);margin-bottom:1.25rem;background:var(--card)}
.flow-step{flex:1;padding:10px 4px;text-align:center;font-size:11px;color:var(--text3);border-right:1px solid var(--border);cursor:pointer;transition:all .15s;line-height:1.3}
.flow-step:last-child{border-right:none}
.flow-step .fn{display:block;font-size:17px;font-weight:700;color:var(--border-strong);margin-bottom:2px}
.flow-step.active{background:var(--navy);color:white}
.flow-step.active .fn{color:rgba(255,255,255,.5)}
.flow-step.done{background:var(--green-light);color:var(--green)}
.flow-step.done .fn{color:var(--green)}

/* ── PANELS ── */
.panel{display:none}.panel.show{display:block}

/* ── SECTION LABEL ── */
.slabel{font-size:11px;font-weight:700;letter-spacing:.07em;text-transform:uppercase;color:var(--text3);margin-bottom:.75rem}

/* ── TRAIT GRID ── */
.trait-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(148px,1fr));gap:6px;margin-bottom:.75rem}
.tbtn{border:1.5px solid var(--border);border-radius:8px;padding:9px 10px;cursor:pointer;background:var(--card);text-align:left;font-size:12px;color:var(--text2);transition:all .15s;line-height:1.35;font-family:inherit}
.tbtn:hover{border-color:var(--border-strong);background:#f0f3fb}
.tbtn.sel{border:2px solid var(--navy);background:#eef2fa;color:var(--navy);font-weight:600}

/* ── STATUS BAR ── */
.sbar{display:flex;align-items:center;justify-content:space-between;padding:10px 14px;background:var(--card);border-radius:8px;border:0.5px solid var(--border);margin-bottom:1rem;font-size:13px}
.sbar-txt{color:var(--text2)}
.sbar-count{font-weight:700;color:var(--navy)}

/* ── NGANH GRID ── */
.nganh-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(200px,1fr));gap:8px;margin-bottom:1rem}
.ncard{border:1.5px solid var(--border);border-radius:var(--r);padding:14px;cursor:pointer;background:var(--card);transition:all .15s;box-shadow:var(--shadow)}
.ncard:hover{border-color:var(--border-strong);transform:translateY(-1px)}
.ncard.sel{border:2px solid var(--navy);background:#eef2fa}
.ncard-icon{font-size:24px;margin-bottom:6px}
.ncard-name{font-size:13px;font-weight:600;color:var(--text);margin-bottom:3px;line-height:1.3}
.ncard-match{font-size:11px;font-weight:600;margin-bottom:4px}
.match-high{color:var(--green)}
.match-mid{color:#b05a00}
.match-low{color:var(--text3)}
.ncard-desc{font-size:11px;color:var(--text3);line-height:1.4}

/* ── RESULT CARD ── */
.rcard{background:var(--card);border:1.5px solid var(--border);border-radius:var(--r);padding:1.25rem;margin-bottom:1rem;box-shadow:var(--shadow)}
.rcard.hl{border:2px solid var(--navy)}
.rl{font-size:11px;font-weight:700;letter-spacing:.06em;text-transform:uppercase;color:var(--text3);margin-bottom:5px}
.rv{font-size:15px;font-weight:600;color:var(--text);margin-bottom:4px}
.cdung{background:var(--amber-light);border-left:3px solid var(--amber);padding:12px 14px;border-radius:0 8px 8px 0;font-size:13px;color:#633806;line-height:1.6;margin-bottom:1rem;font-style:italic}
.tags{display:flex;flex-wrap:wrap;gap:5px;margin-top:5px}
.tag{font-size:11px;padding:3px 9px;border-radius:20px;font-weight:500}
.tag-navy{background:#eef2fa;color:var(--navy);border:1px solid var(--navy)}
.tag-green{background:var(--green-light);color:var(--green);border:1px solid #9fdd97}
.tag-amber{background:var(--amber-light);color:#854f0b;border:1px solid var(--amber)}
.tag-plain{background:#f0f3fb;color:var(--text2);border:1px solid var(--border)}
.divider{height:1px;background:var(--border);margin:1rem 0}
.school-item{padding:10px 12px;border-radius:8px;background:var(--bg);margin-bottom:5px;border:0.5px solid var(--border)}
.school-name{font-size:13px;font-weight:600;color:var(--text)}
.school-tohop{font-size:12px;color:var(--text2);margin-top:2px}
.warn-box{background:#fff0f0;border-left:3px solid #e24b4a;padding:10px 14px;border-radius:0 8px 8px 0;font-size:12px;color:#a32d2d;line-height:1.5;margin-top:.75rem}

/* ── BUTTONS ── */
.btn-row{display:flex;gap:8px;flex-wrap:wrap;margin-top:1rem}
.btn{border:1.5px solid var(--border-strong);border-radius:8px;padding:9px 18px;background:var(--card);cursor:pointer;font-size:13px;font-weight:500;color:var(--text);font-family:inherit;transition:all .15s}
.btn:hover{background:#f0f3fb;border-color:var(--navy)}
.btn:disabled{opacity:.4;cursor:default}
.btn-primary{background:var(--navy);color:white;border-color:var(--navy)}
.btn-primary:hover{background:var(--navy-light)}
.btn-primary:disabled{background:var(--navy);opacity:.4}

/* ── FOOTER ── */
.footer{background:var(--navy);padding:1.25rem 1.5rem;text-align:center;margin-top:3rem}
.footer-txt{color:rgba(255,255,255,.7);font-size:12px;line-height:1.7}
.footer-hl{color:var(--amber);font-weight:600}
.footer-link{color:rgba(255,255,255,.7);text-decoration:none}
.footer-link:hover{text-decoration:underline}
a.footer-hl{text-decoration:none}
a.footer-hl:hover{text-decoration:underline}

/* ── SCHOOL SEARCH ── */
.school-search-box{background:var(--card);border:1.5px solid var(--border-strong);border-radius:var(--r);padding:1rem 1.25rem;margin-bottom:1rem}
.school-search-box input{width:100%;padding:9px 12px;border:1.5px solid var(--border);border-radius:8px;font-size:13px;font-family:inherit;color:var(--text);background:var(--bg);outline:none;margin-top:6px}
.school-search-box input:focus{border-color:var(--navy)}
.school-search-box input::placeholder{color:var(--text3)}
.school-found{background:var(--green-light);border:1.5px solid #9fdd97;border-radius:8px;padding:10px 14px;margin-top:8px;font-size:13px;color:var(--green)}
.school-notfound{background:var(--amber-light);border:1.5px solid var(--amber);border-radius:8px;padding:10px 14px;margin-top:8px;font-size:13px;color:#854f0b}
.chung-table{width:100%;border-collapse:collapse;font-size:12px;margin-top:6px}
.chung-table th{background:var(--navy);color:white;padding:8px 10px;text-align:left;font-weight:600}
.chung-table td{padding:8px 10px;border-bottom:0.5px solid var(--border);color:var(--text2);vertical-align:top}
.chung-table tr:last-child td{border-bottom:none}
.chung-table tr:nth-child(even) td{background:#f7f8fc}
.hna-cta{background:var(--navy);border-radius:var(--r);padding:1.25rem;margin-top:1rem;display:flex;align-items:center;gap:1rem;flex-wrap:wrap}
.hna-cta-txt{flex:1;min-width:200px}
.hna-cta-txt .title{color:white;font-weight:700;font-size:14px;margin-bottom:4px}
.hna-cta-txt .sub{color:rgba(255,255,255,.65);font-size:12px;line-height:1.5}
.hna-cta .btn-amber{background:var(--amber);color:#142768;border:none;border-radius:8px;padding:10px 18px;font-size:13px;font-weight:700;cursor:pointer;font-family:inherit;white-space:nowrap;text-decoration:none;display:inline-block}
.hna-cta .btn-amber:hover{background:#e68800}

/* ── CTRUC PANEL ── */
.ctruc-wrap{background:var(--card);border:1.5px solid var(--border-strong);border-radius:var(--r);margin-bottom:1.25rem;overflow:hidden;box-shadow:var(--shadow)}
.ctruc-header{display:flex;align-items:center;justify-content:space-between;padding:1rem 1.25rem;background:var(--navy);gap:1rem}
.ctruc-title{font-size:15px;font-weight:700;color:white;line-height:1.3}
.ctruc-sub{font-size:11px;color:rgba(255,255,255,.6);margin-top:2px}
.ctruc-toggle{font-size:11px;font-weight:600;color:var(--amber);background:none;border:1px solid var(--amber);border-radius:6px;padding:4px 10px;cursor:pointer;white-space:nowrap;font-family:inherit}
.ctruc-toggle:hover{background:rgba(255,153,0,.15)}
#ctruc-body{padding:1.25rem}
.ctruc-summary{display:flex;align-items:center;justify-content:center;gap:1rem;margin-bottom:1.25rem;flex-wrap:wrap;padding:.75rem;background:var(--bg);border-radius:8px}
.cs-box{text-align:center;padding:.5rem .75rem}
.cs-num{font-size:32px;font-weight:800;line-height:1}
.cs-label{font-size:12px;font-weight:600;margin-top:2px}
.cs-hint{font-size:10px;color:var(--text3);margin-top:1px}
.cs-total .cs-num{color:var(--navy)}
.cs-total .cs-label{color:var(--navy)}
.cs-bb .cs-num{color:var(--navy)}
.cs-bb .cs-label{color:var(--navy)}
.cs-tc .cs-num{color:#c0392b}
.cs-tc .cs-label{color:#c0392b}
.cs-divider{width:1px;height:48px;background:var(--border);margin:0 .5rem}
.cs-plus{font-size:20px;font-weight:700;color:var(--text3)}
.ctruc-tables{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1rem}
.ct-table{border-radius:8px;overflow:hidden;border:1.5px solid var(--border)}
.ct-head{padding:10px 12px;font-size:12px;font-weight:700;letter-spacing:.04em;text-align:center}
.ct-head-bb{background:var(--navy);color:white}
.ct-head-tc{background:#c0392b;color:white}
.ct-tbl{width:100%;border-collapse:collapse;font-size:12px}
.ct-tbl th{padding:6px 10px;background:#f0f3fb;color:var(--text3);font-weight:600;text-align:left;border-bottom:1px solid var(--border)}
.ct-tbl td{padding:7px 10px;border-bottom:0.5px solid var(--border);color:var(--text2)}
.ct-tbl td:first-child{width:36px;text-align:center;font-weight:700;color:var(--navy)}
.ct-tbl tr:last-child td{border-bottom:none}
.ct-tbl tr:nth-child(even) td{background:#fafbfe}
.tc-row td:first-child{color:#c0392b}
.tc-row td{font-weight:500;color:var(--text)}
.ctruc-note{display:flex;align-items:flex-start;gap:8px;padding:10px 14px;background:var(--amber-light);border-radius:8px;border-left:3px solid var(--amber);font-size:13px;color:#633806;line-height:1.5}
.note-icon{font-size:16px;flex-shrink:0;margin-top:1px}
@media(max-width:480px){
  .ctruc-tables{grid-template-columns:1fr}
  .ctruc-summary{gap:.5rem}
  .cs-num{font-size:26px}
}

/* ── ACCORDION TỔ HỢP ── */
.acc-list{display:flex;flex-direction:column;gap:6px}
.acc-item{border:1px solid var(--border);border-radius:var(--r);overflow:hidden;background:var(--card)}
.acc-item.acc-main{border:2px solid var(--navy)}
.acc-head{width:100%;display:flex;align-items:center;gap:10px;padding:11px 14px;background:none;border:none;cursor:pointer;text-align:left;font-family:inherit;transition:background .12s}
.acc-head:hover{background:var(--bg)}
.acc-head.open{background:#eef2fa}
.acc-code{font-size:15px;font-weight:700;color:var(--text2);min-width:52px;flex-shrink:0}
.acc-code-main{color:var(--navy)}
.acc-mon3{flex:1;font-size:12px;color:var(--text2);line-height:1.4}
.acc-chevron{font-size:13px;color:var(--text3);transition:transform .2s;flex-shrink:0}
.acc-head.open .acc-chevron{transform:rotate(180deg)}
.acc-body{padding:10px 14px 12px;border-top:1px solid var(--border);background:var(--bg)}
.acc-row{display:flex;gap:8px;margin-bottom:7px;font-size:12px;align-items:flex-start}
.acc-row:last-child{margin-bottom:0}
.acc-label{color:var(--text3);min-width:130px;flex-shrink:0;padding-top:1px}
.acc-val{color:var(--text2);flex:1;line-height:1.5}
.acc-val.accent{color:var(--navy);font-weight:500}
.acc-val.muted{color:var(--text3)}
.acc-highlight{margin-top:8px;padding:7px 10px;background:#eef2fa;border-left:3px solid var(--navy);border-radius:0 6px 6px 0;font-size:12px;color:var(--navy)}
@media(max-width:480px){.acc-label{min-width:100px}}

/* ── CHỌN MÔN THI TN ── */
.tn-section{margin-top:1rem;padding-top:1rem;border-top:1.5px dashed var(--border)}
.tn-section.hidden{display:none}
.tn-chips{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:.75rem}
.tn-chip{padding:6px 14px;border-radius:20px;font-size:12px;font-weight:500;border:1.5px solid var(--border);background:var(--bg);cursor:pointer;transition:all .15s;color:var(--text2);font-family:inherit}
.tn-chip:hover{border-color:var(--navy);color:var(--navy)}
.tn-chip.picked{background:var(--amber);color:#142768;border-color:var(--amber);font-weight:700}
.tn-chip.disabled-chip{opacity:.35;cursor:default;pointer-events:none}
.tohop-result-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(190px,1fr));gap:8px;margin-top:.75rem}
.tohop-result-card{border:1.5px solid var(--border);border-radius:var(--r);padding:12px;background:var(--card)}
.tohop-result-card.match-card{border:2px solid var(--navy);background:#eef2fa}
.trc-code{font-size:16px;font-weight:700;color:var(--navy);margin-bottom:3px}
.trc-mons{font-size:11px;color:var(--text2);margin-bottom:6px;line-height:1.5}
.trc-nganh{font-size:11px;color:var(--text3);line-height:1.4}
.trc-badge{display:inline-block;font-size:10px;font-weight:700;padding:2px 8px;border-radius:20px;margin-bottom:5px}
.badge-target{background:#142768;color:white}
.badge-open{background:#eaf4ea;color:var(--green);border:1px solid #9fdd97}
.badge-partial{background:var(--amber-light);color:#854f0b;border:1px solid var(--amber)}
.tn-summary-bar{display:flex;align-items:center;gap:6px;padding:10px 14px;background:#eef2fa;border-radius:8px;margin-bottom:.75rem;flex-wrap:wrap;font-size:12px}
.tn-fixed-pill{padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:var(--navy);color:white}
.tn-plus{color:var(--text3);font-weight:700;font-size:13px}
.tn-chosen-pill{padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:var(--amber);color:#142768}
.tn-eq{color:var(--text3);font-size:12px}

/* ── NHẬP TỔ HỢP TRƯỜNG ── */
.tohop-builder{background:var(--card);border:1.5px solid var(--border-strong);border-radius:var(--r);padding:1.25rem;margin-bottom:1rem}
.tohop-builder .tb-title{font-size:13px;font-weight:600;color:var(--navy);margin-bottom:.5rem}
.tohop-builder .tb-sub{font-size:12px;color:var(--text3);margin-bottom:1rem}
.mon-chips{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:.75rem}
.mon-chip{padding:6px 12px;border-radius:20px;font-size:12px;font-weight:500;border:1.5px solid var(--border);background:var(--bg);cursor:pointer;transition:all .15s;color:var(--text2);font-family:inherit}
.mon-chip:hover{border-color:var(--navy);color:var(--navy)}
.mon-chip.picked{background:var(--navy);color:white;border-color:var(--navy)}
.tohop-slots{display:flex;gap:6px;flex-wrap:wrap;margin-bottom:.75rem;min-height:36px;padding:6px 10px;background:var(--bg);border-radius:8px;border:1.5px dashed var(--border)}
.slot-tag{display:flex;align-items:center;gap:4px;padding:4px 10px;border-radius:20px;background:#eef2fa;color:var(--navy);font-size:12px;font-weight:500}
.slot-tag button{background:none;border:none;cursor:pointer;color:#a0a8c0;font-size:14px;padding:0;line-height:1;font-family:inherit}
.slot-tag button:hover{color:var(--navy)}
.slots-hint{font-size:12px;color:var(--text3);align-self:center}
.match-result{border-radius:var(--r);padding:1rem;margin-top:.75rem;border:1.5px solid}
.match-yes{background:#eaf4ea;border-color:#9fdd97}
.match-no{background:#fff0f0;border-color:#f09595}
.match-partial{background:var(--amber-light);border-color:var(--amber)}
.match-icon{font-size:22px;margin-bottom:4px}
.match-title{font-size:14px;font-weight:700;margin-bottom:4px}
.match-yes .match-title{color:var(--green)}
.match-no .match-title{color:#a32d2d}
.match-partial .match-title{color:#854f0b}
.match-detail{font-size:12px;line-height:1.6;color:var(--text2)}

/* ── FORM GỬI DATA ── */
.send-form{background:var(--card);border:1.5px solid var(--border);border-radius:var(--r);padding:1.25rem;margin-top:1rem}
.send-form .sf-title{font-size:13px;font-weight:600;color:var(--navy);margin-bottom:4px}
.send-form .sf-sub{font-size:12px;color:var(--text3);margin-bottom:.75rem;line-height:1.5}
.send-form input,.send-form select{width:100%;padding:8px 12px;border:1.5px solid var(--border);border-radius:8px;font-size:13px;font-family:inherit;color:var(--text);background:var(--bg);outline:none;margin-bottom:8px}
.send-form input:focus,.send-form select:focus{border-color:var(--navy)}
.send-form .row2{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.send-status{margin-top:8px;font-size:13px;padding:8px 12px;border-radius:8px;display:none}
.send-ok{background:var(--green-light);color:var(--green)}
.send-err{background:#fff0f0;color:#a32d2d}

/* ── SÔNG AN STYLE — NGANH LIST ── */
/* ── TÌM KIẾM 36 NGÀNH ── */
.nganh-search-wrap{position:relative;margin-bottom:.625rem}
.nganh-search{width:100%;padding:9px 70px 9px 12px;font-size:13px;border:1px solid var(--border-strong);border-radius:8px;background:var(--card);color:var(--text);font-family:inherit}
.nganh-search:focus{outline:none;border-color:var(--navy)}
.nganh-search-count{position:absolute;right:10px;top:50%;transform:translateY(-50%);font-size:10px;color:var(--text3);background:var(--bg);padding:2px 8px;border-radius:20px;pointer-events:none}

.sa-list{border:1px solid var(--border-strong);border-radius:var(--r);overflow:hidden}
.sa-item{border-bottom:0.5px solid var(--border)}
.sa-item:last-child{border-bottom:none}
.sa-head{display:flex;align-items:center;gap:10px;padding:12px 14px;cursor:pointer;background:var(--card);transition:background .12s;-webkit-tap-highlight-color:transparent;width:100%;border:none;text-align:left;font-family:inherit}
.sa-head:hover{background:var(--bg)}
.sa-item.open .sa-head,.sa-item.selected .sa-head{background:#eef2fa}
.sa-icon{width:36px;height:36px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:17px;flex-shrink:0;background:var(--bg)}
.sa-item.open .sa-icon,.sa-item.selected .sa-icon{background:#dde6fa}
.sa-info{flex:1;min-width:0}
.sa-name{font-size:14px;font-weight:500;color:var(--text);line-height:1.3}
.sa-sub{font-size:11px;color:var(--text3);margin-top:2px}
.sa-right{display:flex;align-items:center;gap:6px;flex-shrink:0}
.sa-badge{font-size:10px;font-weight:600;padding:3px 8px;border-radius:20px;white-space:nowrap}
.sa-badge-match{background:var(--navy);color:white}
.sa-badge-ok{background:var(--green-light);color:#27500a;border:0.5px solid #97c459}
.sa-sel-dot{width:8px;height:8px;border-radius:50%;background:var(--amber);display:none}
.sa-item.selected .sa-sel-dot{display:block}
.sa-chev{color:var(--text3);font-size:15px;transition:transform .2s}
.sa-item.open .sa-chev{transform:rotate(180deg);color:var(--navy)}
.sa-body{display:none;padding:12px 14px 14px;background:#f7f9fe;border-top:0.5px solid #dde6fa}
.sa-item.open .sa-body{display:block}
.sa-mo{font-size:13px;color:var(--text2);line-height:1.6;margin-bottom:10px}
.sa-detail{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:10px}
.sa-box{background:var(--card);border:0.5px solid var(--border);border-radius:8px;padding:9px 11px}
.sa-box.full{grid-column:1/-1}
.sa-blabel{font-size:10px;font-weight:600;letter-spacing:.05em;text-transform:uppercase;color:var(--text3);margin-bottom:5px}
.sa-pills{display:flex;flex-wrap:wrap;gap:4px}
.sa-pill{font-size:11px;font-weight:500;padding:3px 9px;border-radius:20px;background:#eef2fa;color:var(--navy);border:0.5px solid #b5caf4}
.sa-pill.star{background:var(--navy);color:white;border-color:var(--navy)}
.sa-mon-item{padding:4px 0;border-bottom:0.5px solid var(--border);display:flex;align-items:baseline;gap:5px;font-size:12px;color:var(--text2)}
.sa-mon-item:last-child{border-bottom:none}
.sa-mon-item::before{content:'→';color:var(--navy);font-size:10px;flex-shrink:0}
.sa-truong-list{font-size:12px;color:var(--text2);line-height:1.8}
.sa-truong-item{display:flex;align-items:center;gap:5px}
.sa-truong-item::before{content:'•';color:var(--navy);font-size:14px;line-height:1}
.sa-foot{display:flex;gap:8px;margin-top:10px;flex-wrap:wrap}
.sa-btn-sel{font-size:12px;padding:7px 16px;border-radius:8px;border:none;background:var(--navy);color:white;cursor:pointer;font-family:inherit;font-weight:500}
.sa-btn-sel:hover{background:var(--navy-light)}
.sa-btn-sel.selected-state{background:var(--amber);color:#142768}
.sa-btn-skip{font-size:12px;padding:7px 14px;border-radius:8px;border:0.5px solid var(--border-strong);background:transparent;color:var(--text2);cursor:pointer;font-family:inherit}

/* ── TIMELINE 2026 ── */
.ts26-wrap{background:var(--card);border:1px solid var(--border-strong);border-radius:var(--r);padding:1rem 1.25rem;margin-top:1rem}
.ts26-header{display:flex;align-items:center;gap:8px;margin-bottom:.875rem}
.ts26-badge{font-size:11px;font-weight:700;padding:3px 9px;border-radius:20px;background:var(--navy);color:white}
.ts26-title{font-size:13px;font-weight:600;color:var(--navy)}
.ts26-grid{display:flex;flex-direction:column;gap:0;position:relative;padding-left:24px}
.ts26-grid::before{content:'';position:absolute;left:6px;top:8px;bottom:8px;width:2px;background:var(--border)}
.ts26-item{display:flex;align-items:flex-start;padding:6px 0;position:relative}
.ts26-dot{width:14px;height:14px;border-radius:50%;border:2px solid var(--border);background:var(--card);flex-shrink:0;margin-top:2px;position:absolute;left:-24px}
.ts26-item.done .ts26-dot{background:var(--green);border-color:var(--green)}
.ts26-item.active .ts26-dot{background:var(--amber);border-color:var(--amber);box-shadow:0 0 0 3px rgba(255,153,0,.2)}
.ts26-date{font-size:11px;font-weight:700;color:var(--navy);min-width:90px;padding-top:1px}
.ts26-item.done .ts26-date{color:#1a7a1a}
.ts26-item.active .ts26-date{color:#854f0b}
.ts26-desc{font-size:12px;color:var(--text2);line-height:1.5;flex:1}
.ts26-warn{margin-top:.875rem;padding:9px 12px;background:#fff0f0;border-left:3px solid #e24b4a;border-radius:0 8px 8px 0;font-size:12px;color:#a32d2d;line-height:1.5}

/* ── TAB SYSTEM BƯỚC 3 ── */
.dh-tabs{display:flex;border-bottom:0.5px solid var(--border);gap:0;background:var(--card)}
.dh-tab{font-size:12px;font-weight:500;padding:10px 14px;border-bottom:2px solid transparent;color:var(--text3);cursor:pointer;background:none;border-top:none;border-left:none;border-right:none;font-family:inherit;flex:1;text-align:center;white-space:nowrap;transition:color .12s}
.dh-tab:hover{color:var(--text2)}
.dh-tab.active{color:var(--navy);border-bottom-color:var(--navy)}
.dh-tabpane{display:none}.dh-tabpane.show{display:block}
.dh-card{background:var(--card);border:0.5px solid var(--border-strong);border-radius:var(--r);overflow:hidden;margin-bottom:.75rem}
.dh-card-head{display:flex;align-items:flex-start;gap:10px;padding:1rem 1.25rem;border-bottom:0.5px solid var(--border)}
.dh-nganh-icon{width:40px;height:40px;border-radius:8px;background:var(--bg);display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0}
.dh-nganh-name{font-size:15px;font-weight:600;color:var(--navy)}
.dh-nganh-sub{font-size:11px;color:var(--text3);margin-top:2px}
.dh-section{padding:.875rem 1.25rem;border-bottom:0.5px solid var(--border)}
.dh-section:last-child{border-bottom:none}
.dh-slabel{font-size:10px;font-weight:600;letter-spacing:.06em;text-transform:uppercase;color:var(--text3);margin-bottom:.5rem}
.dh-pills{display:flex;flex-wrap:wrap;gap:5px}
.dh-pill{font-size:12px;font-weight:500;padding:3px 10px;border-radius:20px;background:var(--bg);color:var(--text2);border:0.5px solid var(--border)}
.dh-pill-star{background:#eef2fa;color:var(--navy);border-color:#b5caf4;font-weight:600}
.dh-mon-row{font-size:12px;color:var(--text2);padding:4px 0;border-bottom:0.5px solid var(--border);display:flex;align-items:baseline;gap:6px}
.dh-mon-row:last-child{border-bottom:none}
.dh-mon-row::before{content:'→';color:var(--navy);font-size:10px;flex-shrink:0}
.dh-stat-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;padding:.875rem 1.25rem}
.dh-stat{background:var(--bg);border-radius:8px;padding:.5rem .75rem;text-align:center}
.dh-stat-val{font-size:15px;font-weight:600;color:var(--navy)}
.dh-stat-lbl{font-size:10px;color:var(--text3);margin-top:1px}
.dh-truong-list{display:flex;flex-direction:column;gap:4px}
.dh-truong-row{display:flex;align-items:center;gap:8px;padding:6px 10px;border-radius:8px;background:var(--bg)}
.dh-truong-dn{border-left:2px solid var(--navy);background:#eef2fa}
.dh-truong-name{flex:1;font-size:12px;font-weight:500;color:var(--text);min-width:0;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.dh-truong-dn .dh-truong-name{color:var(--navy)}
.dh-chip{font-size:10px;padding:2px 7px;border-radius:20px;white-space:nowrap;flex-shrink:0}
.dh-chip-ct{background:var(--card);color:var(--text3);border:0.5px solid var(--border)}
.dh-chip-high{background:#fff0f0;color:#a32d2d}
.dh-chip-mid{background:var(--amber-light);color:#854f0b}
.dh-chip-ok{background:var(--green-light);color:#27500a}
.co-hoi-item{display:flex;align-items:flex-start;gap:8px;font-size:12px;color:var(--text2);padding:5px 0;border-bottom:0.5px solid var(--border);line-height:1.5}
.co-hoi-item:last-child{border-bottom:none}
.co-hoi-item::before{content:'✦';color:var(--amber);font-size:9px;flex-shrink:0;margin-top:3px}
.luong-box{display:flex;align-items:center;gap:10px;padding:8px 12px;background:var(--green-light);border-radius:8px;border-left:2px solid var(--green)}
.luong-val{font-size:14px;font-weight:600;color:#27500a}
.luong-lbl{font-size:11px;color:var(--text3)}
.dh-ts247-btn{display:inline-flex;align-items:center;gap:6px;font-size:12px;font-weight:600;padding:9px 16px;border-radius:8px;background:var(--navy);color:white;text-decoration:none;transition:background .12s}
.dh-ts247-btn:hover{background:var(--navy-light)}
.dh-ts247-btn:active{transform:scale(.98)}

/* ── 207 TRƯỜNG TRA CỨU ── */
.sch207-search{width:100%;padding:8px 12px;font-size:12px;border:0.5px solid var(--border-strong);border-radius:8px;background:var(--card);color:var(--text);font-family:inherit;margin-bottom:8px}
.sch207-search:focus{outline:none;border-color:var(--navy)}
.sch207-filters{display:flex;gap:5px;margin-bottom:8px;flex-wrap:wrap}
.sch207-filter{font-size:11px;font-weight:500;padding:4px 11px;border-radius:20px;border:0.5px solid var(--border-strong);background:var(--card);color:var(--text2);cursor:pointer;font-family:inherit}
.sch207-filter.active{background:var(--navy);color:white;border-color:var(--navy)}
.sch207-list{display:flex;flex-direction:column;gap:4px;max-height:340px;overflow-y:auto}
.sch207-row{padding:7px 10px;border-radius:8px;background:var(--bg);border:0.5px solid transparent}
.sch207-dn{border-left:2px solid var(--navy);background:#eef2fa}
.sch207-main{display:flex;align-items:center;justify-content:space-between;gap:8px;flex-wrap:wrap}
.sch207-name{font-size:12px;font-weight:500;color:var(--text)}
.sch207-dn .sch207-name{color:var(--navy)}
.sch207-meta{display:flex;gap:5px;align-items:center;flex-shrink:0}
.sch207-ma{font-size:10px;font-weight:600;color:var(--navy);background:#eef2fa;padding:1px 6px;border-radius:20px}
.sch207-mien,.sch207-loai{font-size:10px;color:var(--text3);background:var(--card);padding:1px 6px;border-radius:20px;border:0.5px solid var(--border)}
.sch207-pt{font-size:11px;color:var(--text2);margin-top:3px;line-height:1.5}

/* ── 3 CỘT MIỀN BẮC/TRUNG/NAM ── */
.mien-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
.mien-col{background:var(--bg);border-radius:8px;overflow:hidden;border:0.5px solid var(--border);display:flex;flex-direction:column}
.mien-head{font-size:11px;font-weight:600;padding:7px 9px;display:flex;align-items:center;justify-content:space-between;border-bottom:0.5px solid var(--border)}
.mien-bac{background:#e8f0fe;color:#1a4fa0}
.mien-trung{background:#e6f4ea;color:#1a6e2e}
.mien-nam{background:#fff0db;color:#9a5a00}
.mien-count{font-size:10px;font-weight:700;background:rgba(255,255,255,.6);padding:1px 6px;border-radius:20px}
.mien-list{display:flex;flex-direction:column;max-height:340px;overflow-y:auto}
.mien-item{padding:7px 9px;border-bottom:0.5px solid var(--border)}
.mien-item:last-child{border-bottom:none}
.mien-item-dn{background:#eef2fa}
.mien-item-name{font-size:11px;font-weight:600;color:var(--text);line-height:1.35;margin-bottom:4px}
.mien-item-dn .mien-item-name{color:var(--navy)}
.mien-item-meta{display:flex;flex-wrap:wrap;gap:4px}
.mien-tag{font-size:9px;font-weight:600;padding:1px 6px;border-radius:20px;background:var(--card);color:var(--text3);border:0.5px solid var(--border);white-space:nowrap}
.mien-tag-ct{color:var(--navy);background:#eef2fa;border-color:#b5caf4}
.mien-tag-hp{color:#1a6e2e;background:var(--green-light);border-color:transparent}
.mien-empty{font-size:11px;color:var(--text3);padding:10px 9px;text-align:center;font-style:italic}

/* ── RESPONSIVE ── */
@media(max-width:480px){
  .hero-title{font-size:18px}
  .trait-grid{grid-template-columns:repeat(2,1fr)}
  .nganh-grid{grid-template-columns:1fr}
  .flow-step{font-size:10px}
  .flow-step .fn{font-size:15px}
  .mien-grid{grid-template-columns:1fr;gap:6px}
  .mien-list{max-height:200px}
}
</style>
</head>
<body>

<header class="hdr">
  <div>
    <div class="hdr-brand">Hướng Nghiệp Alpha</div>
    <div class="hdr-sub">Biến ước mơ thành sự nghiệp</div>
  </div>
  <a href="tel:0969374411" class="hdr-contact">📞 096 937 4411</a>
</header>

<div class="main">

  <div class="hero">
    <div class="hero-tag">Công cụ tư vấn hướng nghiệp 2K11</div>
    <div class="hero-title">Hiểu mình → Nhóm ngành → Tổ hợp xét tuyển → Môn lựa chọn lớp 10</div>
    <div class="hero-desc">Chọn mô tả phù hợp với bản thân để nhận gợi ý nhóm ngành, tổ hợp xét tuyển tham khảo và môn lựa chọn nên đăng ký ở lớp 10.</div>
  </div>

  <!-- PANEL 0: CẤU TRÚC CHƯƠNG TRÌNH -->
  <div class="ctruc-wrap" id="ctruc-wrap">
    <div class="ctruc-header">
      <div>
        <div class="ctruc-title">Chọn Tổ Hợp Môn Lớp 10 Theo Chương Trình 2018</div>
        <div class="ctruc-sub">Hiểu đúng cấu trúc trước khi chọn môn</div>
      </div>
      <button class="ctruc-toggle" onclick="toggleCtruc()" id="ctruc-toggle-btn">Thu gọn ▲</button>
    </div>

    <div id="ctruc-body">
      <!-- TỔNG QUAN -->
      <div class="ctruc-summary">
        <div class="cs-box cs-total">
          <div class="cs-num">12</div>
          <div class="cs-label">Môn ghi học bạ</div>
        </div>
        <div class="cs-divider"></div>
        <div class="cs-box cs-bb">
          <div class="cs-num">8</div>
          <div class="cs-label">Môn bắt buộc</div>
        </div>
        <div class="cs-plus">+</div>
        <div class="cs-box cs-tc">
          <div class="cs-num">4</div>
          <div class="cs-label">Môn tự chọn</div>
          <div class="cs-hint">(chọn trong 9 môn)</div>
        </div>
      </div>

      <!-- BẢNG 2 CỘT -->
      <div class="ctruc-tables">
        <!-- CỘT TRÁI: BẮT BUỘC -->
        <div class="ct-table">
          <div class="ct-head ct-head-bb">8 MÔN BẮT BUỘC</div>
          <table class="ct-tbl">
            <thead><tr><th>STT</th><th>Môn học</th></tr></thead>
            <tbody>
              <tr><td>1</td><td>Toán</td></tr>
              <tr><td>2</td><td>Ngữ văn</td></tr>
              <tr><td>3</td><td>Tiếng Anh</td></tr>
              <tr><td>4</td><td>Lịch sử</td></tr>
              <tr><td>5</td><td>GD Quốc phòng &amp; An ninh</td></tr>
              <tr><td>6</td><td>GD Thể chất</td></tr>
              <tr><td>7</td><td>HĐTN &amp; HN</td></tr>
              <tr><td>8</td><td>Giáo dục địa phương</td></tr>
            </tbody>
          </table>
        </div>

        <!-- CỘT PHẢI: TỰ CHỌN -->
        <div class="ct-table">
          <div class="ct-head ct-head-tc">9 MÔN TỰ CHỌN <span style="font-weight:400;font-size:11px">(chọn 4 trong 9)</span></div>
          <table class="ct-tbl">
            <thead><tr><th>STT</th><th>Môn học</th></tr></thead>
            <tbody>
              <tr class="tc-row"><td>1</td><td>Vật lí</td></tr>
              <tr class="tc-row"><td>2</td><td>Hóa học</td></tr>
              <tr class="tc-row"><td>3</td><td>Sinh học</td></tr>
              <tr class="tc-row"><td>4</td><td>Tin học</td></tr>
              <tr class="tc-row"><td>5</td><td>Địa lí</td></tr>
              <tr class="tc-row"><td>6</td><td>GD Kinh tế &amp; Pháp luật</td></tr>
              <tr class="tc-row"><td>7</td><td>Công nghệ</td></tr>
              <tr class="tc-row"><td>8</td><td>Âm nhạc</td></tr>
              <tr class="tc-row"><td>9</td><td>Mỹ thuật</td></tr>
            </tbody>
          </table>
        </div>
      </div>

      <!-- LƯU Ý QUAN TRỌNG -->
      <div class="ctruc-note">
        <span class="note-icon">💡</span>
        <span>4 môn tự chọn bạn đăng ký ở lớp 10 sẽ học xuyên suốt lớp 10–11–12 → trực tiếp quyết định tổ hợp xét tuyển đại học. <strong>Chọn sai rất khó sửa!</strong></span>
      </div>

      <!-- MỐC THỜI GIAN 2026 -->
      <div class="ts26-wrap">
        <div class="ts26-header">
          <span class="ts26-badge">📅 2026</span>
          <span class="ts26-title">Mốc thời gian xét tuyển đại học quan trọng</span>
        </div>
        <div class="ts26-grid">
          <div class="ts26-item done">
            <div class="ts26-dot"></div>
            <div class="ts26-content">
              <div class="ts26-date">6/6/2026</div>
              <div class="ts26-desc">Hoàn thành rà soát điểm học bạ THPT trên hệ thống</div>
            </div>
          </div>
          <div class="ts26-item active">
            <div class="ts26-dot"></div>
            <div class="ts26-content">
              <div class="ts26-date">17–21/6/2026</div>
              <div class="ts26-desc"><strong>Thực hành đăng ký nguyện vọng</strong> — làm quen hệ thống</div>
            </div>
          </div>
          <div class="ts26-item">
            <div class="ts26-dot"></div>
            <div class="ts26-content">
              <div class="ts26-date">2–14/7/2026</div>
              <div class="ts26-desc"><strong>Đăng ký nguyện vọng chính thức</strong> tại thisinh.thitotnghiepthpt.edu.vn</div>
            </div>
          </div>
          <div class="ts26-item">
            <div class="ts26-dot"></div>
            <div class="ts26-content">
              <div class="ts26-date">15–21/7/2026</div>
              <div class="ts26-desc">Nộp lệ phí xét tuyển trực tuyến</div>
            </div>
          </div>
          <div class="ts26-item">
            <div class="ts26-dot"></div>
            <div class="ts26-content">
              <div class="ts26-date">21/8/2026</div>
              <div class="ts26-desc">Xác nhận nhập học đợt 1 (hạn chót 17:00)</div>
            </div>
          </div>
        </div>
        <div class="ts26-warn">
          ⚠️ <strong>Quy chế mới 2026:</strong> Xét học bạ yêu cầu kết quả cả 6 học kỳ (3 năm THPT), tổ hợp phải có Toán hoặc Ngữ văn, và đạt tối thiểu <strong>15/30 điểm</strong> ở 3 môn thi tốt nghiệp tương ứng.
        </div>
      </div>

      <div style="text-align:center;margin-top:1rem">
        <button class="btn btn-primary" onclick="startTool()">Bắt đầu chọn tổ hợp phù hợp →</button>
      </div>
    </div>
  </div>

  <div class="flow" id="flow-bar">
    <div class="flow-step active" id="fs1" onclick="goStep(1)"><span class="fn">1</span>Hiểu mình</div>
    <div class="flow-step" id="fs2" onclick="goStep(2)"><span class="fn">2</span>Nhóm ngành</div>
    <div class="flow-step" id="fs3" onclick="goStep(3)"><span class="fn">3</span>Tổ hợp ĐH</div>
    <div class="flow-step" id="fs4" onclick="goStep(4)"><span class="fn">4</span>Môn lớp 10</div>
  </div>

  <!-- PANEL 1 -->
  <div class="panel show" id="panel1">
    <div class="slabel">Bước 1 — Chọn những từ mô tả đúng bản thân (chọn nhiều nhất có thể)</div>
    <div class="trait-grid" id="trait-grid"></div>
    <div class="sbar">
      <span class="sbar-txt" id="sbar-txt">Chưa chọn gì — hãy chọn ít nhất 2 mô tả bản thân</span>
      <span class="sbar-count" id="sbar-cnt">0</span>
    </div>
    <div class="btn-row">
      <button class="btn" onclick="resetAll()">Làm lại</button>
      <button class="btn btn-primary" id="btn12" onclick="goStep(2)" disabled>Xem ngành phù hợp →</button>
    </div>
  </div>

  <!-- PANEL 2 -->
  <div class="panel" id="panel2">
    <div class="slabel">Bước 2 — Chọn nhóm ngành phù hợp với bạn</div>
    <p style="font-size:12px;color:var(--text3);margin-bottom:.625rem">Bấm vào ngành để xem chi tiết · Chọn 1 ngành để tiếp tục</p>
    <div class="nganh-search-wrap">
      <input type="text" class="nganh-search" id="nganh-search" placeholder="🔍 Tìm trong 36 nhóm ngành (VD: y dược, luật, cơ khí...)" oninput="nganhSearchInput(this.value)">
      <span class="nganh-search-count" id="nganh-search-count"></span>
    </div>
    <div class="sa-list" id="nganh-grid"></div>
    <div class="btn-row" style="margin-top:1rem">
      <button class="btn" onclick="goStep(1)">← Hiểu mình</button>
      <button class="btn btn-primary" id="btn23" onclick="goStep(3)" disabled>Xem tổ hợp ĐH →</button>
    </div>
  </div>

  <!-- PANEL 3 -->
  <div class="panel" id="panel3">
    <div class="slabel">Bước 3 — Tổ hợp xét tuyển đại học</div>
    <div id="dh-result"></div>
    <div class="btn-row">
      <button class="btn" onclick="goStep(2)">← Nhóm ngành</button>
      <button class="btn btn-primary" onclick="goStep(4)">Xem môn lớp 10 →</button>
    </div>
  </div>

  <!-- PANEL 4 -->
  <div class="panel" id="panel4">
    <div class="slabel">Bước 4 — Môn cần chọn lớp 10 & kiểm tra tổ hợp trường bạn</div>
    <div id="school-result"></div>

    <!-- TÌM TRƯỜNG -->
    <div class="school-search-box">
      <div class="rl">Tìm trường của bạn trong dữ liệu</div>
      <input type="text" id="school-input" placeholder="Nhập tên trường THPT của bạn..." oninput="searchSchool(this.value)">
      <div id="school-search-result"></div>
    </div>

    <!-- NHẬP TỔ HỢP TRƯỜNG (nếu không có trong dữ liệu) -->
    <div class="tohop-builder" id="tohop-builder">
      <div class="tb-title">Trường bạn có những tổ hợp môn nào?</div>
      <div class="tb-sub">Chọn các môn trong tổ hợp trường bạn đã/sẽ đăng ký → hệ thống tự so sánh với ngành bạn muốn học</div>
      <div class="rl" style="margin-bottom:6px">Chọn môn để tạo tổ hợp trường</div>
      <div class="mon-chips" id="mon-chips"></div>
      <div class="rl" style="margin-bottom:4px">Tổ hợp bạn đã chọn <span style="color:var(--text3);font-weight:400">(tối đa 4 môn)</span></div>
      <div class="tohop-slots" id="tohop-slots"><span class="slots-hint">Chọn môn bên trên để thêm vào đây...</span></div>

      <!-- BƯỚC 2B: CHỌN 2 MÔN THI TỐT NGHIỆP -->
      <div class="tn-section hidden" id="tn-section">
        <div style="display:flex;align-items:center;gap:8px;margin-bottom:6px">
          <div style="background:var(--amber);color:#142768;font-size:11px;font-weight:700;padding:2px 9px;border-radius:20px">Bước tiếp theo</div>
          <div class="rl" style="margin-bottom:0">Chọn 2 môn thi tốt nghiệp từ 4 môn đã đăng ký</div>
        </div>
        <div style="background:var(--amber-light);border-left:3px solid var(--amber);padding:8px 12px;border-radius:0 6px 6px 0;font-size:12px;color:#633806;margin-bottom:10px">
          <strong>Toán + Ngữ văn</strong> là 2 môn bắt buộc (tính sẵn). Bấm chọn thêm <strong>2 môn dưới đây</strong> để hệ thống tạo tổ hợp xét tuyển ĐH và vẽ sơ đồ luồng cho bạn.
        </div>
        <div style="display:flex;align-items:center;gap:8px;margin-bottom:8px;flex-wrap:wrap">
          <span style="font-size:12px;color:var(--text2)">Đã chọn:</span>
          <span id="tn-progress" style="font-size:12px;font-weight:700;color:var(--navy)">0 / 2 môn</span>
          <span style="font-size:11px;color:var(--text3)" id="tn-hint">← bấm vào môn bên dưới để chọn</span>
        </div>
        <div class="tn-chips" id="tn-chips"></div>
        <div class="tn-summary-bar" id="tn-summary-bar" style="display:none">
          <span class="tn-fixed-pill">Toán</span>
          <span class="tn-plus">+</span>
          <span class="tn-fixed-pill">Ngữ văn</span>
          <span class="tn-plus">+</span>
          <span id="tn-chosen-display" style="display:flex;gap:4px;flex-wrap:wrap"></span>
          <span class="tn-eq">→</span>
          <span style="font-size:12px;color:var(--navy);font-weight:600">4 môn thi tốt nghiệp</span>
        </div>
        <div id="tohop-xettuyen-result"></div>
        <div id="flow-svg-wrap" style="display:none;margin-top:1rem"></div>

      <button class="btn btn-primary" onclick="checkMatch()" id="btn-check" style="margin-top:.75rem;opacity:.4" disabled>Kiểm tra phù hợp với ngành →</button>
      <div id="match-result"></div>

      <!-- FORM GỬI DATA -->
      <div class="send-form" id="send-form" style="display:none">
        <div class="sf-title">Gửi thông tin để HNA hỗ trợ tư vấn miễn phí</div>
        <div class="sf-sub">HNA sẽ liên hệ tư vấn chi tiết hơn cho tổ hợp và ngành của bạn. Thông tin chỉ dùng để hỗ trợ học sinh, không chia sẻ cho bên thứ ba.</div>
        <div class="row2">
          <input type="text" id="sf-name" placeholder="Họ tên học sinh *">
          <input type="text" id="sf-phone" placeholder="Số điện thoại (HS hoặc PH) *">
        </div>
        <input type="text" id="sf-school" placeholder="Tên trường THPT đang học *">
        <div class="row2">
          <select id="sf-lop">
            <option value="">Hiện đang học lớp...</option>
            <option>Lớp 9 (chuẩn bị vào 10)</option>
            <option>Lớp 10</option>
            <option>Lớp 11</option>
            <option>Lớp 12</option>
          </select>
          <select id="sf-tinh">
            <option value="">Tỉnh / Thành phố</option>
            <option>Đồng Nai</option>
            <option>TP. Hồ Chí Minh</option>
            <option>Bình Dương</option>
            <option>Bà Rịa – Vũng Tàu</option>
            <option>Khác</option>
          </select>
        </div>
        <div id="sf-summary" style="font-size:12px;color:var(--text3);margin-bottom:8px"></div>
        <div style="display:flex;gap:8px;flex-wrap:wrap">
          <button class="btn btn-primary" onclick="submitForm()">Gửi thông tin cho HNA →</button>
          <button class="btn" onclick="document.getElementById('send-form').style.display='none'">Bỏ qua</button>
        </div>
        <div class="send-status" id="send-status"></div>
      </div>
    </div>

    <div id="chung-result"></div>
    <div class="btn-row">
      <button class="btn" onclick="goStep(3)">← Tổ hợp ĐH</button>
      <button class="btn" onclick="resetAll()">Bắt đầu lại</button>
    </div>
  </div>

</div>

<footer class="footer">
  <div class="footer-txt">
    <span class="footer-hl">Hướng Nghiệp Alpha</span> – Biến ước mơ thành sự nghiệp<br>
    Hotline: <a href="tel:0969374411" class="footer-hl footer-link">096 937 4411</a> &nbsp;|&nbsp; <a href="mailto:huongnghiepalpha@gmail.com" class="footer-link">huongnghiepalpha@gmail.com</a> &nbsp;|&nbsp; <a href="https://www.huongnghiepalpha.vn" target="_blank" class="footer-link">www.huongnghiepalpha.vn</a><br>
    TP. Biên Hòa, Đồng Nai
  </div>
</footer>

<script>
const TRAITS=[
  {id:'may-moc',    label:'Thích làm việc với máy móc, công cụ, thiết bị',     cats:['cokhi','cntt','xd','quan-doi']},
  {id:'thuc-hanh',  label:'Thích thực hành hơn lý thuyết, học qua làm',        cats:['cokhi','yd','nlts','quan-doi']},
  {id:'chinh-xac',  label:'Cẩn thận, tỉ mỉ, coi trọng sự chính xác',          cats:['kt-tc','yd','cokhi','spg']},
  {id:'phan-tich',  label:'Thích phân tích, tìm hiểu nguyên nhân sự việc',     cats:['cntt','khtn','kt-tc','tl']},
  {id:'khoa-hoc',   label:'Tò mò khoa học, thích thử nghiệm và khám phá',      cats:['khtn','yd','nlts','cntt']},
  {id:'so-lieu',    label:'Nhạy với số liệu, dữ liệu và thống kê',             cats:['kt-tc','cntt','khtn','kt-qtkd']},
  {id:'sang-tao',   label:'Sáng tạo, có gu thẩm mỹ, thích cái mới lạ',        cats:['tkdh','nt','xd','bao-chi']},
  {id:'hinh-anh',   label:'Tư duy hình ảnh, dễ hình dung cấu trúc không gian', cats:['xd','tkdh','cntt','khtn']},
  {id:'bieu-dat',   label:'Thích biểu đạt cảm xúc qua nghệ thuật, ngôn ngữ',  cats:['nt','bao-chi','tl','ngoai-giao']},
  {id:'giup-do',    label:'Thích giúp đỡ, chăm sóc và hỗ trợ người khác',     cats:['yd','spg','tl','quan-doi']},
  {id:'giao-tiep',  label:'Giao tiếp tốt, dễ kết nối và tạo niềm tin',        cats:['bao-chi','du-lich','ngoai-giao','kt-qtkd']},
  {id:'dong-cam',   label:'Đồng cảm sâu, biết lắng nghe và thấu hiểu',        cats:['tl','spg','yd','ngoai-giao']},
  {id:'lanh-dao',   label:'Thích tổ chức, lên kế hoạch và dẫn dắt nhóm',      cats:['kt-qtkd','bao-chi','ngoai-giao','quan-doi']},
  {id:'kinh-doanh', label:'Tư duy kinh doanh, nhạy bén cơ hội thị trường',    cats:['kt-qtkd','kt-tc','bao-chi']},
  {id:'thuyet-phuc',label:'Giỏi thuyết phục, tranh luận, bảo vệ quan điểm',   cats:['luat','bao-chi','ngoai-giao','kt-qtkd']},
  {id:'ky-luat',    label:'Kỷ luật cao, làm việc theo quy trình và tiêu chuẩn',cats:['kt-tc','quan-doi','spg','cokhi']},
  {id:'kien-nhan',  label:'Kiên nhẫn, bền bỉ với mục tiêu dài hạn',           cats:['yd','spg','nlts','khtn']},
  {id:'tu-nhien',   label:'Yêu thiên nhiên, thích sinh vật và môi trường sống',cats:['nlts','khtn','tl','xd']},
  {id:'ngon-ngu',   label:'Yêu ngôn ngữ, ngoại ngữ, đọc viết và diễn đạt tốt',cats:['ngoai-giao','bao-chi','luat','spg']},
  {id:'noi-tam',    label:'Hướng nội, thích tự suy ngẫm và hiểu rõ bản thân', cats:['tl','khtn','spg','yd']},
];

const NGANH=[
  {id:'yd',       icon:'🩺',ten:'Y – Dược – Điều dưỡng',
   mo:'Người nhân ái, cẩn thận, ham học, muốn chăm sóc sức khỏe cộng đồng.',
   tomtat:'Phù hợp với người nhân ái, cẩn trọng, ham học và muốn tạo giá trị thông qua chăm sóc, chữa trị và bảo vệ sức khỏe cộng đồng.',
   dh:['B00: Toán – Hóa học – Sinh học (CHỦ LỰC)','A00: Toán – Vật lý – Hóa học','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Hóa học (bắt buộc)','Sinh học (bắt buộc cho Y khoa)'],
   tohop_l10:['B00 → PHẢI học: Hóa học + Sinh học','A00 → cần: Vật lý + Hóa học','D07 → cần: Hóa học + Tiếng Anh'],
   truong:'ĐH Y Dược TP.HCM, ĐH Y Hà Nội, ĐH Y Dược Huế, ĐH Y Dược Cần Thơ, ĐH Y khoa Phạm Ngọc Thạch, ĐH Lạc Hồng (Đồng Nai)',
   warn:'Sinh học là môn BẮT BUỘC nếu muốn vào Y khoa, Răng Hàm Mặt, Điều dưỡng.',
   traits:['giup-do','chinh-xac','kien-nhan','khoa-hoc']},

  {id:'cntt',     icon:'💻',ten:'Công nghệ thông tin – AI',
   mo:'Người logic, kiên nhẫn, tò mò công nghệ. Thích lập trình, dữ liệu, trí tuệ nhân tạo.',
   tomtat:'Phù hợp với người logic, kiên nhẫn, thích công nghệ và sẵn sàng học liên tục để xây dựng và vận hành hệ thống số.',
   dh:['A01: Toán – Vật lý – Tiếng Anh','A00: Toán – Vật lý – Hóa học','X06: Toán – Vật lý – Tin học (mới 2025)'],
   mon_txt:['Vật lý (cốt lõi)','Tiếng Anh hoặc Tin học'],
   tohop_l10:['A01 → cần: Vật lý + Tiếng Anh','A00 → cần: Vật lý + Hóa học','X06 → cần: Vật lý + Tin học (MỚI 2025)'],
   truong:'ĐH Bách Khoa HN, ĐH Bách Khoa TP.HCM, ĐH CNTT TP.HCM, ĐH Công Nghệ – ĐHQG HN, FPT University, ĐH Lạc Hồng (Đồng Nai)',
   warn:'Vật lý là môn nền tảng CNTT — bắt buộc phải chọn ở lớp 10. 🤖 2026: AI & bán dẫn đang bùng nổ — CNTT, Khoa học dữ liệu, An toàn mạng là nhóm ngành có nhu cầu tuyển dụng cao nhất.',
   traits:['phan-tich','thuc-hanh','so-lieu','may-moc']},

  {id:'kt-tc',    icon:'🏦',ten:'Tài chính – Ngân hàng – Kế toán',
   mo:'Người logic, cẩn thận, nhạy số liệu. Quan tâm tiền tệ, đầu tư, rủi ro, báo cáo tài chính.',
   tomtat:'Phù hợp với người logic, cẩn thận, thích số liệu – tiền tệ – rủi ro và có khả năng giao tiếp xây dựng niềm tin.',
   dh:['A00: Toán – Vật lý – Hóa học','A01: Toán – Vật lý – Tiếng Anh','D01: Toán – Ngữ văn – Tiếng Anh','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Toán (cốt lõi)','Tiếng Anh (ưu tiên cao)','Hóa học hoặc Vật lý tùy tổ hợp trường mục tiêu'],
   tohop_l10:['Ưu tiên 1: Toán + Tiếng Anh (áp dụng cho A01, D01, D07)','Chọn thêm Hóa học → mở thêm A00, D07','Chọn thêm Vật lý → mở thêm A00, A01','Chọn thêm Tin học / GDKT&PL → theo tổ hợp trường mục tiêu'],
   truong:'HV Tài chính, HV Ngân hàng, ĐH Kinh Tế Quốc Dân (NEU), ĐH Kinh Tế TP.HCM (UEH), ĐH Ngoại Thương, ĐH Đồng Nai',
   warn:'D07 (Toán–Hóa–Anh) là tổ hợp đáng cân nhắc cho ngành này, nhưng không phải tổ hợp riêng — nhiều ngành khác cũng dùng D07. Nên kiểm tra đề án tuyển sinh năm đó của trường ĐH mục tiêu.',
   traits:['phan-tich','so-lieu','chinh-xac','kinh-doanh']},

  {id:'kt-qtkd',  icon:'📊',ten:'Kinh tế – QTKD – Thương mại',
   mo:'Người năng động, tư duy tổ chức, quan sát thị trường, thích quản lý doanh nghiệp.',
   tomtat:'Phù hợp với người chủ động, linh hoạt, có tư duy kinh doanh và muốn tạo ra giá trị thông qua vận hành – quản lý – phát triển doanh nghiệp.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh (phổ biến nhất)','A01: Toán – Vật lý – Tiếng Anh','A00: Toán – Vật lý – Hóa học'],
   mon_txt:['Tiếng Anh (quan trọng nhất)'],
   tohop_l10:['D01 → cần: Tiếng Anh (phổ biến nhất)','A01 → cần: Vật lý + Tiếng Anh','A00 → cần: Vật lý + Hóa học'],
   truong:'ĐH Kinh Tế Quốc Dân (NEU), ĐH Kinh Tế TP.HCM (UEH), ĐH Ngoại Thương, ĐH Kinh Tế – ĐHQG HN, ĐH Văn Lang, ĐH Đồng Nai',
   warn:'',traits:['giao-tiep','kinh-doanh','phan-tich','so-lieu']},

  {id:'spg',      icon:'📚',ten:'Sư phạm – Giáo dục',
   mo:'Người kiên nhẫn, yêu thích chia sẻ kiến thức, quan tâm sự phát triển người khác.',
   tomtat:'Phù hợp với người kiên nhẫn, có trách nhiệm, thích giúp người khác tiến bộ và muốn tạo giá trị thông qua dạy học và phát triển con người.',
   dh:['A00: Toán – Vật lý – Hóa học (SP Toán/Lý/Hóa)','B00: Toán – Hóa học – Sinh học (SP Sinh/Hóa)','C00: Ngữ văn – Lịch sử – Địa lý (SP Văn/Sử/Địa)','D01: Toán – Ngữ văn – Tiếng Anh (SP Tiếng Anh/Tin)'],
   mon_txt:['SP Toán/Lý/Hóa → chọn Vật lý + Hóa học lớp 10','SP Sinh/Hóa → chọn Hóa học + Sinh học lớp 10','SP Tiếng Anh → cần Tiếng Anh ≥ 8.0 điểm','SP Văn/Sử/Địa → chọn Địa lý + Lịch sử lớp 10'],
   tohop_l10:['SP Toán/Lý/Hóa → A00: Vật lý + Hóa học','SP Sinh/Hóa → B00: Hóa học + Sinh học','SP Tiếng Anh → D01: Tiếng Anh ≥ 8 điểm','SP Văn/Sử/Địa → C00: không cần môn KHTN'],
   truong:'ĐH Sư Phạm Hà Nội, ĐH Sư Phạm TP.HCM, ĐH Sư Phạm Huế, ĐH Đồng Nai (SP), ĐH Ngoại Ngữ – ĐHQG HN',
   warn:'Tổ hợp tùy chuyên ngành SP — A00 cho KHTN, C00 cho KHXH. Điểm sàn SP tối thiểu 19 điểm.',
   traits:['giup-do','kien-nhan','giao-tiep','dong-cam']},

  {id:'bao-chi',  icon:'📰',ten:'Báo chí – Marketing – Truyền thông',
   mo:'Người nhạy thông tin, sáng tạo, giao tiếp tốt. Thích nội dung, thương hiệu, mạng xã hội.',
   tomtat:'Phù hợp với người linh hoạt, sáng tạo, giao tiếp tốt và muốn tạo ảnh hưởng thông qua truyền thông, nội dung và thương hiệu.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','A01: Toán – Vật lý – Tiếng Anh','C00: Ngữ văn – Lịch sử – Địa lý'],
   mon_txt:['Tiếng Anh','Địa lý + Lịch sử (nếu học C00)'],
   tohop_l10:['D01 → cần: Tiếng Anh mạnh (phổ biến nhất)','C00 → cần: Địa lý + Lịch sử (báo chí KHXH truyền thống)','A01 → cần: Vật lý + Tiếng Anh'],
   truong:'HV Báo Chí & Tuyên Truyền, ĐH KHXH&NV HN, ĐH KHXH&NV TP.HCM, ĐH Văn Lang, ĐH HUTECH, FPT University',
   warn:'',traits:['giao-tiep','sang-tao','ngon-ngu','dong-cam']},

  {id:'luat',     icon:'⚖️',ten:'Luật – Tòa án',
   mo:'Người logic, yêu công bằng, phân tích nhiều góc nhìn. Thích pháp luật và tranh luận.',
   tomtat:'Phù hợp với người công bằng, lý trí, giỏi lập luận và muốn dùng hiểu biết pháp luật để bảo vệ quyền lợi, góp phần xây dựng xã hội minh bạch.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','C00: Ngữ văn – Lịch sử – Địa lý','X70: Ngữ văn – Lịch sử – GDKTPL','A01: Toán – Vật lý – Tiếng Anh','X35: Toán – Lịch sử – GDKTPL'],
   mon_txt:['GDKTPL (nền tảng pháp luật — quan trọng nhất)','Tiếng Anh','Địa lý + Lịch sử (nếu học C00)'],
   tohop_l10:['X70 → cần: Lịch sử + GDKTPL (★ rất phù hợp — học sẵn kiến thức pháp luật từ lớp 10)','D01 → cần: Tiếng Anh (Luật quốc tế)','C00 → cần: Địa lý + Lịch sử (Luật truyền thống)'],
   truong:'ĐH Luật Hà Nội, ĐH Luật TP.HCM, ĐH Kinh Tế Luật – ĐHQG TP.HCM, Khoa Luật – ĐHQG HN, ĐH Ngoại Thương',
   warn:'GDKTPL là môn học trực tiếp về pháp luật trong chương trình 2018 — chọn tổ hợp có GDKTPL từ lớp 10 giúp làm quen sớm với tư duy pháp lý.',
   traits:['phan-tich','dong-cam','chinh-xac','kien-nhan']},

  {id:'cokhi',    icon:'⚙️',ten:'Ô tô – Cơ khí – Điện – Tự động hóa',
   mo:'Người thích máy móc, kỹ thuật. Muốn thiết kế – lắp ráp – cải tiến hệ thống, động cơ.',
   tomtat:'Phù hợp với người thực tế, thích máy móc, có tư duy kỹ thuật và muốn tạo ra hoặc cải tiến các sản phẩm cơ khí – điện tử – tự động hóa.',
   dh:['A00: Toán – Vật lý – Hóa học','A01: Toán – Vật lý – Tiếng Anh','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Vật lý (bắt buộc)','Hóa học'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học (tổ hợp phổ biến nhất)','A01 → cần: Vật lý + Tiếng Anh','Vật lý là ưu tiên số 1 cho mọi ngành kỹ thuật'],
   truong:'ĐH Bách Khoa HN, ĐH Bách Khoa TP.HCM, ĐH SP Kỹ Thuật TP.HCM, ĐH Công Nghiệp HN, ĐH Công Nghiệp TP.HCM, ĐH Lạc Hồng (Đồng Nai)',
   warn:'Vật lý là môn BẮT BUỘC cho tất cả ngành Kỹ thuật – Cơ khí – Điện – Ô tô.',
   traits:['may-moc','phan-tich','chinh-xac','khoa-hoc']},

  {id:'xd',       icon:'🏛️',ten:'Xây dựng – Kiến trúc – Giao thông',
   mo:'Người có tư duy không gian, thích thiết kế – tính toán, quan tâm hạ tầng đô thị.',
   tomtat:'Phù hợp với người có tư duy không gian – kỹ thuật, cẩn thận và muốn góp phần xây dựng nhà cửa, đô thị, cầu đường phục vụ cộng đồng.',
   dh:['A00: Toán – Vật lý – Hóa học','V00: Toán – Vật lý – Vẽ kỹ thuật','A01: Toán – Vật lý – Tiếng Anh','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Vật lý (bắt buộc — nền tảng kỹ thuật)','Vẽ kỹ thuật (Kiến trúc — luyện thêm ngoài trường)'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học (Xây dựng — chủ lực)','V00 → CẦN luyện Vẽ kỹ thuật riêng (Kiến trúc — không có trong chương trình THPT)','A01 → cần: Vật lý + Tiếng Anh','D01 → hướng Quản lý dự án/Kinh tế xây dựng (không cần Vẽ)'],
   truong:'ĐH Kiến Trúc HN, ĐH Kiến Trúc TP.HCM, ĐH Xây Dựng HN, ĐH Giao Thông Vận Tải, ĐH Bách Khoa HN/HCM',
   warn:'Kiến trúc (V00) cần môn Vẽ kỹ thuật — không có trong chương trình THPT, phải luyện thêm bên ngoài. Xây dựng/Giao thông (A00/A01) không cần Vẽ.',
   traits:['may-moc','sang-tao','phan-tich','chinh-xac']},

  {id:'tkdh',     icon:'🎨',ten:'Thiết kế đồ họa – Game – Đa phương tiện',
   mo:'Người sáng tạo, nhạy hình ảnh, màu sắc. Thích thiết kế, animation, game, giao diện số.',
   tomtat:'Phù hợp với người sáng tạo, yêu hình ảnh, có gu thẩm mỹ và muốn tạo ra sản phẩm số như thiết kế, game, video hay animation.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','X01: Ngữ văn – Toán – GDKTPL','A00: Toán – Vật lý – Hóa học'],
   mon_txt:['Mỹ thuật (năng khiếu – luyện thêm)','GDKTPL (cho X01)'],
   tohop_l10:['D01 → cần: Tiếng Anh tốt','X01 → cần: GDKTPL lớp 10','CẦN thi NĂNG KHIẾU Vẽ riêng — luyện từ lớp 10'],
   truong:'ĐH Mỹ Thuật VN, ĐH Mỹ Thuật TP.HCM, FPT University (Design), ĐH Văn Lang, ĐH Kiến Trúc (TKNT)',
   warn:'Thiết kế đồ họa yêu cầu thi năng khiếu Vẽ riêng — cần chuẩn bị từ sớm ngay lớp 10.',
   traits:['sang-tao','thuc-hanh','phan-tich']},

  {id:'du-lich',  icon:'✈️',ten:'Du lịch – Khách sạn – Sự kiện',
   mo:'Người cởi mở, giao tiếp tốt, yêu dịch vụ. Thích tạo trải nghiệm tích cực cho người khác.',
   tomtat:'Phù hợp với người cởi mở, giao tiếp tốt, yêu dịch vụ và muốn tạo cảm giác hài lòng cho khách trong các hoạt động du lịch, lưu trú và sự kiện.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','C00: Ngữ văn – Lịch sử – Địa lý','C04: Ngữ văn – Toán – Địa lý'],
   mon_txt:['Tiếng Anh (bắt buộc)','Địa lý'],
   tohop_l10:['D01 → cần: Tiếng Anh tốt (quan trọng nhất)','C00 → cần: Lịch sử + Địa lý','C04 → cần: Địa lý (không cần Lịch sử)'],
   truong:'ĐH Khoa học Xã hội & Nhân văn HN/HCM, ĐH Đà Lạt, ĐH Hoa Sen, ĐH Văn Lang, ĐH Tôn Đức Thắng',
   warn:'Tiếng Anh giỏi là lợi thế cạnh tranh số 1 trong ngành Du lịch – Khách sạn.',
   traits:['giao-tiep','ngon-ngu','kien-nhan','dong-cam']},

  {id:'nlts',     icon:'🌱',ten:'Nông – Lâm – Thủy sản',
   mo:'Người yêu thiên nhiên, thích cây trồng, vật nuôi. Quan tâm nông nghiệp bền vững.',
   tomtat:'Phù hợp với người gần gũi thiên nhiên, thích sinh học – môi trường và muốn tạo giá trị thông qua nông nghiệp, thủy sản, lâm nghiệp và phát triển bền vững.',
   dh:['B00: Toán – Hóa học – Sinh học','D01: Toán – Ngữ văn – Tiếng Anh','B03: Toán – Sinh học – Ngữ văn'],
   mon_txt:['Hóa học','Sinh học'],
   tohop_l10:['B00 → cần: Hóa học + Sinh học (tổ hợp chủ lực)','B03 → cần: Sinh học','Môn CN Nông nghiệp lớp 10 là lợi thế đặc thù'],
   truong:'ĐH Nông Lâm TP.HCM, ĐH Nông Nghiệp HN, ĐH Cần Thơ, ĐH Nha Trang (Thủy sản), ĐH Lâm Nghiệp',
   warn:'',traits:['tu-nhien','kien-nhan','khoa-hoc']},

  {id:'tl',       icon:'💙',ten:'Tâm lý – Công tác xã hội',
   mo:'Người đồng cảm, biết lắng nghe, nhạy cảm cảm xúc. Thích hỗ trợ sức khỏe tinh thần.',
   tomtat:'Phù hợp với người đồng cảm, sâu sắc, biết lắng nghe và muốn tạo giá trị thông qua hỗ trợ sức khỏe tinh thần, tham vấn, giáo dục hay phát triển con người.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','C00: Ngữ văn – Lịch sử – Địa lý','C03: Ngữ văn – Toán – Lịch sử'],
   mon_txt:['Tiếng Anh','Địa lý + Lịch sử (nếu học C00)'],
   tohop_l10:['D01 → cần: Tiếng Anh tốt','C00 → cần: Địa lý + Lịch sử','C03 → cần: Lịch sử'],
   truong:'ĐH KHXH&NV HN, ĐH KHXH&NV TP.HCM, ĐH SP HN (Tâm lý GD), ĐH Văn Hiến, ĐH Mở TP.HCM',
   warn:'',traits:['giup-do','dong-cam','kien-nhan','giao-tiep']},

  {id:'ngoai-giao',icon:'🌐',ten:'Ngoại giao – Ngoại ngữ – Ngoại thương',
   mo:'Người yêu ngôn ngữ, nhạy văn hóa. Thích kết nối quốc tế, xuất nhập khẩu, kinh tế toàn cầu.',
   tomtat:'Phù hợp với người giỏi ngôn ngữ, thích kết nối, hiểu văn hóa và muốn tạo cầu nối giữa con người, tổ chức hoặc quốc gia trong môi trường quốc tế.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','D14: Ngữ văn – Lịch sử – Tiếng Anh','D15: Ngữ văn – Địa lý – Tiếng Anh'],
   mon_txt:['Tiếng Anh (quan trọng nhất)','Địa lý hoặc Lịch sử'],
   tohop_l10:['D01 → cần: Tiếng Anh ≥ 8.5 điểm','D15 → cần: Địa lý + Tiếng Anh','D14 → cần: Lịch sử + Tiếng Anh'],
   truong:'HV Ngoại Giao, ĐH Ngoại Thương, ĐH Ngoại Ngữ – ĐHQG HN, ĐH KHXH&NV HN/HCM, ĐH Hà Nội',
   warn:'Tiếng Anh ≥ 8.5/10 là yêu cầu thực tế cho Ngoại ngữ – Ngoại giao tại các trường top.',
   traits:['ngon-ngu','dong-cam','giao-tiep','kien-nhan']},

  {id:'nt',       icon:'🎵',ten:'Mỹ thuật – Âm nhạc – Nghệ thuật',
   mo:'Người giàu cảm xúc, nhạy cái đẹp, muốn thể hiện qua hội họa, âm nhạc, biểu diễn.',
   tomtat:'Phù hợp với người sáng tạo, nhạy cảm thẩm mỹ, có năng khiếu nghệ thuật và muốn tạo ra giá trị thông qua cái đẹp, cảm xúc hay tác phẩm sáng tạo.',
   dh:['H00: Ngữ văn – NK Vẽ 1 – NK Vẽ 2','N00: Ngữ văn – Hòa âm – Hát','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Âm nhạc hoặc Mỹ thuật (năng khiếu — bắt buộc luyện sớm)'],
   tohop_l10:['H00 → CẦN luyện năng khiếu Vẽ từ lớp 10','N00 → CẦN luyện Âm nhạc chuyên sâu (★ khớp tên ngành Âm nhạc)','D01 → hướng quản lý/lý luận nghệ thuật (không cần năng khiếu)'],
   truong:'HV Âm Nhạc Quốc Gia VN, ĐH Mỹ Thuật VN, ĐH Sân Khấu Điện Ảnh HN/HCM, ĐH Văn Hóa HN/HCM',
   warn:'Cần luyện năng khiếu chuyên sâu từ sớm — không thể bổ sung ngắn hạn trước kỳ thi.',
   traits:['sang-tao','kien-nhan','dong-cam']},

  {id:'khtn',     icon:'🔬',ten:'Khoa học tự nhiên – Công nghệ sinh–hóa',
   mo:'Người tò mò, thích khám phá bản chất sự vật. Quan tâm Vật lý, Hóa học, Sinh học nghiên cứu.',
   tomtat:'Phù hợp với người ham học hỏi, thích nghiên cứu, có tư duy khoa học và muốn tạo ra tri thức hoặc ứng dụng khoa học vào đời sống, công nghệ và môi trường.',
   dh:['B00: Toán – Hóa học – Sinh học','A00: Toán – Vật lý – Hóa học','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Hóa học','Sinh học','Vật lý'],
   tohop_l10:['B00 → cần: Hóa học + Sinh học (CN Sinh–Hóa, Thực phẩm)','A00 → cần: Vật lý + Hóa học','Nên học ít nhất 3 môn KHTN để linh hoạt'],
   truong:'ĐH Khoa học TN HN, ĐH Khoa học TN TP.HCM, ĐH Bách Khoa HN/HCM, ĐH Cần Thơ, ĐH Nông Lâm HCM',
   warn:'',traits:['khoa-hoc','phan-tich','kien-nhan','so-lieu']},

  {id:'quan-doi', icon:'🎖️',ten:'Công an – Quân đội – An ninh',
   mo:'Người kỷ luật, bản lĩnh, trách nhiệm cao. Sẵn sàng phục vụ Tổ quốc, giữ trật tự xã hội.',
   tomtat:'Phù hợp với người kỷ luật, dũng cảm, yêu nước và mong muốn đóng góp cho an ninh, quốc phòng và trật tự xã hội.',
   dh:['A01: Toán – Vật lý – Tiếng Anh','A00: Toán – Vật lý – Hóa học','Q00: Tư duy định lượng – Định tính – KH/Tiếng Anh'],
   mon_txt:['Vật lý (kỹ thuật quân sự)','Lịch sử (chính trị–an ninh)'],
   tohop_l10:['A01 → cần: Vật lý + Tiếng Anh','A00 → cần: Vật lý + Hóa học','Ngoài học lực: sức khỏe tốt + sơ tuyển thể lực riêng'],
   truong:'HV Cảnh Sát Nhân Dân, HV An Ninh Nhân Dân, HV Kỹ Thuật Quân Sự, ĐH Phòng Cháy Chữa Cháy, ĐH Trần Quốc Tuấn',
   warn:'Ngoài học lực, cần sức khỏe tốt, lý lịch trong sáng và vượt sơ tuyển thể lực riêng.',
   traits:['ky-luat','kien-nhan','dong-cam']},

  // ── NHÓM NGÀNH BỔ SUNG (từ 36 chân dung HNA) ──────────────────────

  {id:'ke-toan',   icon:'🧾',ten:'Kế toán – Kiểm toán',
   mo:'Người cẩn thận, tỉ mỉ, có tư duy hệ thống và coi trọng sự chính xác trong từng con số.',
   tomtat:'Phù hợp với người ngăn nắp, kiên nhẫn, trung thực, thích số liệu – chứng từ – quy trình và muốn đảm bảo tính minh bạch tài chính cho tổ chức.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','A00: Toán – Vật lý – Hóa học','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Toán (cốt lõi)','Tiếng Anh'],
   tohop_l10:['D01 → cần: Tiếng Anh tốt (phổ biến nhất)','D07 → cần: Hóa học + Tiếng Anh (★ dùng chung nhiều ngành Kinh tế)','A00 → cần: Vật lý + Hóa học'],
   truong:'HV Tài Chính, ĐH Kinh Tế Quốc Dân, ĐH Kinh Tế TP.HCM (UEH), ĐH Thăng Long, ĐH Đồng Nai',
   warn:'',traits:['chinh-xac','so-lieu','kien-nhan','ky-luat']},

  {id:'ban-dan',   icon:'💡',ten:'Công nghiệp bán dẫn',
   mo:'Người có tư duy logic–kỹ thuật tốt, thích tìm hiểu cách thiết bị điện tử vận hành và kiên trì với vấn đề phức tạp.',
   tomtat:'Phù hợp với người giỏi tư duy logic, thích công nghệ lõi, kiên trì và muốn tham gia lĩnh vực công nghệ cao mang tính chiến lược.',
   dh:['A00: Toán – Vật lý – Hóa học','A01: Toán – Vật lý – Tiếng Anh','X06: Toán – Vật lý – Tin học'],
   mon_txt:['Vật lý (bắt buộc)','Toán nền tảng vững'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học','A01 → cần: Vật lý + Tiếng Anh','X06 → cần: Vật lý + Tin học (MỚI 2025)'],
   truong:'ĐH Bách Khoa HN/HCM, ĐH Công Nghệ ĐHQG HN, ĐH RMIT, FPT University',
   warn:'🤖 Bán dẫn là ngành chiến lược quốc gia 2026 — nhu cầu nhân lực rất cao, học bổng nhiều.',
   traits:['phan-tich','may-moc','khoa-hoc','kien-nhan']},

  {id:'ngoai-thuong',icon:'🌍',ten:'Ngoại thương – Xuất nhập khẩu',
   mo:'Người năng động, thích môi trường quốc tế và có tư duy kinh doanh xuyên biên giới.',
   tomtat:'Phù hợp với người giỏi ngoại ngữ, năng động, thích kinh doanh quốc tế và muốn kết nối thị trường Việt Nam với thế giới.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','A01: Toán – Vật lý – Tiếng Anh','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Tiếng Anh (quan trọng nhất)'],
   tohop_l10:['D01 → cần: Tiếng Anh ≥ 8.0','A01 → cần: Vật lý + Tiếng Anh'],
   truong:'ĐH Ngoại Thương HN/HCM, ĐH Kinh Tế Quốc Dân, ĐH Kinh Tế TP.HCM (UEH)',
   warn:'',traits:['ngon-ngu','giao-tiep','kinh-doanh','phan-tich']},

  {id:'dien-tu',   icon:'⚡',ten:'Điện – Điện tử – Tự động hóa',
   mo:'Người thích kỹ thuật, mạch điện, thiết bị điện và muốn hiểu cách các hệ thống vận hành.',
   tomtat:'Phù hợp với người thực tế, thích công nghệ kỹ thuật, khéo tay và muốn làm việc với thiết bị điện–điện tử–tự động hóa trong đời sống và sản xuất.',
   dh:['A00: Toán – Vật lý – Hóa học','A01: Toán – Vật lý – Tiếng Anh'],
   mon_txt:['Vật lý (bắt buộc)','Hóa học'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học (tổ hợp chủ lực)','Vật lý là nền tảng bắt buộc của ngành Điện'],
   truong:'ĐH Bách Khoa HN/HCM, ĐH Điện Lực, ĐH Công Nghiệp HN/HCM, ĐH SP Kỹ Thuật HCM, ĐH Lạc Hồng',
   warn:'',traits:['may-moc','thuc-hanh','phan-tich','chinh-xac']},

  {id:'hang-khong',icon:'✈️',ten:'Hàng không – Vũ trụ – Hạt nhân',
   mo:'Người có tư duy logic mạnh, yêu thích khoa học–công nghệ cao và thích giải quyết bài toán phức tạp với độ chính xác tuyệt đối.',
   tomtat:'Phù hợp với người giỏi tư duy khoa học, kỷ luật, chính xác và muốn tham gia các lĩnh vực chiến lược như hàng không, không gian và năng lượng hạt nhân.',
   dh:['A00: Toán – Vật lý – Hóa học','A01: Toán – Vật lý – Tiếng Anh','X06: Toán – Vật lý – Tin học'],
   mon_txt:['Vật lý (nền tảng cốt lõi)','Toán cao'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học','A01 → cần: Vật lý + Tiếng Anh'],
   truong:'HV Hàng Không VN, ĐH Bách Khoa HN, ĐH Công Nghệ ĐHQG HN, ĐH Giao Thông Vận Tải',
   warn:'Điểm chuẩn rất cao, yêu cầu sức khỏe đặc biệt (phi công), hoặc nền tảng KHTN rất vững.',
   traits:['khoa-hoc','ky-luat','chinh-xac','kien-nhan']},

  {id:'vat-lieu',  icon:'🔩',ten:'Công nghệ vật liệu',
   mo:'Người thích khoa học ứng dụng, tò mò về cấu tạo của vật chất và muốn tạo ra vật liệu mới phục vụ sản xuất và công nghệ cao.',
   tomtat:'Phù hợp với người thích khoa học tự nhiên, có tư duy nghiên cứu–kỹ thuật và muốn tạo ra hoặc cải tiến vật liệu cho công nghiệp, y sinh, năng lượng hay công nghệ cao.',
   dh:['A00: Toán – Vật lý – Hóa học','B00: Toán – Hóa học – Sinh học'],
   mon_txt:['Hóa học (cốt lõi)','Vật lý'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học','B00 → cần: Hóa học + Sinh học (CN vật liệu sinh học)'],
   truong:'ĐH Bách Khoa HN/HCM, ĐH Khoa học TN HN/HCM, ĐH Công Nghệ ĐHQG HN',
   warn:'',traits:['khoa-hoc','phan-tich','chinh-xac','kien-nhan']},

  {id:'thuc-pham', icon:'🍽️',ten:'Công nghệ thực phẩm – Dinh dưỡng',
   mo:'Người thích khoa học ứng dụng, quan tâm đến thực phẩm, dinh dưỡng và quy trình sản xuất.',
   tomtat:'Phù hợp với người cẩn thận, thích khoa học–thực phẩm–sản xuất và muốn tạo ra các sản phẩm ăn uống an toàn, dinh dưỡng và có giá trị cho cộng đồng.',
   dh:['B00: Toán – Hóa học – Sinh học','A00: Toán – Vật lý – Hóa học','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Hóa học (bắt buộc)','Sinh học'],
   tohop_l10:['B00 → cần: Hóa học + Sinh học (chủ lực thực phẩm–dinh dưỡng)','A00 → cần: Vật lý + Hóa học'],
   truong:'ĐH Bách Khoa HN/HCM, ĐH Nông Lâm HCM, ĐH Công Nghiệp HCM, ĐH Cần Thơ',
   warn:'',traits:['khoa-hoc','chinh-xac','kien-nhan','thuc-hanh']},

  {id:'hang-hai',  icon:'⚓',ten:'Hàng hải – Thủy lợi – Thời tiết',
   mo:'Người thích thiên nhiên, kỹ thuật, môi trường nước và khí hậu. Quan tâm đến tàu biển, cảng biển, đê điều, thủy lợi, dự báo thời tiết.',
   tomtat:'Phù hợp với người thực tế, thích kỹ thuật–thiên nhiên và muốn góp phần vào vận tải biển, quản lý nguồn nước, phòng chống thiên tai hay dự báo thời tiết.',
   dh:['A00: Toán – Vật lý – Hóa học (phổ biến nhất)','A01: Toán – Vật lý – Tiếng Anh','C01: Ngữ văn – Toán – Vật lý','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Vật lý (bắt buộc — nền tảng kỹ thuật)','Hóa học (A00)','Tiếng Anh (A01 — xu hướng nhiều trường)'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học (chủ lực)','A01 → cần: Vật lý + Tiếng Anh (xu hướng 2025–2026)','C01 → cần: Vật lý (Hàng hải–Thủy lợi)'],
   truong:'ĐH Hàng Hải VN (Hải Phòng), ĐH Thủy Lợi HN, ĐH Tài Nguyên & Môi Trường HN/HCM, ĐH Bách Khoa HN/HCM',
   warn:'A01 (Toán–Lý–Anh) đang được nhiều trường kỹ thuật mở rộng và ưu tiên hơn A00 — nên cân nhắc giữ Tiếng Anh tốt.',traits:['tu-nhien','may-moc','thuc-hanh','kien-nhan']},

  {id:'mo-dia',    icon:'⛏️',ten:'Mỏ – Địa chất',
   mo:'Người thích khám phá tự nhiên, đất đá, tài nguyên và bản đồ địa hình.',
   tomtat:'Phù hợp với người thực tế, thích thiên nhiên–tài nguyên–kỹ thuật và muốn góp phần vào khai thác tài nguyên, khảo sát địa chất hay bảo vệ môi trường địa chất.',
   dh:['A00: Toán – Vật lý – Hóa học','C01: Ngữ văn – Toán – Vật lý'],
   mon_txt:['Vật lý','Hóa học','Địa lý'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học','Môn Địa lý lớp 10 là lợi thế'],
   truong:'ĐH Mỏ–Địa Chất HN, ĐH Tài Nguyên & Môi Trường HN/HCM, ĐH Khoa học TN HN/HCM',
   warn:'',traits:['tu-nhien','thuc-hanh','kien-nhan','phan-tich']},

  {id:'toan-tk',   icon:'📐',ten:'Toán học – Thống kê – Khoa học dữ liệu',
   mo:'Người có tư duy logic tốt, thích tìm quy luật và giải quyết vấn đề bằng con số–mô hình–lập luận chặt chẽ.',
   tomtat:'Phù hợp với người logic, kiên nhẫn, thích con số–dữ liệu–quy luật và muốn dùng toán học, thống kê để phân tích, dự báo hay hỗ trợ ra quyết định trong nhiều lĩnh vực.',
   dh:['A00: Toán – Vật lý – Hóa học','A01: Toán – Vật lý – Tiếng Anh','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Toán (nền tảng tuyệt đối)','Tin học (Khoa học dữ liệu)'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học','A01 → cần: Vật lý + Tiếng Anh','Nên chọn Tin học → hướng Data Science'],
   truong:'ĐH Khoa học TN HN/HCM, ĐH Bách Khoa HN, ĐH Kinh Tế Quốc Dân, ĐH Sư Phạm HN',
   warn:'',traits:['so-lieu','phan-tich','kien-nhan','noi-tam']},

  {id:'nhan-su',   icon:'👥',ten:'Nhân sự – Hành chính – Quản trị văn phòng',
   mo:'Người cẩn thận, có trách nhiệm và thích làm việc với con người. Quan tâm đến tuyển dụng, đào tạo, văn hóa doanh nghiệp.',
   tomtat:'Phù hợp với người ngăn nắp, trách nhiệm, giao tiếp tốt và muốn tạo giá trị thông qua tuyển dụng, đào tạo, hành chính và xây dựng môi trường làm việc hiệu quả.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','C00: Ngữ văn – Lịch sử – Địa lý','X01: Ngữ văn – Toán – GDKTPL','A01: Toán – Vật lý – Tiếng Anh'],
   mon_txt:['Tiếng Anh','GDKTPL (luật lao động, quản trị hành chính)','Giao tiếp – Văn bản hành chính'],
   tohop_l10:['D01 → cần: Tiếng Anh tốt (phổ biến nhất)','X01 → cần: GDKTPL (hỗ trợ luật lao động, hành chính)','C00 → cần: Địa lý + Lịch sử'],
   truong:'ĐH Kinh Tế QD, ĐH Kinh Tế HCM (UEH), ĐH Lao Động Xã Hội, ĐH Văn Lang, ĐH HUTECH',
   warn:'',traits:['giao-tiep','kien-nhan','chinh-xac','dong-cam']},

  {id:'van-hoa',   icon:'🏛️',ten:'Văn hóa – Chính trị – Khoa học xã hội',
   mo:'Người quan tâm đến con người, xã hội, lịch sử và văn hóa. Thích tìm hiểu về hành vi xã hội, chính sách, cộng đồng.',
   tomtat:'Phù hợp với người sâu sắc, ham hiểu biết, thích tìm hiểu con người–xã hội–chính sách và muốn tạo giá trị thông qua nghiên cứu, truyền thông hay công tác xã hội.',
   dh:['C00: Ngữ văn – Lịch sử – Địa lý','D01: Toán – Ngữ văn – Tiếng Anh','X70: Ngữ văn – Lịch sử – GDKTPL','C03: Ngữ văn – Toán – Lịch sử'],
   mon_txt:['Lịch sử (cốt lõi)','GDKTPL (chính trị, chính sách, pháp luật)','Địa lý','Ngữ văn'],
   tohop_l10:['C00 → cần: Địa lý + Lịch sử (chủ lực)','X70 → cần: Lịch sử + GDKTPL (rất hợp hướng Chính trị – Chính sách)','D01 → cần: Tiếng Anh tốt'],
   truong:'ĐH KHXH&NV HN/HCM, HV Báo Chí & TT, ĐH Văn Hóa HN/HCM, HV Chính Trị QG HCM',
   warn:'',traits:['ngon-ngu','dong-cam','noi-tam','xa-hoi']},

  {id:'the-thao',  icon:'🏆',ten:'Thể dục – Thể thao',
   mo:'Người yêu vận động, có tinh thần kỷ luật, sức bền tốt và thích rèn luyện cơ thể nghiêm túc.',
   tomtat:'Phù hợp với người năng động, kỷ luật, yêu vận động và muốn tạo giá trị thông qua sức khỏe, thể chất, tinh thần thể thao và lối sống tích cực.',
   dh:['T00: Toán – Sinh học – Năng khiếu TDTT','T01: Toán – Ngữ văn – Năng khiếu TDTT','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Thi năng khiếu TDTT riêng','Sinh học (Huấn luyện–Y học thể thao)'],
   tohop_l10:['T00/T01 → CẦN thi năng khiếu TDTT riêng tại trường','D01 → hướng Quản lý thể thao, Giáo dục thể chất'],
   truong:'ĐH SP TDTT HN, ĐH SP TDTT TP.HCM, ĐH SP TDTT Đà Nẵng',
   warn:'Cần có thành tích thi đấu thể thao hoặc vượt qua bài thi năng khiếu TDTT.',
   traits:['ky-luat','kien-nhan','thuc-hanh','giup-do']},

  {id:'thoi-trang',icon:'👗',ten:'Thời trang – May mặc',
   mo:'Người nhạy với cái đẹp, màu sắc, chất liệu và thích tạo ra sản phẩm mang tính thẩm mỹ–ứng dụng.',
   tomtat:'Phù hợp với người sáng tạo, tỉ mỉ, yêu cái đẹp và muốn tạo ra các sản phẩm thời trang vừa có tính thẩm mỹ vừa có giá trị sử dụng trong đời sống.',
   dh:['H00: Ngữ văn – Năng khiếu 1 – Năng khiếu 2','C00: Ngữ văn – Lịch sử – Địa lý','D01: Toán – Ngữ văn – Tiếng Anh'],
   mon_txt:['Mỹ thuật (năng khiếu–thi riêng)','Tư duy thẩm mỹ'],
   tohop_l10:['H00 → CẦN luyện năng khiếu Vẽ từ lớp 10','D01 → hướng Thiết kế + Kinh doanh thời trang'],
   truong:'ĐH Mỹ Thuật Công Nghiệp HN, ĐH Công Nghiệp Dệt May HN, ĐH Kiến Trúc TP.HCM',
   warn:'Cần luyện năng khiếu vẽ và tư duy thẩm mỹ từ lớp 10.',
   traits:['sang-tao','chinh-xac','hinh-anh','kien-nhan']},

  {id:'in-giay',   icon:'🖨️',ten:'Công nghệ In – Giấy – Bao bì',
   mo:'Người cẩn thận, thực tế và quan tâm đến vật liệu, màu sắc, bao bì và các sản phẩm in ấn.',
   tomtat:'Phù hợp với người thực tế, tỉ mỉ, thích sản xuất–thiết kế ứng dụng và muốn tạo ra các sản phẩm in ấn, bao bì có chất lượng và tính thẩm mỹ.',
   dh:['A00: Toán – Vật lý – Hóa học','C01: Ngữ văn – Toán – Vật lý'],
   mon_txt:['Hóa học (mực in, vật liệu)','Vật lý'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học'],
   truong:'ĐH Bách Khoa HN, ĐH Sư Phạm Kỹ Thuật TP.HCM, ĐH Công Nghiệp HN/HCM',
   warn:'',traits:['chinh-xac','thuc-hanh','sang-tao','kien-nhan']},

  {id:'tai-nguyen',icon:'🌿',ten:'Tài nguyên – Môi trường',
   mo:'Người quan tâm đến thiên nhiên, đất, nước, không khí và các vấn đề ô nhiễm–biến đổi khí hậu–phát triển bền vững.',
   tomtat:'Phù hợp với người yêu thiên nhiên, có tư duy khoa học và muốn góp phần bảo vệ tài nguyên, cải thiện chất lượng sống và hướng tới phát triển bền vững.',
   dh:['A00: Toán – Vật lý – Hóa học','B00: Toán – Hóa học – Sinh học','D07: Toán – Hóa học – Tiếng Anh'],
   mon_txt:['Hóa học','Sinh học','Địa lý'],
   tohop_l10:['A00 → cần: Vật lý + Hóa học','B00 → cần: Hóa học + Sinh học (KH môi trường)','Môn Địa lý lớp 10 rất có ích'],
   truong:'ĐH Tài Nguyên & Môi Trường HN/HCM, ĐH Khoa học TN HN/HCM, ĐH Nông Lâm HCM',
   warn:'',traits:['tu-nhien','khoa-hoc','phan-tich','kien-nhan']},

  {id:'cham-soc',  icon:'💆',ten:'Chăm sóc sắc đẹp – Gia đình',
   mo:'Người khéo léo, tinh tế và thích chăm sóc con người. Hứng thú với làm đẹp, da–tóc–móng, spa, trang điểm, dinh dưỡng.',
   tomtat:'Phù hợp với người chu đáo, khéo tay, yêu cái đẹp và muốn tạo giá trị thông qua việc giúp con người đẹp hơn, khỏe hơn và có cuộc sống sinh hoạt tốt hơn.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','B00: Toán – Hóa học – Sinh học','C00: Ngữ văn – Lịch sử – Địa lý'],
   mon_txt:['Sinh học (cơ sở chăm sóc da–dinh dưỡng)','Hóa học (mỹ phẩm)'],
   tohop_l10:['D01 → cần: Tiếng Anh tốt (phổ biến nhất)','B00 → cần: Hóa học + Sinh học (★ khớp trực tiếp với môn lớp 10 — hướng dinh dưỡng, mỹ phẩm)'],
   truong:'ĐH Công Nghệ TP.HCM (HUTECH), ĐH Văn Lang, ĐH Nguyễn Tất Thành, Cao đẳng nghề thẩm mỹ',
   warn:'Nhiều trường đào tạo hệ Cao đẳng nghề — nhanh ra nghề, chi phí thấp.',
   traits:['giup-do','dong-cam','chinh-xac','sang-tao']},

  {id:'cong-tac-xa-hoi',icon:'🤝',ten:'Công tác xã hội – Xã hội học',
   mo:'Người quan tâm đến cộng đồng, bảo trợ xã hội, trẻ em, người yếu thế và mong muốn góp phần cải thiện đời sống xã hội.',
   tomtat:'Phù hợp với người đồng cảm, trách nhiệm, biết lắng nghe và muốn tạo giá trị thông qua hỗ trợ cộng đồng, chính sách xã hội hay công tác nhân đạo.',
   dh:['D01: Toán – Ngữ văn – Tiếng Anh','C00: Ngữ văn – Lịch sử – Địa lý','X70: Ngữ văn – Lịch sử – GDKTPL','C03: Ngữ văn – Toán – Lịch sử','X35: Toán – Lịch sử – GDKTPL'],
   mon_txt:['Ngữ văn (giao tiếp–viết)','Địa lý + Lịch sử','GDKTPL (chính sách xã hội, pháp luật)'],
   tohop_l10:['C00 → cần: Địa lý + Lịch sử','X70 → cần: Lịch sử + GDKTPL (rất phù hợp — chính sách & pháp luật xã hội)','D01 → cần: Tiếng Anh tốt (CTXH quốc tế)'],
   truong:'ĐH KHXH&NV HN/HCM, ĐH Lao Động Xã Hội HN/HCM, ĐH Đà Lạt',
   warn:'GDKTPL (Kinh tế & Pháp luật) là môn rất phù hợp với CTXH — giúp hiểu chính sách xã hội, luật bảo trợ, quyền trẻ em.',
   traits:['giup-do','dong-cam','ngon-ngu','kien-nhan']},

  {id:'bac-si-thu-y',icon:'🐾',ten:'Bác sĩ thú y',
   mo:'Người yêu động vật, cẩn thận, kiên nhẫn và có tinh thần trách nhiệm cao với sức khỏe vật nuôi và cộng đồng.',
   tomtat:'Phù hợp với người yêu động vật, học tốt các môn tự nhiên, cẩn trọng và muốn chăm sóc–điều trị sức khỏe động vật cũng như bảo vệ cộng đồng khỏi dịch bệnh.',
   dh:['B00: Toán – Hóa học – Sinh học','B03: Toán – Sinh học – Ngữ văn','A00: Toán – Vật lý – Hóa học'],
   mon_txt:['Sinh học (bắt buộc)','Hóa học'],
   tohop_l10:['B00 → PHẢI có: Hóa học + Sinh học (tổ hợp chủ lực)','B03 → cần: Sinh học','Sinh học là môn cốt lõi không thể thiếu'],
   truong:'ĐH Nông Lâm TP.HCM, ĐH Nông Nghiệp HN, ĐH Cần Thơ, ĐH Nha Trang',
   warn:'Sinh học là môn BẮT BUỘC cho ngành Bác sĩ thú y.',
   traits:['giup-do','tu-nhien','khoa-hoc','kien-nhan']},
];

const SCHOOLS={
  'B00':[
    {ten:'THPT Ngô Quyền',    t:'Tổ hợp A: Lý, Hóa, Sinh, Tin — có Sinh học'},
    {ten:'THPT Chu Văn An',   t:'Tổ hợp A/B: Lý,Hóa,Sinh,Tin hoặc Lý,Hóa,Sinh,CN'},
  ],
  'A00':[
    {ten:'THPT Ngô Quyền',    t:'Tổ hợp A: Lý, Hóa, Sinh, Tin'},
    {ten:'THPT Trấn Biên',    t:'Tổ hợp A: Lý, Hóa, Tin + 1 môn'},
    {ten:'THPT Nguyễn Trãi',  t:'Cần xác nhận — SĐT: 0251 3884 351'},
    {ten:'THPT Lê Hồng Phong',t:'Cần xác nhận — lehongphongdongnai.edu.vn'},
  ],
  'D07':[
    {ten:'THPT Ngô Quyền',    t:'Tổ hợp A: Lý, Hóa, Sinh, Tin — có Hóa học'},
    {ten:'THPT Chu Văn An',   t:'Tổ hợp A: Lý, Hóa, Sinh, Tin'},
  ],
  'D01':[
    {ten:'THPT Ngô Quyền',    t:'Tổ hợp B/C: Hóa,Sinh,GDKTPL,CN hoặc Địa,CN,Tin,GDKTPL'},
    {ten:'THPT Trấn Biên',    t:'Tổ hợp C: Địa, GDKTPL, Tin, Công nghệ'},
    {ten:'THPT Chu Văn An',   t:'Tổ hợp C/D: Tin,Địa,GDKTPL,CN công nghiệp/nông nghiệp'},
  ],
  'C00':[
    {ten:'THPT Ngô Quyền',    t:'Tổ hợp C: Địa, CN, Tin, GDKTPL'},
    {ten:'THPT Trấn Biên',    t:'Tổ hợp C: Địa, GDKTPL, Tin, Công nghệ'},
    {ten:'THPT Chu Văn An',   t:'Tổ hợp C/D: Tin, Địa, GDKTPL, CN nông nghiệp'},
  ],
};

let selT=new Set(),selN=null;

function buildTraits(){
  document.getElementById('trait-grid').innerHTML=
    TRAITS.map(t=>`<button class="tbtn" id="tb-${t.id}" onclick="toggleT('${t.id}')">${t.label}</button>`).join('');
}

function toggleT(id){
  if(selT.has(id)){selT.delete(id);document.getElementById('tb-'+id).classList.remove('sel')}
  else{selT.add(id);document.getElementById('tb-'+id).classList.add('sel')}
  const n=selT.size;
  document.getElementById('sbar-txt').textContent=n===0?'Chưa chọn gì — hãy chọn ít nhất 2 mô tả bản thân':`Đã chọn ${n} mô tả bản thân`;
  document.getElementById('sbar-cnt').textContent=n;
  const b=document.getElementById('btn12');b.disabled=n<2;
}

function scoreNganh(){
  return NGANH.map(n=>{
    let s=0;n.traits.forEach(t=>{if(selT.has(t))s++});return{...n,s};
  }).sort((a,b)=>b.s-a.s);
}

let saOpenId=null;

let nganhSearchQuery='';

function nganhSearchInput(v){
  nganhSearchQuery=v;
  buildNganh();
}

function buildNganh(){
  const sc=scoreNganh();
  const q=nganhSearchQuery.trim().toLowerCase();
  const countEl=document.getElementById('nganh-search-count');
  let shown, isSearching=false;
  if(q){
    isSearching=true;
    shown=sc.filter(n=>n.ten.toLowerCase().includes(q)||n.tomtat.toLowerCase().includes(q));
    if(countEl)countEl.textContent=`${shown.length}/36`;
  } else {
    shown=sc.slice(0,12);
    if(countEl)countEl.textContent='';
  }
  if(shown.length===0){
    document.getElementById('nganh-grid').innerHTML=`<div style="padding:1.5rem;text-align:center;font-size:13px;color:var(--text3)">Không tìm thấy nhóm ngành phù hợp với "<strong>${nganhSearchQuery}</strong>".<br>Hãy thử từ khóa khác hoặc xóa ô tìm kiếm để xem 12 ngành gợi ý.</div>`;
    return;
  }
  document.getElementById('nganh-grid').innerHTML=shown.map(n=>{
    const mc=n.s,mt=n.traits.length;
    const isMatch=mc>=3;
    const lbl=mc>=3?'Rất phù hợp':mc>=2?'Phù hợp':mc>=1?'Tham khảo':'Tham khảo';
    const isOpen=saOpenId===n.id;
    const isSel=selN===n.id;
    const starTH=n.dh[0].split(':')[0].trim();
    return`<div class="sa-item${isOpen?' open':''}${isSel?' selected':''}" id="sa-${n.id}">
      <button class="sa-head" onclick="saToggle('${n.id}')" aria-expanded="${isOpen}">
        <div class="sa-icon">${n.icon}</div>
        <div class="sa-info">
          <div class="sa-name">${n.ten}</div>
          <div class="sa-sub">${n.dh.slice(0,4).map(d=>d.split(':')[0]).join(' · ')}</div>
        </div>
        <div class="sa-right">
          <span class="sa-badge ${isMatch?'sa-badge-match':'sa-badge-ok'}">${lbl}</span>
          <div class="sa-sel-dot" title="Đã chọn"></div>
          <i class="ti ti-chevron-down sa-chev" aria-hidden="true"></i>
        </div>
      </button>
      <div class="sa-body">
        <div class="sa-mo">${n.tomtat}</div>
        <div class="sa-detail">
          <div class="sa-box">
            <div class="sa-blabel">Tổ hợp xét tuyển ĐH</div>
            <div class="sa-pills">
              ${n.dh.map(d=>{const code=d.split(':')[0].trim();return`<span class="sa-pill${code===starTH?' star':''}">${code}${code===starTH?' ★':''}</span>`}).join('')}
            </div>
          </div>
          <div class="sa-box">
            <div class="sa-blabel">Môn cần chú ý từ lớp 10</div>
            <div>${n.mon_txt.map(m=>`<div class="sa-mon-item">${m}</div>`).join('')}</div>
          </div>
          <div class="sa-box full">
            <div class="sa-blabel">Trường đào tạo tiêu biểu</div>
            <div class="sa-truong-list">${n.truong.split(',').map(t=>`<div class="sa-truong-item">${t.trim()}</div>`).join('')}</div>
          </div>
        </div>
        <div class="sa-foot">
          <button class="sa-btn-sel${isSel?' selected-state':''}" onclick="saSelect('${n.id}',event)">
            ${isSel?'✓ Đã chọn ngành này':'Chọn ngành này →'}
          </button>
          <button class="sa-btn-skip" onclick="saToggle('${n.id}')">Thu gọn</button>
        </div>
      </div>
    </div>`;
  }).join('');
}

function saToggle(id){
  saOpenId = saOpenId===id ? null : id;
  buildNganh();
  if(saOpenId){
    const el=document.getElementById('sa-'+saOpenId);
    if(el) el.scrollIntoView({behavior:'smooth',block:'nearest'});
  }
}

function saSelect(id,e){
  e&&e.stopPropagation();
  selN=id;
  saOpenId=id;
  buildNganh();
  const b=document.getElementById('btn23');
  b.disabled=false;
  setTimeout(()=>b.scrollIntoView({behavior:'smooth',block:'nearest'}),300);
}

function selNganh(id){
  selN=id;
  const b=document.getElementById('btn23');
  b.disabled=false;
}


const CO_HOI={
  'yd':       {jobs:['Bác sĩ đa khoa, chuyên khoa tại bệnh viện công/tư','Dược sĩ lâm sàng, nghiên cứu, kiểm định thuốc','Điều dưỡng, hộ lý tại cơ sở y tế','Nghiên cứu sinh y khoa, giảng viên y'],luong:'15–50 tr/tháng',nhu:'Rất cao — thiếu nhân lực y tế trầm trọng'},
  'cntt':     {jobs:['Lập trình viên phần mềm (web, ứng dụng, hệ thống)','Kỹ sư Trí tuệ nhân tạo, Khoa học dữ liệu','Chuyên gia An toàn thông tin, Bảo mật mạng','Quản lý sản phẩm, Phân tích nghiệp vụ CNTT'],luong:'15–60 tr/tháng',nhu:'Rất cao — nhu cầu tăng mạnh với AI & bán dẫn'},
  'kt-tc':    {jobs:['Chuyên viên phân tích tài chính, đầu tư','Kiểm toán viên, Kế toán trưởng','Chuyên gia Ngân hàng, tín dụng, bảo hiểm','Quản lý rủi ro, Kiểm soát tuân thủ'],luong:'12–40 tr/tháng',nhu:'Cao — tài chính số, công nghệ tài chính đang bùng nổ'},
  'kt-qtkd':  {jobs:['Trưởng phòng Marketing, Quản lý thương hiệu','Phát triển kinh doanh, Trưởng phòng Kinh doanh','Khởi nghiệp, điều hành doanh nghiệp','Chuyên viên tư vấn, Phân tích kinh doanh'],luong:'12–35 tr/tháng',nhu:'Cao — đặc biệt thương mại điện tử & xuất khẩu'},
  'spg':      {jobs:['Giáo viên THPT/THCS công lập và tư thục','Giảng viên đại học, cao đẳng','Chuyên viên giáo dục tại Sở GD&ĐT','Đào tạo nghiệp vụ tại doanh nghiệp, trung tâm'],luong:'8–20 tr/tháng',nhu:'Ổn định — nhu cầu giáo viên khối Khoa học-Kỹ thuật tăng'},
  'luat':     {jobs:['Luật sư tại văn phòng, công ty luật','Thẩm phán, Kiểm sát viên, Chấp hành viên','Chuyên viên pháp lý doanh nghiệp','Công chứng viên, Trọng tài thương mại'],luong:'15–60 tr/tháng',nhu:'Cao — đặc biệt Luật kinh tế, Luật quốc tế'},
  'cokhi':    {jobs:['Kỹ sư cơ khí, thiết kế máy, tự động hóa','Kỹ sư ô tô, điện, điện tử công nghiệp','Quản lý sản xuất, Kiểm soát chất lượng','Kỹ sư bảo trì, vận hành nhà máy'],luong:'12–35 tr/tháng',nhu:'Cao — đầu tư nước ngoài sản xuất tại Đồng Nai & Bình Dương'},
  'ngoai-giao':{jobs:['Cán bộ ngoại giao tại Bộ Ngoại giao','Phiên dịch, Biên dịch viên chuyên nghiệp','Chuyên gia quan hệ quốc tế tại tổ chức quốc tế','Chuyên viên xuất nhập khẩu, đầu tư nước ngoài'],luong:'15–40 tr/tháng',nhu:'Ổn định — ngoại ngữ hiếm (Nhật, Hàn) rất hot'},
  'hang-hai': {jobs:['Sỹ quan hàng hải, Thuyền trưởng, Thuyền phó','Kỹ sư khai thác cảng, logistics đường biển','Chuyên viên thủy lợi, quản lý nguồn nước','Dự báo viên khí tượng thủy văn Nhà nước'],luong:'15–60 tr/tháng',nhu:'Cao — thiếu nhân lực ngành biển và thủy lợi'},
  'tl':       {jobs:['Chuyên viên tâm lý lâm sàng tại bệnh viện','Tư vấn tâm lý học đường, trung tâm tham vấn','Nhân viên hỗ trợ xã hội, phát triển cộng đồng'],luong:'10–25 tr/tháng',nhu:'Tăng mạnh — sức khỏe tinh thần được quan tâm'},
  'xd':       {jobs:['Kỹ sư xây dựng, giám sát công trình','Kiến trúc sư thiết kế nội/ngoại thất','Kỹ sư cầu đường, hạ tầng đô thị','Quản lý dự án bất động sản'],luong:'12–40 tr/tháng',nhu:'Cao — đô thị hóa mạnh tại Đồng Nai/vùng ven'},
  'nlts':     {jobs:['Kỹ sư nông nghiệp, nuôi trồng thủy sản','Chuyên viên kiểm dịch, an toàn thực phẩm','Nghiên cứu viên giống cây trồng, vật nuôi','Quản lý trang trại, nông nghiệp công nghệ cao'],luong:'10–25 tr/tháng',nhu:'Tăng — nông nghiệp công nghệ cao, xuất khẩu'},
  'bao-chi':  {jobs:['Phóng viên, Biên tập viên báo/đài/trực tuyến','Sản xuất nội dung, Quản lý mạng xã hội','Chuyên viên truyền thông, Quan hệ công chúng','Chuyên viên tiếp thị số (digital marketing)'],luong:'10–30 tr/tháng',nhu:'Cao — nội dung số và tiếp thị số bùng nổ'},
  'ngoai-thuong':{jobs:['Chuyên viên xuất nhập khẩu, chứng từ ngoại thương','Nhân viên logistics, giao nhận quốc tế (Forwarder)','Chuyên viên thu mua quốc tế, phát triển nhà cung cấp','Đại diện thương mại tại văn phòng nước ngoài'],luong:'10–35 tr/tháng',nhu:'Cao — Việt Nam là trung tâm sản xuất-xuất khẩu của khu vực, nhu cầu logistics & FTA tăng mạnh'},
  'tkdh':     {jobs:['Thiết kế đồ họa, Thiết kế thương hiệu (Brand)','Lập trình & thiết kế Game (Game Designer)','Dựng phim, biên tập video, hoạt hình 2D/3D','Thiết kế UI/UX cho ứng dụng và website'],luong:'10–30 tr/tháng',nhu:'Cao — nội dung số, game, quảng cáo phát triển mạnh'},
  'du-lich':  {jobs:['Hướng dẫn viên du lịch, điều hành tour','Quản lý khách sạn, lễ tân, F&B','Tổ chức sự kiện, MICE, wedding planner','Chuyên viên booking, OTA, marketing du lịch'],luong:'8–25 tr/tháng',nhu:'Tăng mạnh — du lịch phục hồi sau dịch, FDI khách sạn-resort tăng'},
  'nt':       {jobs:['Họa sĩ minh họa, vẽ tranh, thiết kế mỹ thuật','Ca sĩ, nhạc sĩ, nhạc công, biểu diễn nghệ thuật','Giáo viên thanh nhạc/nhạc cụ/mỹ thuật','Giám tuyển nghệ thuật, quản lý nhà hát-bảo tàng'],luong:'8–25 tr/tháng (tùy năng lực & danh tiếng)',nhu:'Ổn định nhưng cạnh tranh cao — cần năng khiếu và đầu tư sớm'},
  'khtn':     {jobs:['Nghiên cứu viên tại viện Hóa-Sinh-Vật lý','Kỹ sư công nghệ sinh học, dược phẩm','Giảng viên đại học, giáo viên chuyên KHTN','Chuyên viên kiểm nghiệm, R&D doanh nghiệp'],luong:'10–30 tr/tháng',nhu:'Ổn định — nền tảng cho nhiều ngành công nghệ cao khác'},
  'quan-doi': {jobs:['Sĩ quan Quân đội, Công an các chuyên ngành','Cán bộ an ninh, điều tra, kỹ thuật quân sự','Giảng viên các học viện Quân đội-Công an','Chuyên viên an ninh mạng, phòng chống tội phạm công nghệ'],luong:'Theo lương Nhà nước + phụ cấp đặc thù',nhu:'Ổn định — biên chế Nhà nước, miễn học phí, có nơi ở'},
  'ke-toan':  {jobs:['Kế toán viên, Kế toán tổng hợp doanh nghiệp','Kiểm toán viên nội bộ/độc lập','Chuyên viên thuế, tư vấn tài chính-kế toán','Kế toán trưởng, Giám đốc tài chính (CFO) sau nhiều năm'],luong:'8–30 tr/tháng',nhu:'Ổn định — mọi doanh nghiệp đều cần kế toán, nhu cầu bền vững'},
  'ban-dan':  {jobs:['Kỹ sư thiết kế vi mạch (IC Design)','Kỹ sư kiểm thử, sản xuất bán dẫn (Wafer Fab)','Kỹ sư đóng gói-kiểm tra chip (ATP)','Chuyên viên R&D công nghệ bán dẫn tại tập đoàn FDI'],luong:'15–50 tr/tháng (mới ra trường có thể cao hơn nhiều ngành khác)',nhu:'Rất cao — Việt Nam đang là điểm đến đầu tư bán dẫn toàn cầu'},
  'dien-tu':  {jobs:['Kỹ sư điện, thiết kế-vận hành hệ thống điện','Kỹ sư điện tử, tự động hóa nhà máy','Kỹ sư bảo trì, lắp đặt thiết bị điện công nghiệp','Chuyên viên kỹ thuật tại nhà máy FDI (điện-điện tử)'],luong:'10–30 tr/tháng',nhu:'Cao — nhà máy điện tử, năng lượng tái tạo tại Đồng Nai-Bình Dương tăng'},
  'hang-khong':{jobs:['Kỹ sư bảo dưỡng máy bay, kỹ thuật hàng không','Phi công, tiếp viên hàng không (cần thi tuyển riêng)','Kiểm soát viên không lưu, điều hành bay','Kỹ sư nghiên cứu vũ trụ, vệ tinh, năng lượng hạt nhân'],luong:'15–60 tr/tháng (phi công có thể cao hơn nhiều)',nhu:'Ổn định — ngành đặc thù, ít trường đào tạo nên cạnh tranh nhưng nhu cầu thực luôn có'},
  'vat-lieu': {jobs:['Kỹ sư nghiên cứu-phát triển vật liệu mới','Kỹ sư kiểm soát chất lượng vật liệu sản xuất','Chuyên viên R&D tại nhà máy sản xuất linh kiện-vật liệu','Giảng viên, nghiên cứu viên vật liệu tại viện-trường'],luong:'10–28 tr/tháng',nhu:'Tăng — phục vụ ngành công nghiệp chế tạo, bán dẫn, ô tô điện'},
  'thuc-pham':{jobs:['Kỹ sư công nghệ thực phẩm tại nhà máy chế biến','Chuyên viên QA/QC an toàn thực phẩm','Chuyên viên R&D phát triển sản phẩm mới (F&B)','Chuyên gia dinh dưỡng, tư vấn sức khỏe-thực phẩm'],luong:'10–25 tr/tháng',nhu:'Cao — Việt Nam là nước xuất khẩu nông sản-thực phẩm lớn, cần chế biến sâu'},
  'mo-dia':   {jobs:['Kỹ sư khai thác mỏ, địa chất công trình','Chuyên viên khảo sát địa chất, địa hình','Kỹ sư môi trường mỏ, an toàn khai thác','Chuyên viên quản lý tài nguyên khoáng sản'],luong:'10–30 tr/tháng (nhiều vị trí có phụ cấp công trường)',nhu:'Ổn định — nhu cầu khai thác tài nguyên và xây dựng hạ tầng vẫn liên tục'},
  'toan-tk':  {jobs:['Chuyên viên phân tích dữ liệu (Data Analyst)','Chuyên gia khoa học dữ liệu, AI/Machine Learning','Chuyên viên thống kê-bảo hiểm (Actuary)','Giảng viên Toán-Thống kê tại trường ĐH-CĐ'],luong:'12–40 tr/tháng',nhu:'Rất cao — mọi ngành đều cần phân tích dữ liệu trong kỷ nguyên AI'},
  'nhan-su':  {jobs:['Chuyên viên tuyển dụng, đào tạo nhân sự (HR)','Chuyên viên hành chính-văn phòng, thư ký','Chuyên viên C&B (lương, thưởng, phúc lợi)','Trưởng phòng Nhân sự, Quản trị nguồn nhân lực'],luong:'8–25 tr/tháng',nhu:'Ổn định — mọi doanh nghiệp đều có bộ phận nhân sự-hành chính'},
  'van-hoa':  {jobs:['Chuyên viên văn hóa-xã hội tại cơ quan Nhà nước','Nghiên cứu viên khoa học xã hội, nhân học','Biên tập viên, quản lý di sản-bảo tàng-thư viện','Chuyên viên truyền thông chính sách, đối ngoại'],luong:'8–20 tr/tháng',nhu:'Ổn định — biên chế Nhà nước và tổ chức văn hóa-xã hội luôn cần nhân lực'},
  'the-thao': {jobs:['Giáo viên Giáo dục thể chất tại trường học','Huấn luyện viên thể thao, fitness, gym','Chuyên viên y học thể thao, phục hồi chấn thương','Quản lý câu lạc bộ, trung tâm thể thao-giải trí'],luong:'8–25 tr/tháng (HLV chuyên nghiệp có thể cao hơn)',nhu:'Tăng — phong trào thể thao-gym-fitness phát triển mạnh ở đô thị'},
  'thoi-trang':{jobs:['Nhà thiết kế thời trang, stylist','Kỹ thuật viên may, mẫu rập, kiểm soát chất lượng','Chuyên viên merchandising, mua hàng thời trang','Quản lý sản xuất tại nhà máy may xuất khẩu'],luong:'8–25 tr/tháng',nhu:'Ổn định — Việt Nam là trung tâm sản xuất dệt may lớn của thế giới'},
  'in-giay':  {jobs:['Kỹ sư công nghệ in, vận hành máy in công nghiệp','Chuyên viên thiết kế-sản xuất bao bì','Quản lý chất lượng tại nhà máy in-bao bì','Chuyên viên kinh doanh vật liệu in-bao bì'],luong:'8–22 tr/tháng',nhu:'Ổn định — nhu cầu bao bì tăng theo thương mại điện tử và xuất khẩu'},
  'tai-nguyen':{jobs:['Chuyên viên đo đạc-bản đồ, quản lý đất đai','Chuyên viên đánh giá tác động môi trường (ĐTM)','Kỹ sư xử lý nước thải, chất thải, ô nhiễm','Chuyên viên tại Sở/Phòng Tài nguyên-Môi trường'],luong:'8–22 tr/tháng',nhu:'Tăng — yêu cầu pháp lý về môi trường ngày càng chặt, doanh nghiệp cần tuân thủ'},
  'cham-soc': {jobs:['Chuyên viên chăm sóc da, trị liệu spa','Chuyên gia trang điểm, làm nail, tạo mẫu tóc','Tư vấn dinh dưỡng-làm đẹp, bán mỹ phẩm','Quản lý spa, salon, trung tâm thẩm mỹ'],luong:'8–20 tr/tháng (có thể cao hơn nếu tự kinh doanh)',nhu:'Tăng mạnh — nhu cầu làm đẹp-chăm sóc bản thân ngày càng phổ biến'},
  'cong-tac-xa-hoi':{jobs:['Nhân viên công tác xã hội tại bệnh viện, trường học','Chuyên viên tại trung tâm bảo trợ xã hội, mái ấm','Cán bộ chính sách xã hội tại UBND, đoàn thể','Chuyên viên dự án NGO, tổ chức phi chính phủ'],luong:'7–18 tr/tháng',nhu:'Tăng — chính sách an sinh xã hội ngày càng được đầu tư'},
  'bac-si-thu-y':{jobs:['Bác sĩ thú y tại trạm thú y, phòng khám thú cảnh','Chuyên viên kiểm dịch động vật, an toàn thực phẩm','Kỹ sư chăn nuôi, quản lý trang trại, thú y nông trại','Chuyên viên kinh doanh thuốc-vật tư thú y'],luong:'10–25 tr/tháng',nhu:'Tăng — nhu cầu thú cảnh tại đô thị và chăn nuôi quy mô lớn đều tăng'},
};
const ALL_207_SCHOOLS=[
{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; ĐGNL/ĐGTD+CCQT; Thi TN THPT 2026. Không xét học bạ.'},
{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',r:'Bắc',l:'Công lập',p:'Xét tuyển tài năng; ĐGTD (TSA); CCQT (SAT/ACT/A-Level); Thi TN THPT. Không xét học bạ.'},
{t:'Đại Học Ngoại Thương',m:'NTH',r:'Bắc',l:'Công lập',p:'7 PT: ĐGNL/ĐGTD; Kết hợp CCQT+Học bạ/Thi THPT; Thi TN THPT.'},
{t:'Đại Học Thương Mại',m:'TMU',r:'Bắc',l:'Công lập',p:'Thi TN THPT; Học bạ; ĐGNL. Mở 6 ngành mới + 4 tổ hợp mới.'},
{t:'Đại Học Công Nghiệp Hà Nội',m:'DCN',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; HSG/CCQT+Học bạ; Thi TN THPT; ĐGNL(ĐHQGHN)/ĐGTD(BKHN).'},
{t:'Học Viện Công Nghệ Bưu Chính Viễn Thông',m:'BVH',r:'Bắc',l:'Công lập',p:'Tài năng; CCQT(SAT/ACT); ĐGNL/ĐGTD(HSA,V-ACT,TSA,SPT); CCAnh+Học bạ; Thi THPT. Không học bạ độc lập.'},
{t:'Đại Học Công Nghệ-ĐHQG Hà Nội',m:'QHI',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT; ĐGNL(HSA); CCQT(SAT). Không học bạ.'},
{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; ĐGNL(HSA); Thi TN THPT.'},
{t:'Học Viện Ngân Hàng',m:'NHH',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Học bạ+ĐGNL/CCQT; Thi TN THPT 2026.'},
{t:'Học Viện Báo Chí và Tuyên Truyền',m:'HBT',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT; CCQT(IELTS,SAT)+Học bạ.'},
{t:'Đại Học Kinh Tế-ĐHQG Hà Nội',m:'QHE',r:'Bắc',l:'Công lập',p:'Thi TN THPT+CC ngoại ngữ; ĐGNL(ĐHQGHN); Tuyển thẳng.'},
{t:'Đại Học Việt Nhật-ĐHQG Hà Nội',m:'VJU',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi THPT; ĐGNL(ĐHQGHN); SAT; CCNN+Thi THPT; Phỏng vấn+ĐGNL.'},
{t:'Đại Học Sư Phạm Hà Nội',m:'SPH',r:'Bắc',l:'Công lập',p:'Thi TN THPT; Năng lực/thành tích vượt trội; ĐGNL(SPT).'},
{t:'Đại Học Luật-ĐHQGHN',m:'QHL',r:'Bắc',l:'Công lập',p:'Thi TN THPT+CCQT; Tuyển thẳng/Ưu tiên; ĐGNL(ĐHQGHN); Dự bị ĐH.'},
{t:'Đại Học KHTN-ĐHQGHN',m:'QHT',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT; ĐGNL(HSA); SAT; Kết hợp; Hiệp định/dự bị.'},
{t:'Đại Học Giao Thông Vận Tải',m:'GHA',r:'Bắc',l:'Công lập',p:'Thi THPT+tuyển thẳng; Học bạ+Thi THPT; ĐGNL(ĐHQGHN/HCM); ĐGTD(BKHN).'},
{t:'Học Viện Tài Chính',m:'HTC',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Kết hợp; Thi TN THPT 2026.'},
{t:'Đại Học Y Hà Nội',m:'YHB',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026.'},
{t:'Đại Học Y Dược-ĐHQGHN',m:'QHY',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Thi THPT+CCNN; ĐGNL(HSA); Dự bị dân tộc.'},
{t:'Đại Học Mở Hà Nội',m:'MHN',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng; ĐGNL/ĐGTD; Kết hợp; Dự bị.'},
{t:'Đại Học Sư Phạm Hà Nội 2',m:'SP2',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Thi THPT; Học bạ(đặc thù); Năng khiếu/ĐGNL.'},
{t:'Đại học Huế (các trường thành viên)',m:'DHD',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Thi THPT; Học bạ; ĐGNL; Kết hợp.'},
{t:'Đại học Hàng Hải Việt Nam',m:'HHA',r:'Bắc',l:'Công lập',p:'Thi THPT; Kết hợp; Học bạ; ĐGNL/ĐGTD; CCAnh+Học bạ; Tuyển thẳng.'},
{t:'Trường Khoa Học Liên Ngành và Nghệ Thuật-ĐHQGHN',m:'QHQ',r:'Bắc',l:'Công lập',p:'ĐGNL(HSA); Thi THPT; Kết hợp Thi+Năng khiếu/CCQT; Tuyển thẳng.'},
{t:'Học Viện Chính Sách và Phát Triển',m:'HCP',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Kết hợp(HSG/CCQT/Học bạ+Thi); ĐGNL(HSA/SPT)/ĐGTD(TSA); Thi TN THPT.'},
{t:'Đại Học Sư Phạm-ĐH Thái Nguyên',m:'DTS',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; ĐGNL(ĐHSPHN); Thi TN THPT; Năng khiếu/CCQT; Dự bị.'},
{t:'Đại học KH&CN Hà Nội',m:'KCN',r:'Bắc',l:'Công lập',p:'ĐGNL riêng; Năng lực+phỏng vấn; Tuyển thẳng; Thi TN THPT.'},
{t:'Đại Học Tài Nguyên Môi Trường HN',m:'DMT',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQGHN).'},
{t:'Đại Học Tân Trào',m:'TQU',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Thi THPT trước 2026; Học bạ.'},
{t:'Đại Học Kiểm Sát',m:'DKS',r:'Bắc',l:'Công lập',p:'11 tổ hợp, 4 ngành (đang cập nhật).'},
{t:'Đại học Công nghiệp Việt Trì',m:'VUI',r:'Bắc',l:'Công lập',p:'Học bạ; Thi TN THPT 2026; ĐGNL(ĐHQGHN)/ĐGTD(BKHN); Tuyển thẳng.'},
{t:'Đại học QL&CN Hải Phòng',m:'DHP',r:'Bắc',l:'Công lập',p:'Thi THPT(PT100); Học bạ 12(PT200); Tuyển thẳng.'},
{t:'Khoa Quốc tế-ĐH Thái Nguyên',m:'DTQ',r:'Bắc',l:'Công lập',p:'Thi THPT 2026; Học bạ; V-SAT(ĐHTN); ĐGNL/ĐGTD; Tuyển thẳng.'},
{t:'Đại học Hải Dương',m:'DKT',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi THPT; Học bạ; Kết hợp CC Tiếng Anh.'},
{t:'Đại học KT-KT Công nghiệp',m:'DKK',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGTD(BKHN); ĐGNL(ĐHQGHN).'},
{t:'Đại học SP TDTT Hà Nội',m:'TDH',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Thi+năng khiếu; Học bạ+năng khiếu; Thi năng khiếu.'},
{t:'Đại học Thái Bình',m:'DTB',r:'Bắc',l:'Công lập',p:'Thi TN THPT 2026; Học bạ 3 năm; ĐGNL(ĐHQGHN); ĐGTD(BKHN); ĐGNL(ĐHSPHN).'},
{t:'Đại học Hải Phòng',m:'THP',r:'Bắc',l:'Công lập',p:'Thi TN THPT 2026; Học bạ; CCQT; ĐGNL/ĐGTD; Tuyển thẳng.'},
{t:'Đại học Hà Nội',m:'NHF',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Kết hợp; Thi TN THPT 2026.'},
{t:'Đại học Khoa học-ĐH Thái Nguyên',m:'DTZ',r:'Bắc',l:'Công lập',p:'Thi THPT 2026; Học bạ; V-SAT(ĐHTN); ĐGNL/ĐGTD; Tuyển thẳng; Cử tuyển/dự bị; Kết hợp.'},
{t:'Đại học KT-QTKD-ĐH Thái Nguyên',m:'DTE',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQGHN/SPHN); V-SAT-TNU.'},
{t:'Đại học Công nghiệp Quảng Ninh',m:'DDM',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ(TB 3 năm); ĐGNL(ĐHQGHN)/ĐGTD(BKHN).'},
{t:'Đại học SP Kỹ thuật Nam Định',m:'SKN',r:'Bắc',l:'Công lập',p:'Thi TN THPT 2026; Học bạ(6 kỳ); ĐGNL(ĐHQGHN/SPHN)/ĐGTD(BKHN); Tuyển thẳng.'},
{t:'Đại học TDTT Bắc Ninh',m:'TDB',r:'Bắc',l:'Công lập',p:'Học bạ+năng khiếu; Thi THPT+năng khiếu; Tuyển thẳng.'},
{t:'Đại học SP Kỹ thuật Hưng Yên',m:'SKH',r:'Bắc',l:'Công lập',p:'Thi TN THPT 2026; ĐTB lớp 10,11,12; Tuyển thẳng; V-SAT/ĐGNL/ĐGTD.'},
{t:'Đại học Y dược-ĐH Thái Nguyên',m:'DTY',r:'Bắc',l:'Công lập',p:'Thi TN THPT; Tuyển thẳng; Học bạ; ĐGNL(HSA)/V-SAT; PT khác(500).'},
{t:'Đại học Nông Lâm Thái Nguyên',m:'DTN',r:'Bắc',l:'Công lập',p:'Thi TN THPT 2026; Học bạ 12; V-SAT(ĐHTN); Tuyển thẳng.'},
{t:'Đại học Sao Đỏ',m:'SDU',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD; Kết hợp.'},
{t:'Đại học CN Giao thông vận tải',m:'GTA',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Đại học Văn hoá Hà Nội',m:'VHH',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; Kết hợp năng khiếu.'},
{t:'Đại học Y dược Thái Bình',m:'YTB',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Dự bị ĐH; Thi TN THPT; ĐGNL(ĐHSPHN).'},
{t:'Đại học Điện Lực',m:'DDL',r:'Bắc',l:'Công lập',p:'Học bạ; Học bạ+CCQT; Thi TN THPT; Tuyển thẳng.'},
{t:'Đại học CNTT&TT-ĐH Thái Nguyên',m:'DTC',r:'Bắc',l:'Công lập',p:'Học bạ; Thi TN THPT; ĐGNL V-SAT-TNU; Tuyển thẳng.'},
{t:'Đại Học Luật Hà Nội',m:'HLU',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ(1 số ngành); ĐGNL/ĐGTD.'},
{t:'Đại Học Ngoại Ngữ-ĐHQGHN',m:'QHF',r:'Bắc',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; ĐGNL(HSA); Thi TN THPT 2026+CCNN.'},
{t:'Đại Học Dược Hà Nội',m:'DHN',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Học bạ+CCQT; Thi TN THPT 2026.'},
{t:'Đại Học Y Tế Công Cộng',m:'YTC',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Học bạ; Thi TN THPT 2026; ĐGNL.'},
{t:'Học Viện Hành Chính Quốc Gia',m:'HAQ',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Đại Học Xây Dựng Hà Nội',m:'XDH',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Đại Học Thuỷ Lợi',m:'TLU',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQGHN/HCM).'},
{t:'Đại Học Lâm Nghiệp Việt Nam',m:'LNV',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Học Viện Nông Nghiệp Việt Nam',m:'HVN',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; V-SAT/ĐGNL.'},
{t:'Đại Học Mỏ Địa Chất',m:'MDC',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Đại Học Kiến Trúc Hà Nội',m:'KTH',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi THPT 2026+năng khiếu; Học bạ+năng khiếu.'},
{t:'Đại Học Lao Động Xã Hội',m:'LDX',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Học Viện Phụ Nữ Việt Nam',m:'PNV',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL.'},
{t:'Đại Học Mỹ Thuật Việt Nam',m:'MTV',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi năng khiếu mỹ thuật; Kết hợp.'},
{t:'Đại Học Sân Khấu Điện Ảnh Hà Nội',m:'SKD',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi năng khiếu; Thi THPT+năng khiếu.'},
{t:'Học Viện Âm Nhạc Quốc Gia VN',m:'ANQ',r:'Bắc',l:'Công lập',p:'Tuyển thẳng(thi năng khiếu âm nhạc).'},
{t:'Học Viện Ngoại Giao',m:'HNG',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ+CCQT(IELTS/SAT); Tuyển thẳng.'},
{t:'Học Viện Quản Lý Giáo Dục',m:'QGD',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ THPT; Tuyển thẳng; ĐGNL/ĐGTD.'},
{t:'Học Viện Thanh Thiếu Niên VN',m:'TTN',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ 12; Tuyển thẳng.'},
{t:'Học Viện Tòa Án',m:'HTA',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ THPT; Tuyển thẳng.'},
{t:'Học Viện Y Dược Học Cổ Truyền VN',m:'YCT',r:'Bắc',l:'Công lập',p:'Thi THPT 2026; Tuyển thẳng theo quy định.'},
{t:'Học Viện Dân Tộc',m:'HDT',r:'Bắc',l:'Công lập',p:'Dự bị; Tuyển thẳng; ĐGNL; Học bạ; Thi THPT.'},
{t:'Học Viện Kỹ Thuật Mật Mã',m:'KMM',r:'Bắc',l:'Công lập',p:'Tuyển thẳng; Thi THPT 2026.'},
{t:'Học Viện Ngân Hàng-PV Bắc Ninh',m:'NHB',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ; V-SAT; ĐGNL(ĐHQGHN); Tuyển thẳng.'},
{t:'Đại Học Hạ Long',m:'DHL',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ THPT; Tuyển thẳng.'},
{t:'Đại Học Thủ Đô Hà Nội',m:'HNM',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Y Dược Hải Phòng',m:'YPB',r:'Bắc',l:'Công lập',p:'Thi THPT; ĐGNL ĐHQGHN; Tuyển thẳng.'},
{t:'Đại Học Giáo Dục-ĐHQGHN',m:'QHS',r:'Bắc',l:'Công lập',p:'Thi THPT; ĐGNL ĐHQGHN; Tuyển thẳng.'},
{t:'Trường Quốc Tế-ĐHQGHN',m:'QHQ2',r:'Bắc',l:'Công lập',p:'Thi THPT; CCQT; ĐGNL ĐHQGHN; Tuyển thẳng.'},
{t:'Đại Học Hùng Vương',m:'HVP',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Tây Bắc',m:'DTB2',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng; Dự bị ĐH.'},
{t:'Đại Học SP Nghệ Thuật TW',m:'SNA',r:'Bắc',l:'Công lập',p:'Thi THPT+năng khiếu; Tuyển thẳng.'},
{t:'Học Viện Âm Nhạc Quân Đội',m:'ANQ2',r:'Bắc',l:'Công lập',p:'Thi THPT+năng khiếu âm nhạc; Tuyển thẳng.'},
{t:'Đại Học Nội Vụ Hà Nội',m:'NVH',r:'Bắc',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL ĐHQGHN; Tuyển thẳng.'},
{t:'Đại Học Điều Dưỡng Nam Định',m:'DDN',r:'Bắc',l:'Công lập',p:'Thi THPT; Tuyển thẳng.'},
{t:'Học Viện Chính Trị Quốc Gia HCM',m:'CTQ',r:'Bắc',l:'Công lập',p:'Thi THPT; Tuyển thẳng; Theo chỉ tiêu.'},
{t:'Học Viện Quân Y',m:'YQH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng; ĐGNL ĐHQGHN&HCM; Thi THPT; ĐGNL Bộ QP.'},
{t:'Học Viện Kỹ Thuật Quân Sự',m:'KQH',r:'Bắc',l:'Quân sự/CA',p:'Tổ hợp A00,A01,AOT. Hệ dân sự PT riêng công bố sau.'},
{t:'Trường SQ Tăng Thiết Giáp',m:'TGH',r:'Bắc',l:'Quân sự/CA',p:'Tổ hợp A00,A01,C01.'},
{t:'Học Viện Biên Phòng',m:'BPH',r:'Bắc',l:'Quân sự/CA',p:'Dự kiến C03,C04,D01.'},
{t:'Trường SQ Chính Trị',m:'LCH',r:'Bắc',l:'Quân sự/CA',p:'C01,C03,C04,D01.'},
{t:'Đại học PCCC',m:'PCH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng; CCNN+Thi đánh giá BCA; Thi THPT+Thi đánh giá BCA.'},
{t:'Trường SQ Phòng hóa',m:'HGH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng/Ưu tiên; ĐGNL(ĐHQGHN/HCM); Thi TN THPT 2026; ĐGNL Bộ QP.'},
{t:'Học Viện An Ninh Nhân Dân',m:'ANH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng; CCNN+Thi BCA; Thi THPT+Thi BCA.'},
{t:'Học Viện Cảnh Sát Nhân Dân',m:'CSH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng; CCNN+Thi BCA; Thi THPT+Thi BCA.'},
{t:'Học Viện Phòng Không Không Quân',m:'PKH',r:'Bắc',l:'Quân sự/CA',p:'Tổ hợp môn Thi TN THPT; ĐGNL Bộ QP.'},
{t:'Học Viện Chính Trị CAND',m:'CTH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng theo QC BCA; CCNN+Thi BCA; Thi THPT.'},
{t:'Học Viện Hậu Cần-Hệ Dân Sự',m:'HCH',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng theo QC tuyển sinh(Điều 8).'},
{t:'Học Viện KH Quân Sự-Hệ Quân Sự',m:'KQS',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng/ưu tiên giải QG,QT; Thi THPT.'},
{t:'Học Viện KT Quân Sự-Hệ Dân Sự',m:'KDS',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng; ĐGNL ĐHQGHN&HCM; Thi THPT.'},
{t:'Học Viện Quân Y-Hệ Dân Sự',m:'YQD',r:'Bắc',l:'Quân sự/CA',p:'Tuyển thẳng; ĐGNL ĐHQGHN&HCM; Thi THPT.'},
{t:'Đại Học Thăng Long',m:'DTL',r:'Bắc',l:'Tư thục',p:'Thi TN THPT 2026; Kết hợp Thi+CCNN; ĐGNL/ĐGTD; Học bạ; Học bạ+năng khiếu; Tuyển thẳng.'},
{t:'Đại Học FPT',m:'FPT',r:'Bắc',l:'Tư thục',p:'Tuyển thẳng; Kết hợp(Thi THPT+Học bạ); Ưu tiên xét tuyển.'},
{t:'Đại Học Nguyễn Trãi',m:'NTU',r:'Bắc',l:'Tư thục',p:'Thi TN THPT 2026; Học bạ 12; Tuyển thẳng; Kết hợp năng khiếu.'},
{t:'Đại học Phương Đông',m:'DPD',r:'Bắc',l:'Tư thục',p:'Thi TN THPT 2026; Học bạ; Tuyển thẳng; ĐGNL(ĐHQGHN)/ĐGTD(BKHN); Kết hợp năng khiếu.'},
{t:'Đại học CN&QL Hữu Nghị',m:'DCQ',r:'Bắc',l:'Tư thục',p:'Thi THPT QG; Học bạ(6 kỳ); ĐGNL các trường.'},
{t:'Đại học Hòa Bình',m:'ETU',r:'Bắc',l:'Tư thục',p:'Thi TN THPT 2026; Học bạ/Văn bằng TC-CĐ; Tuyển thẳng; Học bạ+năng khiếu.'},
{t:'Đại Học Phenikaa',m:'PHE',r:'Bắc',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQGHN)/ĐGTD(BKHN)/V-SAT.'},
{t:'Đại Học VinUni',m:'VIN',r:'Bắc',l:'Tư thục',p:'Học bạ xuất sắc; CCQT(SAT/ACT/IB/AP); Phỏng vấn năng lực.'},
{t:'Đại học Hà Tĩnh',m:'HHT',r:'Trung',l:'Công lập',p:'Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD; Tốt nghiệp nước ngoài; Tuyển thẳng.'},
{t:'Đại học Hồng Đức',m:'HDT2',r:'Trung',l:'Công lập',p:'Thi TN THPT 2026; Học bạ(trừ SP); ĐGNL/ĐGTD; Tuyển thẳng/Cử tuyển/Dự bị.'},
{t:'Đại học VHTTDL Thanh Hóa',m:'DVD',r:'Trung',l:'Công lập',p:'Thi TN THPT 2026(+năng khiếu đặc thù); Học bạ(ngoài SP); Tuyển thẳng; ĐGNL/ĐGTD.'},
{t:'Đại học Tây Nguyên',m:'TTN2',r:'Trung',l:'Công lập',p:'Thi TN THPT; Học bạ; Tuyển thẳng; ĐGNL ĐHQG HCM; Kết hợp năng khiếu; Dự bị.'},
{t:'Đại học KT Y dược Đà Nẵng',m:'YDN',r:'Trung',l:'Công lập',p:'Thi THPT; Thi THPT+CCQT; Học bạ(trừ Y khoa); ĐGNL; Tuyển thẳng; Dự bị.'},
{t:'Đại Học Bách Khoa-ĐH Đà Nẵng',m:'DDT',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; V-SAT; ĐGNL/ĐGTD. Không học bạ độc lập.'},
{t:'Đại Học Kinh Tế-ĐH Đà Nẵng',m:'DDK',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; V-SAT; ĐGNL/ĐGTD.'},
{t:'Đại Học Sư Phạm-ĐH Đà Nẵng',m:'DDS',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Kết hợp năng khiếu(đặc thù).'},
{t:'Đại Học Vinh',m:'VIU',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD; Dự bị ĐH.'},
{t:'Đại Học Quy Nhơn',m:'QNU',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQG HCM); Dự bị ĐH.'},
{t:'Đại Học Nha Trang',m:'NTU2',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL; Kết hợp.'},
{t:'Đại Học Đà Lạt',m:'DLU',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQG HCM).'},
{t:'Đại Học Phú Yên',m:'PYU',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; Dự bị ĐH.'},
{t:'Đại Học Phạm Văn Đồng',m:'PVD',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; Dự bị ĐH.'},
{t:'Đại Học Quảng Nam',m:'QNM',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; Dự bị ĐH.'},
{t:'Học Viện Âm Nhạc Huế',m:'ANH2',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Năng khiếu âm nhạc+Thi THPT.'},
{t:'Đại Học Y Dược-ĐH Huế',m:'YDH',r:'Trung',l:'Công lập',p:'Thi THPT; Tuyển thẳng theo QC.'},
{t:'Đại Học Khoa Học-ĐH Huế',m:'KHH',r:'Trung',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL; Tuyển thẳng.'},
{t:'HV Ngân Hàng-PV Phú Yên',m:'NHY',r:'Trung',l:'Công lập',p:'Thi THPT; Học bạ; V-SAT; Tuyển thẳng.'},
{t:'PH ĐH Đà Nẵng tại Kon Tum',m:'DDK2',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi THPT; Học bạ; Dự bị ĐH.'},
{t:'PH ĐH Huế tại Quảng Trị',m:'DHQ',r:'Trung',l:'Công lập',p:'Tuyển thẳng; Thi THPT; Học bạ THPT.'},
{t:'Đại Học Bình Định',m:'BDI',r:'Trung',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Quảng Bình',m:'QBU',r:'Trung',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'HV KT Quân Sự-CS Phía Nam',m:'KPN',r:'Trung',l:'Quân sự/CA',p:'Tuyển thẳng; ĐGNL ĐHQG HCM; Thi THPT.'},
{t:'Đại Học Mỹ Thuật Huế',m:'MTH',r:'Trung',l:'Công lập',p:'Thi THPT+thi năng khiếu; Tuyển thẳng.'},
{t:'Đại Học Xây Dựng Miền Trung',m:'XMT',r:'Trung',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Học Viện Lục Quân',m:'LQH',r:'Trung',l:'Quân sự/CA',p:'Tổ hợp môn Thi TN THPT; ĐGNL Bộ QP.'},
{t:'Học Viện Hải Quân',m:'HQH',r:'Trung',l:'Quân sự/CA',p:'Tổ hợp môn Thi TN THPT; ĐGNL Bộ QP.'},
{t:'Đại Học Duy Tân',m:'DTU',r:'Trung',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ 12; ĐGNL(ĐHQG HCM); V-SAT.'},
{t:'Đại Học Đông Á',m:'DAD',r:'Trung',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL/ĐGTD.'},
{t:'Đại Học Yersin Đà Lạt',m:'YDL',r:'Trung',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ 12.'},
{t:'Đại Học Phan Thiết',m:'DPT',r:'Trung',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT.'},
{t:'Đại Học Fulbright VN',m:'FUV',r:'Trung',l:'Tư thục',p:'Hồ sơ toàn diện(học bạ,luận,thư GT,ngoại khóa); Phỏng vấn.'},
{t:'Đại Học Phan Châu Trinh',m:'PCT',r:'Trung',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'ĐH KHXH&NV-ĐHQG HCM',m:'QSX',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Tổng hợp(Thi+ĐGNL+Học bạ 3 năm+CCNN).'},
{t:'ĐH Sư Phạm TPHCM',m:'SPS',r:'Nam',l:'Công lập',p:'ĐGNL chuyên biệt(H-SCA)+Học bạ/năng khiếu; Tuyển thẳng.'},
{t:'ĐHQG TPHCM(Mô hình tích hợp)',m:'QSB',r:'Nam',l:'Công lập',p:'Tích hợp: ĐGNL(trụ cột)+Thi THPT+Học tập THPT.'},
{t:'Đại Học Bách Khoa TPHCM',m:'BKH',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+ĐGNL V-ACT); Tuyển thẳng/Ưu tiên. Không học bạ độc lập.'},
{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+V-ACT+Học bạ 3 năm+CCNN); Tuyển thẳng. Không học bạ độc lập.'},
{t:'Đại Học Kinh Tế TPHCM(UEH)',m:'UEH',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Tốt nghiệp nước ngoài/CCQT; Học tập tốt; ĐGNL+Anh; Thi THPT+Anh.'},
{t:'Đại Học Ngân Hàng TPHCM',m:'BUH',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Học bạ+CCQT; ĐGNL(ĐHQG HCM); Thi TN THPT 2026.'},
{t:'Đại Học SP Kỹ Thuật TPHCM',m:'SKS',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQG HCM); V-SAT.'},
{t:'Đại Học Tài Chính-Marketing',m:'DFM',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; ĐGNL(ĐHQG HCM); Học bạ 3 năm.'},
{t:'Đại Học Mở TPHCM',m:'OMH',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ; ĐGNL(ĐHQG HCM).'},
{t:'Đại Học Luật TPHCM',m:'HCL',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học tập THPT+ĐGNL; ĐGNL(ĐHQG HCM).'},
{t:'ĐH CNTT-ĐHQG TPHCM',m:'QSI',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+V-ACT+Học bạ 3 năm+CCNN); Tuyển thẳng.'},
{t:'ĐH KHTN-ĐHQG TPHCM',m:'QST2',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+V-ACT+Học bạ 3 năm+CCNN); Tuyển thẳng.'},
{t:'Đại Học Quốc Tế-ĐHQG TPHCM',m:'QSG',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; SAT/ACT; ĐGNL(V-ACT).'},
{t:'ĐH Kinh Tế-Luật ĐHQG TPHCM',m:'QSL',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+V-ACT+Học bạ 3 năm+CCNN); Tuyển thẳng.'},
{t:'ĐH Y Khoa Phạm Ngọc Thạch',m:'PNT',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026. Không học bạ độc lập.'},
{t:'Đại Học Cần Thơ',m:'CTU',r:'Nam',l:'Công lập',p:'Tuyển thẳng/Ưu tiên; Thi THPT 2026; Học bạ; V-SAT; CT tiên tiến/CLC.'},
{t:'Đại Học Y Dược Cần Thơ',m:'YCT2',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Dự bị ĐH; Thi TN THPT 2026; ĐGNL(ĐHQG HCM).'},
{t:'Đại Học An Giang-ĐHQG TPHCM',m:'AGU',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+V-ACT+Học bạ+CCNN); Tuyển thẳng.'},
{t:'ĐH KT-KT Bình Dương',m:'BDU2',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; ĐGNL(ĐHQG HCM).'},
{t:'Đại Học Thủ Dầu Một',m:'TDM',r:'Nam',l:'Công lập',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ 3 năm; ĐGNL(ĐHQG HCM).'},
{t:'Học Viện Cán Bộ TPHCM',m:'HVB',r:'Nam',l:'Công lập',p:'Thi TN THPT 2026; Học bạ 6 kỳ; Tuyển thẳng; ĐGNL(ĐHQGHN/HCM).'},
{t:'Đại Học Y Dược TPHCM',m:'YDS',r:'Nam',l:'Công lập',p:'Thi THPT 2026 duy nhất. Không bảo lưu, không học bạ, không CCQT.'},
{t:'Đại Học Tôn Đức Thắng',m:'DTT',r:'Nam',l:'Công lập',p:'Tổng hợp(Thi+Học bạ); Thi THPT; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'Đại Học Nông Lâm TPHCM',m:'NLS',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'Đại Học Kiến Trúc TPHCM',m:'KTS',r:'Nam',l:'Công lập',p:'Thi THPT+năng khiếu; Học bạ+năng khiếu; Tuyển thẳng.'},
{t:'Học Viện Hàng Không VN',m:'HKV',r:'Nam',l:'Công lập',p:'Tuyển thẳng/ưu tiên; Thi THPT; Học bạ; ĐGNL ĐHQG HCM&HN.'},
{t:'Đại Học Đồng Tháp',m:'DTH',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL; Tuyển thẳng.'},
{t:'ĐH Bà Rịa-Vũng Tàu',m:'BVU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'ĐH Tài Nguyên Môi Trường TPHCM',m:'TMT',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'Đại Học Sài Gòn',m:'SGU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'Nhạc Viện TPHCM',m:'NVS',r:'Nam',l:'Công lập',p:'Thi THPT+thi tuyển năng khiếu âm nhạc.'},
{t:'Đại Học Trà Vinh',m:'TVU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'Đại Học Đồng Nai',m:'DNU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng; ĐGNL ĐHQG HCM.'},
{t:'Đại Học Long An',m:'LAU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Tiền Giang',m:'TGU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Kiên Giang',m:'KGU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'ĐH SP Kỹ Thuật Vĩnh Long',m:'SVL',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Bạc Liêu',m:'BLU',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Học Viện Mekong',m:'MKG',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'ĐH Công Nghệ Miền Đông',m:'CMD',r:'Nam',l:'Công lập',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'HV Chính Trị Khu Vực II',m:'CK2',r:'Nam',l:'Công lập',p:'Thi THPT; Tuyển thẳng; Theo chỉ tiêu.'},
{t:'ĐH Công Nghệ Đồng Nai',m:'DNH',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; Kết hợp ĐGNL.'},
{t:'Đại Học Lạc Hồng',m:'LHU',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT.'},
{t:'Đại Học Hoa Sen',m:'HSU',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; ĐGNL(ĐHQG HCM).'},
{t:'Đại Học Văn Lang',m:'VLU',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; ĐGNL(ĐHQG HCM).'},
{t:'ĐH Nguyễn Tất Thành',m:'NTT',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; ĐGNL.'},
{t:'ĐH Công Nghệ TPHCM(HUTECH)',m:'HTC2',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT; ĐGNL(ĐHQG HCM).'},
{t:'Đại Học Gia Định',m:'GDU',r:'Nam',l:'Tư thục',p:'Tuyển thẳng; Thi TN THPT 2026; Học bạ THPT.'},
{t:'Đại Học RMIT VN',m:'RMT',r:'Nam',l:'Tư thục',p:'Tiêu chí riêng RMIT; Học bạ quốc tế; CCQT.'},
{t:'Đại Học Việt Đức',m:'VGU',r:'Nam',l:'Tư thục',p:'Thi THPT; Phỏng vấn; CCQT.'},
{t:'ĐH Quốc Tế Miền Đông',m:'EIU',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'ĐH Kinh Tế-Tài Chính TPHCM(UEF)',m:'UEF',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; ĐGNL ĐHQG HCM; Tuyển thẳng.'},
{t:'Đại Học Tây Đô',m:'TDU',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'ĐH KT-CN Cần Thơ',m:'KCT',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Văn Hiến',m:'VHU',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Cửu Long',m:'MCU',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Nam Cần Thơ',m:'NCT',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Bình Dương',m:'BDU3',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Võ Trường Toản',m:'VTT',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'},
{t:'Đại Học Tân Tạo',m:'TTU',r:'Nam',l:'Tư thục',p:'Thi THPT; Học bạ; Tuyển thẳng.'}
];

let schoolSearchQuery='';
let schoolFilterMien='Tất cả';

function renderSchoolList(){
  const wrap=document.getElementById('school207-list');
  if(!wrap)return;
  const q=schoolSearchQuery.toLowerCase().trim();
  let list=ALL_207_SCHOOLS;
  if(schoolFilterMien!=='Tất cả') list=list.filter(s=>s.r===schoolFilterMien);
  if(q) list=list.filter(s=>s.t.toLowerCase().includes(q)||s.m.toLowerCase().includes(q));
  const shown=list.slice(0,30);
  wrap.innerHTML=shown.map(s=>{
    const isDN=s.t.includes('Đồng Nai')||s.t==='Đại Học Lạc Hồng';
    return`<div class="sch207-row${isDN?' sch207-dn':''}">
      <div class="sch207-main">
        <span class="sch207-name">${isDN?'📍 ':''}${s.t}</span>
        <span class="sch207-meta"><span class="sch207-ma">${s.m}</span><span class="sch207-mien">${s.r}</span><span class="sch207-loai">${s.l}</span></span>
      </div>
      <div class="sch207-pt">${s.p}</div>
    </div>`;
  }).join('');
  document.getElementById('sch207-count').textContent=`${list.length} / 207 trường`+(list.length>30?' (hiện 30 đầu)':'');
}

function schoolSearchInput(v){schoolSearchQuery=v;renderSchoolList();}
function schoolFilterClick(mien,el){schoolFilterMien=mien;document.querySelectorAll('.sch207-filter').forEach(b=>b.classList.remove('active'));el.classList.add('active');renderSchoolList();}

const NGANH_TRUONG_MIEN={
  'yd':{B:[{t:'Đại Học Y Hà Nội',m:'YHB',th:'B00',diem:27.06,hp:15,ct:200},{t:'Đại Học Y Dược-ĐHQGHN',m:'QHY',th:'B00',diem:25.6,hp:18,ct:100},{t:'Đại Học Dược Hà Nội',m:'DHN',th:'B00',diem:23.05,hp:18,ct:60},{t:'Đại Học Y Tế Công Cộng',m:'YTC',th:'B00',diem:22.25,hp:10,ct:60},{t:'Học Viện Y Dược Học Cổ Truyền VN',m:'YCT',th:'B00',diem:19.52,hp:12,ct:150},{t:'Đại Học Y Dược Hải Phòng',m:'YPB',th:'B00',diem:22.31,hp:18,ct:80},{t:'Đại học Y dược Thái Bình',m:'YTB',th:'B00',diem:22.94,hp:18,ct:120},{t:'Đại học Y dược-ĐH Thái Nguyên',m:'DTY',th:'B00',diem:20.21,hp:18,ct:100},{t:'Học Viện Quân Y',m:'YQH',th:'B00',diem:27.74,hp:0,ct:80},{t:'Học Viện Quân Y-Hệ Dân Sự',m:'YQD',th:'B00',diem:25.79,hp:0,ct:80},{t:'Đại Học Điều Dưỡng Nam Định',m:'DDN',th:'B00',diem:22.84,hp:14,ct:100},{t:'Học Viện Nông Nghiệp Việt Nam',m:'HVN',th:'B00',diem:19.86,hp:14,ct:60}],T:[{t:'Đại Học Y Dược-ĐH Huế',m:'YDH',th:'B00',diem:19.51,hp:10,ct:100},{t:'Đại Học Khoa Học-ĐH Huế',m:'KHH',th:'B00',diem:23.66,hp:18,ct:100}],N:[{t:'ĐH Y Khoa Phạm Ngọc Thạch',m:'PNT',th:'B00',diem:27.73,hp:25,ct:180},{t:'Đại Học Y Dược TPHCM',m:'YDS',th:'B00',diem:25.0,hp:25,ct:80},{t:'Đại Học Y Dược Cần Thơ',m:'YCT2',th:'B00',diem:22.04,hp:18,ct:100},{t:'Đại Học Nông Lâm TPHCM',m:'NLS',th:'B00',diem:22.18,hp:10,ct:60}]},
  'cntt':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:27.15,hp:22,ct:80},{t:'Đại Học Công Nghệ-ĐHQG Hà Nội',m:'QHI',th:'A00',diem:27.92,hp:15,ct:150},{t:'Học Viện Công Nghệ Bưu Chính Viễn Thông',m:'BVH',th:'A00',diem:20.53,hp:14,ct:80},{t:'Đại học KH&CN Hà Nội',m:'KCN',th:'A00',diem:21.04,hp:12,ct:100},{t:'Đại Học Giao Thông Vận Tải',m:'GHA',th:'A00',diem:22.86,hp:10,ct:150},{t:'Đại Học Mở Hà Nội',m:'MHN',th:'A00',diem:22.49,hp:18,ct:80},{t:'Đại Học Phenikaa',m:'PHE',th:'A00',diem:15.82,hp:38,ct:200},{t:'Đại Học FPT',m:'FPT',th:'A00',diem:19.95,hp:45,ct:300},{t:'Đại học SP Kỹ thuật Nam Định',m:'SKN',th:'A00',diem:20.21,hp:14,ct:60},{t:'Đại học Sao Đỏ',m:'SDU',th:'A00',diem:20.26,hp:10,ct:100},{t:'Đại Học Việt Nhật-ĐHQG Hà Nội',m:'VJU',th:'A00',diem:21.21,hp:10,ct:80},{t:'Đại Học VinUni',m:'VIN',th:'A00',diem:19.57,hp:42,ct:200}],T:[{t:'Đại Học Bách Khoa-ĐH Đà Nẵng',m:'DDT',th:'A00',diem:20.17,hp:16,ct:120}],N:[{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:28.04,hp:25,ct:100},{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',th:'A00',diem:20.46,hp:12,ct:150},{t:'ĐH CNTT-ĐHQG TPHCM',m:'QSI',th:'A00',diem:26.66,hp:28,ct:150},{t:'ĐH KHTN-ĐHQG TPHCM',m:'QST2',th:'A00',diem:28.09,hp:25,ct:120},{t:'Đại Học SP Kỹ Thuật TPHCM',m:'SKS',th:'A00',diem:20.21,hp:12,ct:150},{t:'Đại Học RMIT VN',m:'RMT',th:'A00',diem:17.47,hp:28,ct:100}]},
  'kt-tc':{B:[{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',th:'D01',diem:25.11,hp:18,ct:200},{t:'Học Viện Ngân Hàng',m:'NHH',th:'D01',diem:26.19,hp:15,ct:150},{t:'Học Viện Tài Chính',m:'HTC',th:'D01',diem:21.1,hp:16,ct:150},{t:'Đại Học Thương Mại',m:'TMU',th:'D01',diem:25.51,hp:28,ct:80},{t:'Học Viện Ngân Hàng-PV Bắc Ninh',m:'NHB',th:'D01',diem:22.74,hp:10,ct:150},{t:'Học Viện Chính Sách và Phát Triển',m:'HCP',th:'D01',diem:23.13,hp:14,ct:60},{t:'Đại Học Thuỷ Lợi',m:'TLU',th:'D01',diem:25.67,hp:18,ct:150}],T:[{t:'HV Ngân Hàng-PV Phú Yên',m:'NHY',th:'D01',diem:19.02,hp:14,ct:150},{t:'Đại Học Kinh Tế-ĐH Đà Nẵng',m:'DDK',th:'D01',diem:23.19,hp:18,ct:60}],N:[{t:'Đại Học Kinh Tế TPHCM(UEH)',m:'UEH',th:'D01',diem:27.98,hp:22,ct:200},{t:'Đại Học Ngân Hàng TPHCM',m:'BUH',th:'D01',diem:21.79,hp:12,ct:80},{t:'Đại Học Tài Chính-Marketing',m:'DFM',th:'D01',diem:21.06,hp:12,ct:150},{t:'ĐH Kinh Tế-Luật ĐHQG TPHCM',m:'QSL',th:'D01',diem:28.31,hp:28,ct:80},{t:'ĐH KT-KT Bình Dương',m:'BDU2',th:'D01',diem:22.29,hp:16,ct:60}]},
  'kt-qtkd':{B:[{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',th:'D01',diem:24.95,hp:22,ct:120},{t:'Đại Học Ngoại Thương',m:'NTH',th:'D01',diem:25.46,hp:18,ct:180},{t:'Đại Học Thương Mại',m:'TMU',th:'D01',diem:28.29,hp:15,ct:200},{t:'Đại Học Kinh Tế-ĐHQG Hà Nội',m:'QHE',th:'D01',diem:21.67,hp:10,ct:150},{t:'Đại Học Thăng Long',m:'DTL',th:'D01',diem:18.83,hp:32,ct:250},{t:'Đại Học Phenikaa',m:'PHE',th:'D01',diem:19.73,hp:32,ct:200}],T:[],N:[{t:'Đại Học Kinh Tế TPHCM(UEH)',m:'UEH',th:'D01',diem:26.61,hp:28,ct:150},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:19.82,hp:42,ct:150},{t:'Đại Học Hoa Sen',m:'HSU',th:'D01',diem:18.56,hp:38,ct:200},{t:'ĐH Nguyễn Tất Thành',m:'NTT',th:'D01',diem:17.19,hp:28,ct:250},{t:'ĐH Công Nghệ TPHCM(HUTECH)',m:'HTC2',th:'D01',diem:15.61,hp:32,ct:100},{t:'Đại Học Ngân Hàng TPHCM',m:'BUH',th:'D01',diem:20.86,hp:18,ct:150},{t:'Đại Học Tài Chính-Marketing',m:'DFM',th:'D01',diem:20.27,hp:12,ct:60},{t:'Đại Học Thủ Dầu Một',m:'TDM',th:'D01',diem:19.39,hp:10,ct:80}]},
  'spg':{B:[{t:'Đại Học Sư Phạm Hà Nội',m:'SPH',th:'C00',diem:19.37,hp:10,ct:100},{t:'Đại Học Sư Phạm Hà Nội 2',m:'SP2',th:'C00',diem:19.39,hp:12,ct:100},{t:'Đại Học Sư Phạm-ĐH Thái Nguyên',m:'DTS',th:'C00',diem:22.68,hp:12,ct:150},{t:'Đại học Văn hoá Hà Nội',m:'VHH',th:'C00',diem:19.73,hp:18,ct:150},{t:'Đại Học SP Nghệ Thuật TW',m:'SNA',th:'C00',diem:21.6,hp:16,ct:120},{t:'Đại học SP TDTT Hà Nội',m:'TDH',th:'C00',diem:20.05,hp:10,ct:120},{t:'Đại học TDTT Bắc Ninh',m:'TDB',th:'C00',diem:20.95,hp:16,ct:120},{t:'Đại học SP Kỹ thuật Hưng Yên',m:'SKH',th:'C00',diem:23.75,hp:10,ct:60},{t:'Đại học KT-QTKD-ĐH Thái Nguyên',m:'DTE',th:'C00',diem:19.33,hp:14,ct:60}],T:[{t:'Đại Học Sư Phạm-ĐH Đà Nẵng',m:'DDS',th:'C00',diem:20.37,hp:12,ct:150},{t:'Đại học Hồng Đức',m:'HDT2',th:'C00',diem:21.47,hp:16,ct:80}],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'C00',diem:20.53,hp:12,ct:60}]},
  'bao-chi':{B:[{t:'Học Viện Báo Chí và Tuyên Truyền',m:'HBT',th:'D01',diem:21.44,hp:18,ct:60},{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',th:'D01',diem:19.28,hp:18,ct:60},{t:'Đại học Văn hoá Hà Nội',m:'VHH',th:'D01',diem:24.33,hp:12,ct:80},{t:'Đại Học Sân Khấu Điện Ảnh Hà Nội',m:'SKD',th:'D01',diem:21.24,hp:16,ct:80}],T:[{t:'Đại Học Duy Tân',m:'DTU',th:'D01',diem:19.32,hp:28,ct:150}],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'D01',diem:21.08,hp:16,ct:100},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:19.63,hp:38,ct:200},{t:'ĐH Công Nghệ TPHCM(HUTECH)',m:'HTC2',th:'D01',diem:17.12,hp:45,ct:300},{t:'ĐH Nguyễn Tất Thành',m:'NTT',th:'D01',diem:18.31,hp:25,ct:150},{t:'ĐH Kinh Tế-Tài Chính TPHCM(UEF)',m:'UEF',th:'D01',diem:15.95,hp:32,ct:100},{t:'Đại Học Văn Hiến',m:'VHU',th:'D01',diem:17.9,hp:28,ct:100}]},
  'luat':{B:[{t:'Đại Học Luật Hà Nội',m:'HLU',th:'C00',diem:27.49,hp:15,ct:80},{t:'Đại Học Luật-ĐHQGHN',m:'QHL',th:'C00',diem:26.84,hp:28,ct:180},{t:'Đại Học Sư Phạm Hà Nội 2',m:'SP2',th:'C00',diem:19.87,hp:18,ct:60},{t:'Đại Học Kiểm Sát',m:'DKS',th:'C00',diem:23.68,hp:10,ct:150}],T:[{t:'Đại Học Phú Yên',m:'PYU',th:'C00',diem:19.37,hp:12,ct:120},{t:'Đại Học Vinh',m:'VIU',th:'C00',diem:19.66,hp:18,ct:80}],N:[{t:'Đại Học Luật TPHCM',m:'HCL',th:'C00',diem:26.82,hp:15,ct:180},{t:'ĐH Kinh Tế-Luật ĐHQG TPHCM',m:'QSL',th:'C00',diem:24.83,hp:28,ct:180},{t:'Đại Học Văn Lang',m:'VLU',th:'C00',diem:17.61,hp:35,ct:150},{t:'ĐH Kinh Tế-Tài Chính TPHCM(UEF)',m:'UEF',th:'C00',diem:18.35,hp:35,ct:150}]},
  'cokhi':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:25.56,hp:18,ct:200},{t:'Đại học SP Kỹ thuật Hưng Yên',m:'SKH',th:'A00',diem:22.55,hp:16,ct:100},{t:'Đại học SP Kỹ thuật Nam Định',m:'SKN',th:'A00',diem:24.11,hp:10,ct:60},{t:'Đại Học Công Nghiệp Hà Nội',m:'DCN',th:'A00',diem:21.52,hp:18,ct:60},{t:'Đại học Sao Đỏ',m:'SDU',th:'A00',diem:19.4,hp:12,ct:150},{t:'Đại học CN Giao thông vận tải',m:'GTA',th:'A00',diem:20.46,hp:14,ct:60},{t:'Đại Học Phenikaa',m:'PHE',th:'A00',diem:19.4,hp:35,ct:200}],T:[{t:'Đại Học Bách Khoa-ĐH Đà Nẵng',m:'DDT',th:'A00',diem:19.87,hp:18,ct:100}],N:[{t:'Đại Học SP Kỹ Thuật TPHCM',m:'SKS',th:'A00',diem:22.36,hp:18,ct:60},{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',th:'A00',diem:22.67,hp:18,ct:100},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:28.23,hp:15,ct:100},{t:'Đại Học Lạc Hồng',m:'LHU',th:'A00',diem:16.32,hp:18,ct:300},{t:'ĐH Công Nghệ Đồng Nai',m:'DNH',th:'A00',diem:15.78,hp:22,ct:300}]},
  'xd':{B:[{t:'Đại Học Xây Dựng Hà Nội',m:'XDH',th:'A00',diem:20.16,hp:14,ct:80},{t:'Đại Học Kiến Trúc Hà Nội',m:'KTH',th:'A00',diem:22.78,hp:14,ct:150},{t:'Đại Học Thuỷ Lợi',m:'TLU',th:'A00',diem:26.45,hp:15,ct:80},{t:'Đại Học Lâm Nghiệp Việt Nam',m:'LNV',th:'A00',diem:22.49,hp:14,ct:60},{t:'Đại Học Giao Thông Vận Tải',m:'GHA',th:'A00',diem:19.02,hp:12,ct:100},{t:'Đại Học Mỏ Địa Chất',m:'MDC',th:'A00',diem:19.89,hp:16,ct:150}],T:[{t:'Đại Học Bách Khoa-ĐH Đà Nẵng',m:'DDT',th:'A00',diem:22.88,hp:18,ct:60},{t:'Đại Học Xây Dựng Miền Trung',m:'XMT',th:'A00',diem:19.62,hp:12,ct:150}],N:[{t:'Đại Học Kiến Trúc TPHCM',m:'KTS',th:'A00',diem:19.2,hp:14,ct:150},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:26.71,hp:25,ct:100},{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',th:'A00',diem:19.23,hp:14,ct:60},{t:'Đại Học Lạc Hồng',m:'LHU',th:'A00',diem:19.49,hp:20,ct:150}]},
  'tkdh':{B:[{t:'Đại Học Mỹ Thuật Việt Nam',m:'MTV',th:'H00',diem:22.67,hp:14,ct:150},{t:'Đại Học Sân Khấu Điện Ảnh Hà Nội',m:'SKD',th:'H00',diem:23.86,hp:16,ct:150},{t:'Đại Học FPT',m:'FPT',th:'H00',diem:18.75,hp:32,ct:150},{t:'Đại Học Sư Phạm Hà Nội 2',m:'SP2',th:'H00',diem:24.37,hp:12,ct:120}],T:[{t:'Đại Học Mỹ Thuật Huế',m:'MTH',th:'H00',diem:19.14,hp:14,ct:120}],N:[{t:'Đại Học Văn Lang',m:'VLU',th:'H00',diem:19.01,hp:45,ct:150},{t:'Đại Học Hoa Sen',m:'HSU',th:'H00',diem:16.33,hp:45,ct:100},{t:'ĐH Nguyễn Tất Thành',m:'NTT',th:'H00',diem:16.91,hp:18,ct:250},{t:'ĐH Công Nghệ TPHCM(HUTECH)',m:'HTC2',th:'H00',diem:16.11,hp:38,ct:200},{t:'ĐH Kinh Tế-Tài Chính TPHCM(UEF)',m:'UEF',th:'H00',diem:16.53,hp:32,ct:150}]},
  'du-lich':{B:[{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',th:'D01',diem:19.13,hp:12,ct:120},{t:'Đại học Văn hoá Hà Nội',m:'VHH',th:'D01',diem:20.81,hp:10,ct:100}],T:[{t:'Đại Học Đà Lạt',m:'DLU',th:'D01',diem:20.93,hp:18,ct:120},{t:'Đại Học Nha Trang',m:'NTU2',th:'D01',diem:22.74,hp:18,ct:100}],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'D01',diem:24.17,hp:10,ct:100},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:15.89,hp:35,ct:100},{t:'Đại Học Hoa Sen',m:'HSU',th:'D01',diem:15.54,hp:38,ct:200},{t:'ĐH Kinh Tế-Tài Chính TPHCM(UEF)',m:'UEF',th:'D01',diem:18.64,hp:35,ct:250},{t:'Đại Học Trà Vinh',m:'TVU',th:'D01',diem:22.33,hp:18,ct:60},{t:'Đại Học Văn Hiến',m:'VHU',th:'D01',diem:16.93,hp:28,ct:150}]},
  'nlts':{B:[{t:'Học Viện Nông Nghiệp Việt Nam',m:'HVN',th:'B00',diem:20.4,hp:16,ct:60},{t:'Đại Học Lâm Nghiệp Việt Nam',m:'LNV',th:'B00',diem:21.86,hp:18,ct:80},{t:'Đại học Nông Lâm Thái Nguyên',m:'DTN',th:'B00',diem:21.0,hp:10,ct:100}],T:[{t:'Đại học Tây Nguyên',m:'TTN2',th:'B00',diem:22.43,hp:10,ct:100},{t:'Đại Học Nha Trang',m:'NTU2',th:'B00',diem:21.79,hp:16,ct:100}],N:[{t:'Đại Học Nông Lâm TPHCM',m:'NLS',th:'B00',diem:21.21,hp:14,ct:150},{t:'Đại Học Cần Thơ',m:'CTU',th:'B00',diem:19.7,hp:16,ct:120},{t:'Đại Học Trà Vinh',m:'TVU',th:'B00',diem:22.73,hp:12,ct:150},{t:'Đại Học An Giang-ĐHQG TPHCM',m:'AGU',th:'B00',diem:22.13,hp:16,ct:150}]},
  'tl':{B:[{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',th:'C00',diem:23.59,hp:14,ct:100},{t:'Đại Học Sư Phạm Hà Nội',m:'SPH',th:'C00',diem:20.16,hp:18,ct:150},{t:'Học Viện Phụ Nữ Việt Nam',m:'PNV',th:'C00',diem:22.6,hp:16,ct:120}],T:[{t:'Đại Học Đà Lạt',m:'DLU',th:'C00',diem:21.43,hp:12,ct:150}],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'C00',diem:21.6,hp:12,ct:60},{t:'Đại Học Văn Hiến',m:'VHU',th:'C00',diem:16.42,hp:28,ct:200}]},
  'ngoai-giao':{B:[{t:'Học Viện Ngoại Giao',m:'HNG',th:'D01',diem:24.87,hp:18,ct:200},{t:'Đại Học Ngoại Thương',m:'NTH',th:'D01',diem:25.74,hp:18,ct:100},{t:'Đại Học Ngoại Ngữ-ĐHQGHN',m:'QHF',th:'D01',diem:19.13,hp:12,ct:120},{t:'Đại học Hà Nội',m:'NHF',th:'D01',diem:22.36,hp:10,ct:120},{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',th:'D01',diem:21.28,hp:18,ct:80},{t:'Học Viện Báo Chí và Tuyên Truyền',m:'HBT',th:'D01',diem:22.95,hp:16,ct:120}],T:[],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'D01',diem:21.2,hp:12,ct:60},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:19.46,hp:28,ct:250}]},
  'nt':{B:[{t:'Đại Học Mỹ Thuật Việt Nam',m:'MTV',th:'N00',diem:20.2,hp:18,ct:120},{t:'Học Viện Âm Nhạc Quốc Gia VN',m:'ANQ',th:'N00',diem:19.28,hp:12,ct:60},{t:'Đại Học Sân Khấu Điện Ảnh Hà Nội',m:'SKD',th:'N00',diem:21.51,hp:16,ct:150},{t:'Học Viện Âm Nhạc Quân Đội',m:'ANQ2',th:'N00',diem:24.43,hp:18,ct:100},{t:'Đại Học Sư Phạm Hà Nội 2',m:'SP2',th:'N00',diem:24.23,hp:16,ct:150},{t:'Đại Học SP Nghệ Thuật TW',m:'SNA',th:'N00',diem:23.48,hp:18,ct:120}],T:[{t:'Đại Học Mỹ Thuật Huế',m:'MTH',th:'N00',diem:23.57,hp:18,ct:120},{t:'Học Viện Âm Nhạc Huế',m:'ANH2',th:'N00',diem:23.93,hp:16,ct:120}],N:[{t:'Nhạc Viện TPHCM',m:'NVS',th:'N00',diem:20.43,hp:12,ct:100}]},
  'khtn':{B:[{t:'Đại Học KHTN-ĐHQGHN',m:'QHT',th:'A00',diem:27.56,hp:28,ct:150},{t:'Đại học KH&CN Hà Nội',m:'KCN',th:'A00',diem:22.45,hp:14,ct:120},{t:'Đại học Khoa học-ĐH Thái Nguyên',m:'DTZ',th:'A00',diem:19.43,hp:14,ct:80},{t:'Học Viện Nông Nghiệp Việt Nam',m:'HVN',th:'A00',diem:20.49,hp:14,ct:150}],T:[{t:'Đại Học Khoa Học-ĐH Huế',m:'KHH',th:'A00',diem:19.44,hp:12,ct:80}],N:[{t:'ĐH KHTN-ĐHQG TPHCM',m:'QST2',th:'A00',diem:26.03,hp:18,ct:200},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:25.36,hp:25,ct:150},{t:'Đại Học Nông Lâm TPHCM',m:'NLS',th:'A00',diem:20.82,hp:16,ct:120}]},
  'quan-doi':{B:[{t:'Học Viện An Ninh Nhân Dân',m:'ANH',th:'A00',diem:22.31,hp:0,ct:120},{t:'Học Viện Cảnh Sát Nhân Dân',m:'CSH',th:'A00',diem:23.95,hp:0,ct:150},{t:'Học Viện Kỹ Thuật Quân Sự',m:'KQH',th:'A00',diem:26.73,hp:0,ct:60},{t:'Trường SQ Tăng Thiết Giáp',m:'TGH',th:'A00',diem:26.28,hp:0,ct:150},{t:'Học Viện Biên Phòng',m:'BPH',th:'A00',diem:23.9,hp:0,ct:60},{t:'Trường SQ Chính Trị',m:'LCH',th:'A00',diem:26.71,hp:0,ct:100},{t:'Đại học PCCC',m:'PCH',th:'A00',diem:25.77,hp:0,ct:120},{t:'Trường SQ Phòng hóa',m:'HGH',th:'A00',diem:24.69,hp:0,ct:150},{t:'Học Viện Phòng Không Không Quân',m:'PKH',th:'A00',diem:26.0,hp:0,ct:80},{t:'Học Viện Quân Y',m:'YQH',th:'A00',diem:26.45,hp:0,ct:120},{t:'Học Viện KH Quân Sự-Hệ Quân Sự',m:'KQS',th:'A00',diem:24.18,hp:0,ct:60},{t:'Học Viện KT Quân Sự-Hệ Dân Sự',m:'KDS',th:'A00',diem:23.94,hp:0,ct:120}],T:[{t:'Học Viện Âm Nhạc Huế',m:'ANH2',th:'A00',diem:22.98,hp:16,ct:80}],N:[]},
  'ke-toan':{B:[{t:'Học Viện Tài Chính',m:'HTC',th:'D01',diem:24.39,hp:18,ct:60},{t:'Học Viện Ngân Hàng',m:'NHH',th:'D01',diem:28.13,hp:28,ct:180},{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',th:'D01',diem:27.15,hp:15,ct:200},{t:'Đại Học Thuỷ Lợi',m:'TLU',th:'D01',diem:26.21,hp:25,ct:100}],T:[{t:'Đại Học Kinh Tế-ĐH Đà Nẵng',m:'DDK',th:'D01',diem:19.28,hp:16,ct:100}],N:[{t:'Đại Học Kinh Tế TPHCM(UEH)',m:'UEH',th:'D01',diem:25.35,hp:22,ct:120},{t:'Đại Học Ngân Hàng TPHCM',m:'BUH',th:'D01',diem:23.19,hp:16,ct:100},{t:'Đại Học Tài Chính-Marketing',m:'DFM',th:'D01',diem:23.14,hp:16,ct:100},{t:'Đại Học Lạc Hồng',m:'LHU',th:'D01',diem:19.17,hp:25,ct:100},{t:'Đại Học Đồng Nai',m:'DNU',th:'D01',diem:23.12,hp:10,ct:100},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:16.12,hp:28,ct:100}]},
  'ban-dan':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:27.52,hp:18,ct:100},{t:'Đại Học Công Nghệ-ĐHQG Hà Nội',m:'QHI',th:'A00',diem:27.86,hp:28,ct:100},{t:'Đại học KH&CN Hà Nội',m:'KCN',th:'A00',diem:20.31,hp:16,ct:60},{t:'Đại Học Phenikaa',m:'PHE',th:'A00',diem:17.82,hp:32,ct:250},{t:'Đại Học FPT',m:'FPT',th:'A00',diem:18.5,hp:35,ct:150}],T:[],N:[{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:26.92,hp:15,ct:100},{t:'ĐH CNTT-ĐHQG TPHCM',m:'QSI',th:'A00',diem:28.36,hp:15,ct:180},{t:'Đại Học RMIT VN',m:'RMT',th:'A00',diem:15.13,hp:35,ct:300}]},
  'ngoai-thuong':{B:[{t:'Đại Học Ngoại Thương',m:'NTH',th:'D01',diem:27.21,hp:25,ct:150},{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',th:'D01',diem:28.27,hp:18,ct:80},{t:'Đại Học Việt Nhật-ĐHQG Hà Nội',m:'VJU',th:'D01',diem:22.26,hp:12,ct:60},{t:'Học Viện Ngoại Giao',m:'HNG',th:'D01',diem:27.29,hp:22,ct:200},{t:'Đại Học Thương Mại',m:'TMU',th:'D01',diem:26.9,hp:15,ct:180}],T:[],N:[{t:'Đại Học Kinh Tế TPHCM(UEH)',m:'UEH',th:'D01',diem:27.63,hp:22,ct:180}]},
  'dien-tu':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:26.21,hp:22,ct:80},{t:'Đại học SP Kỹ thuật Hưng Yên',m:'SKH',th:'A00',diem:21.78,hp:14,ct:60},{t:'Đại học CN Giao thông vận tải',m:'GTA',th:'A00',diem:23.67,hp:16,ct:60},{t:'Đại học Điện Lực',m:'DDL',th:'A00',diem:21.38,hp:14,ct:120},{t:'Đại Học Công Nghiệp Hà Nội',m:'DCN',th:'A00',diem:22.89,hp:16,ct:80}],T:[],N:[{t:'Đại Học SP Kỹ Thuật TPHCM',m:'SKS',th:'A00',diem:23.04,hp:14,ct:150},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:27.73,hp:28,ct:150},{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',th:'A00',diem:21.56,hp:18,ct:100},{t:'Đại Học Lạc Hồng',m:'LHU',th:'A00',diem:16.61,hp:20,ct:100},{t:'ĐH Công Nghệ Đồng Nai',m:'DNH',th:'A00',diem:16.39,hp:25,ct:150}]},
  'hang-khong':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:27.5,hp:28,ct:180},{t:'Đại Học Giao Thông Vận Tải',m:'GHA',th:'A00',diem:22.68,hp:14,ct:60},{t:'Đại Học Công Nghệ-ĐHQG Hà Nội',m:'QHI',th:'A00',diem:26.48,hp:22,ct:100},{t:'Đại Học Việt Nhật-ĐHQG Hà Nội',m:'VJU',th:'A00',diem:21.68,hp:14,ct:100}],T:[],N:[{t:'Học Viện Hàng Không VN',m:'HKV',th:'A00',diem:20.87,hp:18,ct:100},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:26.72,hp:28,ct:100}]},
  'vat-lieu':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:24.84,hp:25,ct:150},{t:'Đại Học KHTN-ĐHQGHN',m:'QHT',th:'A00',diem:26.72,hp:18,ct:200},{t:'Đại học KH&CN Hà Nội',m:'KCN',th:'A00',diem:21.62,hp:16,ct:120}],T:[],N:[{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:27.67,hp:15,ct:120},{t:'ĐH KHTN-ĐHQG TPHCM',m:'QST2',th:'A00',diem:25.39,hp:18,ct:120}]},
  'thuc-pham':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'B00',diem:27.16,hp:22,ct:150}],T:[],N:[{t:'Đại Học Nông Lâm TPHCM',m:'NLS',th:'B00',diem:22.04,hp:14,ct:120},{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',th:'B00',diem:24.48,hp:18,ct:100},{t:'Đại Học Cần Thơ',m:'CTU',th:'B00',diem:20.93,hp:16,ct:100},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'B00',diem:25.73,hp:18,ct:80},{t:'Đại Học Lạc Hồng',m:'LHU',th:'B00',diem:18.61,hp:22,ct:100}]},
  'hang-hai':{B:[{t:'Đại học Hàng Hải Việt Nam',m:'HHA',th:'A00',diem:23.09,hp:12,ct:80},{t:'Đại Học Thuỷ Lợi',m:'TLU',th:'A00',diem:25.37,hp:25,ct:120},{t:'Đại Học Tài Nguyên Môi Trường HN',m:'DMT',th:'A00',diem:22.99,hp:18,ct:150},{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:25.63,hp:15,ct:100}],T:[],N:[{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:25.68,hp:22,ct:100},{t:'ĐH Tài Nguyên Môi Trường TPHCM',m:'TMT',th:'A00',diem:20.66,hp:18,ct:80}]},
  'mo-dia':{B:[{t:'Đại Học Mỏ Địa Chất',m:'MDC',th:'A00',diem:20.51,hp:10,ct:150},{t:'Đại Học Tài Nguyên Môi Trường HN',m:'DMT',th:'A00',diem:20.61,hp:12,ct:120},{t:'Đại Học KHTN-ĐHQGHN',m:'QHT',th:'A00',diem:24.91,hp:15,ct:180}],T:[],N:[{t:'ĐH Tài Nguyên Môi Trường TPHCM',m:'TMT',th:'A00',diem:20.56,hp:16,ct:120}]},
  'toan-tk':{B:[{t:'Đại Học KHTN-ĐHQGHN',m:'QHT',th:'A00',diem:25.86,hp:15,ct:120},{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:28.26,hp:25,ct:80},{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',th:'A00',diem:27.79,hp:25,ct:150},{t:'Đại Học Sư Phạm Hà Nội',m:'SPH',th:'A00',diem:19.41,hp:10,ct:80}],T:[],N:[{t:'ĐH KHTN-ĐHQG TPHCM',m:'QST2',th:'A00',diem:25.1,hp:28,ct:120},{t:'Đại Học Bách Khoa TPHCM',m:'BKH',th:'A00',diem:24.84,hp:18,ct:80}]},
  'nhan-su':{B:[{t:'Đại Học Kinh Tế Quốc Dân',m:'KHA',th:'D01',diem:26.73,hp:25,ct:180},{t:'Đại Học Lao Động Xã Hội',m:'LDX',th:'D01',diem:22.28,hp:18,ct:80}],T:[],N:[{t:'Đại Học Kinh Tế TPHCM(UEH)',m:'UEH',th:'D01',diem:27.6,hp:25,ct:150},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:19.54,hp:35,ct:300},{t:'ĐH Công Nghệ TPHCM(HUTECH)',m:'HTC2',th:'D01',diem:19.95,hp:35,ct:300},{t:'Đại Học Thủ Dầu Một',m:'TDM',th:'D01',diem:22.42,hp:18,ct:60}]},
  'van-hoa':{B:[{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',th:'C00',diem:24.21,hp:12,ct:80},{t:'Học Viện Báo Chí và Tuyên Truyền',m:'HBT',th:'C00',diem:20.46,hp:10,ct:80},{t:'Đại học Văn hoá Hà Nội',m:'VHH',th:'C00',diem:20.32,hp:18,ct:60},{t:'Học Viện Chính Trị Quốc Gia HCM',m:'CTQ',th:'C00',diem:19.86,hp:16,ct:120},{t:'Học Viện Hành Chính Quốc Gia',m:'HAQ',th:'C00',diem:22.79,hp:16,ct:100}],T:[],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'C00',diem:19.18,hp:14,ct:100}]},
  'the-thao':{B:[{t:'Đại học SP TDTT Hà Nội',m:'TDH',th:'T00',diem:22.87,hp:16,ct:60},{t:'Đại học TDTT Bắc Ninh',m:'TDB',th:'T00',diem:22.78,hp:14,ct:150}],T:[],N:[{t:'ĐH Sư Phạm TPHCM',m:'SPS',th:'T00',diem:22.64,hp:12,ct:120}]},
  'thoi-trang':{B:[{t:'Đại Học Mỹ Thuật Việt Nam',m:'MTV',th:'H00',diem:19.63,hp:12,ct:80},{t:'Đại Học Kiến Trúc Hà Nội',m:'KTH',th:'H00',diem:24.0,hp:12,ct:60},{t:'Đại Học Sư Phạm Hà Nội 2',m:'SP2',th:'H00',diem:19.33,hp:14,ct:150}],T:[],N:[{t:'Đại Học Kiến Trúc TPHCM',m:'KTS',th:'H00',diem:23.12,hp:18,ct:100}]},
  'in-giay':{B:[{t:'Đại Học Bách Khoa Hà Nội',m:'BKA',th:'A00',diem:26.26,hp:25,ct:200},{t:'Đại Học Công Nghiệp Hà Nội',m:'DCN',th:'A00',diem:20.67,hp:16,ct:100}],T:[],N:[{t:'Đại Học SP Kỹ Thuật TPHCM',m:'SKS',th:'A00',diem:21.75,hp:16,ct:120},{t:'Đại Học Công Nghiệp TPHCM',m:'DIC',th:'A00',diem:19.44,hp:10,ct:120}]},
  'tai-nguyen':{B:[{t:'Đại Học Tài Nguyên Môi Trường HN',m:'DMT',th:'A00',diem:23.04,hp:18,ct:100},{t:'Đại Học KHTN-ĐHQGHN',m:'QHT',th:'A00',diem:24.6,hp:18,ct:200}],T:[{t:'Đại Học Khoa Học-ĐH Huế',m:'KHH',th:'A00',diem:23.6,hp:18,ct:150}],N:[{t:'ĐH Tài Nguyên Môi Trường TPHCM',m:'TMT',th:'A00',diem:24.23,hp:14,ct:150},{t:'Đại Học Nông Lâm TPHCM',m:'NLS',th:'A00',diem:19.22,hp:12,ct:120}]},
  'cham-soc':{B:[],T:[],N:[{t:'ĐH Công Nghệ TPHCM(HUTECH)',m:'HTC2',th:'D01',diem:17.59,hp:38,ct:200},{t:'Đại Học Văn Lang',m:'VLU',th:'D01',diem:15.91,hp:42,ct:250},{t:'ĐH Nguyễn Tất Thành',m:'NTT',th:'D01',diem:18.17,hp:25,ct:100}]},
  'cong-tac-xa-hoi':{B:[{t:'Đại Học KHXH&NV Hà Nội',m:'QHX',th:'D01',diem:21.59,hp:16,ct:100},{t:'Đại Học Lao Động Xã Hội',m:'LDX',th:'D01',diem:20.77,hp:10,ct:80}],T:[{t:'Đại Học Đà Lạt',m:'DLU',th:'D01',diem:20.81,hp:16,ct:100}],N:[{t:'Đại Học Văn Hiến',m:'VHU',th:'D01',diem:18.31,hp:25,ct:300}]},
  'bac-si-thu-y':{B:[{t:'Học Viện Nông Nghiệp Việt Nam',m:'HVN',th:'B00',diem:19.2,hp:10,ct:100}],T:[{t:'Đại Học Nha Trang',m:'NTU2',th:'B00',diem:20.39,hp:10,ct:120}],N:[{t:'Đại Học Nông Lâm TPHCM',m:'NLS',th:'B00',diem:23.76,hp:10,ct:150},{t:'Đại Học Cần Thơ',m:'CTU',th:'B00',diem:21.54,hp:10,ct:80},{t:'Đại Học An Giang-ĐHQG TPHCM',m:'AGU',th:'B00',diem:21.85,hp:18,ct:120}]},
};

let dhActiveTab='tohop';
function switchDHTab(tab){
  dhActiveTab=tab;
  document.querySelectorAll('.dh-tab').forEach(t=>t.classList.toggle('active',t.dataset.tab===tab));
  document.querySelectorAll('.dh-tabpane').forEach(p=>p.classList.toggle('show',p.dataset.pane===tab));
  if(tab==='truong'){schoolSearchQuery='';schoolFilterMien='Tất cả';renderSchoolList();}
}
function buildDH(){
  const n=NGANH.find(x=>x.id===selN);if(!n)return;
  const ch=CO_HOI[selN];
  const mainTH=n.dh[0].split(':')[0].trim();
  dhActiveTab='tohop';
  document.getElementById('dh-result').innerHTML=`
    <div class="cdung">"${n.tomtat}"</div>
    <div class="dh-card">
      <div class="dh-card-head">
        <div class="dh-nganh-icon">${n.icon}</div>
        <div style="flex:1;min-width:0">
          <div class="dh-nganh-name">${n.ten}</div>
          <div class="dh-nganh-sub">${n.dh.slice(0,4).map(d=>d.split(':')[0]).join(' · ')}</div>
        </div>
      </div>
      <div class="dh-tabs">
        <button class="dh-tab active" data-tab="tohop" onclick="switchDHTab('tohop')">Tổ hợp & môn</button>
        <button class="dh-tab" data-tab="truong" onclick="switchDHTab('truong')">Trường & điểm</button>
        <button class="dh-tab" data-tab="nghe" onclick="switchDHTab('nghe')">Cơ hội nghề</button>
      </div>
      <div class="dh-tabpane show" data-pane="tohop">
        <div class="dh-section">
          <div class="dh-slabel">Tổ hợp xét tuyển đại học</div>
          <div class="dh-pills">${n.dh.map(d=>{const code=d.split(':')[0].trim();const isStar=code===mainTH;return`<span class="dh-pill${isStar?' dh-pill-star':''}">${d}${isStar?' ★':''}</span>`;}).join('')}</div>
        </div>
        <div class="dh-section">
          <div class="dh-slabel">Môn học cần chú ý từ lớp 10</div>
          ${n.mon_txt.map(m=>`<div class="dh-mon-row">${m}</div>`).join('')}
        </div>
        ${n.warn?`<div style="margin:.25rem 1.25rem .5rem;padding:8px 12px;border-left:2px solid #e24b4a;background:#fff0f0;border-radius:0 8px 8px 0;font-size:12px;color:#a32d2d;line-height:1.5">⚠️ ${n.warn}</div>`:''}
        <div style="margin:.25rem 1.25rem .75rem;padding:9px 12px;background:#fff0f0;border-left:2px solid #e24b4a;border-radius:0 8px 8px 0;font-size:12px;color:#a32d2d;line-height:1.5">📋 <strong>Quy chế xét học bạ 2026:</strong> Tính cả <strong>6 học kỳ</strong>, đạt tối thiểu <strong>15/30 điểm</strong> ở 3 môn thi TN tương ứng.</div>
      </div>
      <div class="dh-tabpane" data-pane="truong">
        ${(()=>{
          const mienData=NGANH_TRUONG_MIEN[selN];
          const allSchools=mienData?[...mienData.B,...mienData.T,...mienData.N]:[];
          const total=allSchools.length;
          const diemRange=total>0?{min:Math.min(...allSchools.map(s=>s.diem)),max:Math.max(...allSchools.map(s=>s.diem))}:null;
          const hpList=allSchools.filter(s=>s.hp>0).map(s=>s.hp);
          const hpRange=hpList.length>0?{min:Math.min(...hpList),max:Math.max(...hpList)}:null;
          return`<div class="dh-stat-grid">
            <div class="dh-stat"><div class="dh-stat-val">${diemRange?diemRange.min.toFixed(1)+'–'+diemRange.max.toFixed(1):'—'}</div><div class="dh-stat-lbl">Điểm chuẩn 2024</div></div>
            <div class="dh-stat"><div class="dh-stat-val">${hpRange?hpRange.min+'–'+hpRange.max+'tr':'—'}</div><div class="dh-stat-lbl">Học phí/năm</div></div>
            <div class="dh-stat"><div class="dh-stat-val">${ch?ch.luong:'—'}</div><div class="dh-stat-lbl">Lương sau ra trường</div></div>
          </div>`;
        })()}
        ${(()=>{
          const mienData=NGANH_TRUONG_MIEN[selN];
          if(!mienData)return`<div class="dh-section"><p style="font-size:12px;color:var(--text3)">Đang cập nhật dữ liệu trường đào tạo cho ngành này.</p></div>`;
          const renderCol=(label,list,colorClass)=>{
            if(list.length===0)return`<div class="mien-col"><div class="mien-head ${colorClass}">${label}<span class="mien-count">0</span></div><div class="mien-empty">Chưa có dữ liệu</div></div>`;
            const rows=list.map(s=>{
              const isDN=s.t.includes('Đồng Nai')||s.t.includes('Lạc Hồng');
              const hpTxt=s.hp>0?s.hp+'tr/năm':'Miễn phí';
              const dcCls=s.diem>=26?'dh-chip-high':s.diem>=23?'dh-chip-mid':'dh-chip-ok';
              return`<div class="mien-item${isDN?' mien-item-dn':''}">
                <div class="mien-item-name">${isDN?'📍 ':''}${s.t}</div>
                <div class="mien-item-meta">
                  <span class="mien-tag">${s.th}</span>
                  <span class="mien-tag ${dcCls}">${s.diem.toFixed(1)}đ</span>
                  <span class="mien-tag mien-tag-ct">${s.ct} CT</span>
                  <span class="mien-tag mien-tag-hp">${hpTxt}</span>
                </div>
              </div>`;
            }).join('');
            return`<div class="mien-col"><div class="mien-head ${colorClass}">${label}<span class="mien-count">${list.length}</span></div><div class="mien-list">${rows}</div></div>`;
          };
          return`<div class="dh-section">
            <div class="dh-slabel" style="margin-bottom:.5rem">Trường đào tạo ngành này trên cả nước &nbsp;<span style="font-weight:400;color:var(--text3);font-size:10px">(${mienData.B.length+mienData.T.length+mienData.N.length}/207 trường) · ★ Khối · Điểm chuẩn 2024 · Chỉ tiêu (CT) · Học phí/năm</span></div>
            <div class="mien-grid">
              ${renderCol('🔵 Miền Bắc',mienData.B,'mien-bac')}
              ${renderCol('🟢 Miền Trung',mienData.T,'mien-trung')}
              ${renderCol('🟠 Miền Nam',mienData.N,'mien-nam')}
            </div>
            <p style="font-size:10px;color:var(--text3);margin-top:6px">📍 = Đồng Nai/Lạc Hồng. Điểm chuẩn, chỉ tiêu, học phí 2024 — chỉ tham khảo định hướng, thay đổi theo đề án tuyển sinh hằng năm.</p>
          </div>`;
        })()}
        <div style="padding:.75rem 1.25rem">
          <p style="font-size:11px;color:var(--text3);margin-bottom:8px">Học phí, chỉ tiêu cụ thể từng trường thay đổi theo đề án tuyển sinh hằng năm. Liên hệ HNA để được tư vấn cập nhật.</p>
          <a href="tel:0969374411" class="dh-ts247-btn">📞 Liên hệ HNA tư vấn — 096 937 4411</a>
        </div>
        <div class="dh-section">
          <div class="dh-slabel" style="margin-bottom:.5rem">Tra cứu 207 trường ĐH cả nước &nbsp;<span style="font-weight:400;color:var(--text3);font-size:10px" id="sch207-count">207 / 207 trường</span></div>
          <input type="text" class="sch207-search" placeholder="Tìm tên trường hoặc mã trường (VD: Bách Khoa, KHA)..." oninput="schoolSearchInput(this.value)">
          <div class="sch207-filters">
            <button class="sch207-filter active" onclick="schoolFilterClick('Tất cả',this)">Tất cả</button>
            <button class="sch207-filter" onclick="schoolFilterClick('Bắc',this)">Miền Bắc</button>
            <button class="sch207-filter" onclick="schoolFilterClick('Trung',this)">Miền Trung</button>
            <button class="sch207-filter" onclick="schoolFilterClick('Nam',this)">Miền Nam</button>
          </div>
          <div class="sch207-list" id="school207-list"></div>
        </div>
      </div>
      <div class="dh-tabpane" data-pane="nghe">
        ${ch?`<div class="dh-section"><div class="dh-slabel">Vị trí việc làm phổ biến</div><div>${ch.jobs.map(j=>`<div class="co-hoi-item">${j}</div>`).join('')}</div></div><div class="dh-section"><div class="dh-slabel">Thu nhập & nhu cầu thị trường</div><div class="luong-box"><div><div class="luong-val">${ch.luong}</div><div class="luong-lbl">Mức lương tham khảo</div></div><div style="flex:1;border-left:0.5px solid var(--border);padding-left:10px;font-size:12px;color:#27500a;line-height:1.5">${ch.nhu}</div></div></div>`:`<div class="dh-section"><p style="font-size:12px;color:var(--text3)">Đang cập nhật dữ liệu cơ hội nghề nghiệp cho ngành này.</p></div>`}
        <div style="padding:.75rem 1.25rem">
          <a href="tel:0969374411" class="dh-ts247-btn">📞 Liên hệ HNA tư vấn ngành này — 096 937 4411</a>
        </div>
      </div>
    </div>`;
}

const ALL_SCHOOLS=[
  {ten:'THPT Ngô Quyền',       tohop:{B00:'Tổ hợp A: Lý, Hóa, Sinh, Tin',A00:'Tổ hợp A: Lý, Hóa, Sinh, Tin',D07:'Tổ hợp A: Lý, Hóa, Sinh, Tin',D01:'Tổ hợp B/C: Hóa,Sinh,GDKTPL,CN hoặc Địa,CN,Tin,GDKTPL',C00:'Tổ hợp C: Địa, CN, Tin, GDKTPL',V00:'Tổ hợp D: Lý, Hóa, Địa, CN'}},
  {ten:'THPT Trấn Biên',        tohop:{A00:'Tổ hợp A: Lý, Hóa, Tin + 1 môn',B00:'Tổ hợp A: Lý, Hóa, Tin + 1 môn',D01:'Tổ hợp C: Địa, GDKTPL, Tin, CN',C00:'Tổ hợp C: Địa, GDKTPL, Tin, CN'}},
  {ten:'THPT Chu Văn An',       tohop:{A00:'Tổ hợp A: Lý, Hóa, Sinh, Tin',B00:'Tổ hợp A/B: Lý,Hóa,Sinh,Tin hoặc Lý,Hóa,Sinh,CN CN',D07:'Tổ hợp A: Lý, Hóa, Sinh, Tin',D01:'Tổ hợp C/D: Tin,Địa,GDKTPL,CN CN hoặc CN NN',C00:'Tổ hợp C/D: Tin, Địa, GDKTPL, CN NN'}},
  {ten:'THPT Lê Hồng Phong',    tohop:{A00:'Cần xác nhận — lehongphongdongnai.edu.vn',B00:'Cần xác nhận — lehongphongdongnai.edu.vn'}},
  {ten:'THPT Nguyễn Trãi',      tohop:{A00:'Cần xác nhận — SĐT: 0251 3884 351'}},
  {ten:'THPT Tam Hiệp',         tohop:{A00:'Cần xác nhận — website nhà trường'}},
  {ten:'THPT Nam Hà',           tohop:{A00:'Cần xác nhận — website nhà trường'}},
  {ten:'THPT Nguyễn Hữu Cảnh',  tohop:{A00:'Cần xác nhận — website nhà trường'}},
  {ten:'THPT Long Khánh',       tohop:{A00:'Cần xác nhận — website nhà trường'}},
  {ten:'THPT Long Thành',       tohop:{A00:'Cần xác nhận — website nhà trường'}},
  {ten:'THPT Xuân Lộc',         tohop:{A00:'Cần xác nhận — website nhà trường'}},
];

const CHUNG_TABLE=[
  // ── NHÓM A: TOÁN – LÝ – HÓA/ANH/TIN ─────────────────────────────────────────────
  {dh:'A00',mon3:'Toán – Vật lý – Hóa học',     l10:'Chọn tổ hợp có Vật lý + Hóa học',    nganh:'Kỹ thuật, CNTT, Cơ khí, Xây dựng, Hàng không, Hàng hải, Thủy lợi, Khí tượng, CN Vật liệu, Bán dẫn'},
  {dh:'A01',mon3:'Toán – Vật lý – Tiếng Anh',   l10:'Chọn tổ hợp có Vật lý + Tiếng Anh',  nganh:'CNTT, Kỹ thuật điện tử, Cơ khí, Xây dựng, Hàng không, Ngoại thương, Công an–Quân đội (⭐ nhiều trường kỹ thuật ưu tiên hơn A00)'},
  {dh:'A02',mon3:'Toán – Vật lý – Sinh học',     l10:'Chọn tổ hợp có Vật lý + Sinh học',   nganh:'Kỹ thuật Y học, KHTN, Y tế cộng đồng, Môi trường'},
  {dh:'X06',mon3:'Toán – Vật lý – Tin học',      l10:'Chọn tổ hợp có Vật lý + Tin học',   nganh:'CNTT, An toàn mạng, Hàng không (chính thức 2026 — ĐH Công Nghệ ĐHQG HN)'},
  // ── NHÓM B: TOÁN – HÓA – SINH/ANH ────────────────────────────────────────────
  {dh:'B00',mon3:'Toán – Hóa học – Sinh học',    l10:'Chọn tổ hợp có Hóa học + Sinh học',  nganh:'Y – Dược, Bác sĩ thú y, CN Sinh–Hóa, CN Thực phẩm, Nông–Lâm–Thủy sản'},
  {dh:'B03',mon3:'Toán – Sinh học – Ngữ văn',    l10:'Chọn tổ hợp có Sinh học',            nganh:'Bác sĩ thú y, Nông–Lâm–Thủy sản'},
  {dh:'B08',mon3:'Toán – Sinh học – Tiếng Anh',  l10:'Chọn tổ hợp có Sinh học + Tiếng Anh', nganh:'Điều dưỡng, Y tế cộng đồng, Dinh dưỡng, CN Sinh học'},
  // ── NHÓM C: NGỮ VĂN – CÁC KẾT HỢP ───────────────────────────────────────────
  {dh:'C00',mon3:'Ngữ văn – Lịch sử – Địa lý',  l10:'Chọn tổ hợp có Địa lý + Lịch sử',   nganh:'Luật, Sư phạm KHXH, Báo chí, Tâm lý, Du lịch, Mỹ thuật – Âm nhạc'},
  {dh:'C01',mon3:'Ngữ văn – Toán – Vật lý',      l10:'Chọn tổ hợp có Vật lý',              nganh:'Điện–Điện tử, Hàng hải, CN In–Giấy, Mỏ–Địa chất, Xây dựng'},
  {dh:'C02',mon3:'Ngữ văn – Toán – Hóa học',     l10:'Chọn tổ hợp có Hóa học',             nganh:'Hóa học, CN Thực phẩm, Môi trường, Dược học (một số trường)'},
  {dh:'C03',mon3:'Ngữ văn – Toán – Lịch sử',     l10:'Chọn tổ hợp có Lịch sử',             nganh:'Tâm lý học, Quân đội–Chính trị, Luật'},
  {dh:'C04',mon3:'Ngữ văn – Toán – Địa lý',      l10:'Chọn tổ hợp có Địa lý',              nganh:'Du lịch, Khách sạn, Sư phạm Địa lý, Kinh tế'},
  // ── NHÓM D01: TOÁN – VĂN – TIẾNG ANH (PHỔ BIẾN NHẤT) ─────────────────────────
  {dh:'D01',mon3:'Toán – Ngữ văn – Tiếng Anh',   l10:'Học Tiếng Anh tốt từ lớp 10',        nganh:'Kinh tế, QTKD, Luật, Du lịch, Báo chí, Ngoại giao, Sư phạm, Tâm lý'},
  {dh:'D07',mon3:'Toán – Hóa học – Tiếng Anh',   l10:'Chọn tổ hợp có Hóa học + Tiếng Anh', nganh:'Tài chính, Ngân hàng, Kế toán, Ngoại thương, CN Thực phẩm (dùng chung nhiều ngành)'},
  {dh:'D09',mon3:'Toán – Lịch sử – Tiếng Anh',   l10:'Học Tiếng Anh + chọn tổ hợp có Lịch sử', nganh:'Ngoại giao, Kinh tế, Luật, Sư phạm Lịch sử'},
  {dh:'D10',mon3:'Toán – Địa lý – Tiếng Anh',    l10:'Học Tiếng Anh + chọn tổ hợp có Địa lý',  nganh:'Du lịch, Địa lý học, Kinh tế, Ngoại giao'},
  // ── NHÓM D NGOẠI NGỮ: VĂN – TOÁN – NGOẠI NGỮ ──────────────────────────────
  {dh:'D04',mon3:'Ngữ văn – Toán – Tiếng Trung',  l10:'Học Tiếng Trung tốt từ lớp 10',     nganh:'Tiếng Trung, Ngoại ngữ, Kinh doanh QT, Du lịch Trung Quốc'},
  {dh:'D06',mon3:'Ngữ văn – Toán – Tiếng Nhật',   l10:'Học Tiếng Nhật tốt từ lớp 10',      nganh:'Tiếng Nhật, Ngoại ngữ, Kinh doanh với Nhật Bản'},
  {dh:'D03',mon3:'Ngữ văn – Toán – Tiếng Pháp',   l10:'Học Tiếng Pháp tốt từ lớp 10',      nganh:'Tiếng Pháp, Ngoại ngữ, Quan hệ QT'},
  {dh:'D02',mon3:'Ngữ văn – Toán – Tiếng Nga',    l10:'Học Tiếng Nga tốt từ lớp 10',       nganh:'Tiếng Nga, Ngoại ngữ, Quan hệ QT'},
  {dh:'D05',mon3:'Ngữ văn – Toán – Tiếng Đức',    l10:'Học Tiếng Đức tốt từ lớp 10',       nganh:'Tiếng Đức, Ngoại ngữ, Quan hệ QT'},
  // ── NHÓM D NGOẠI NGỮ: TOÁN – LÝ/HÓA – NGOẠI NGỮ ──────────────────────────
  {dh:'D28',mon3:'Toán – Vật lý – Tiếng Nhật',    l10:'Chọn tổ hợp có Vật lý + Tiếng Nhật', nganh:'KT điện tử, CNTT hướng Nhật Bản'},
  {dh:'D29',mon3:'Toán – Vật lý – Tiếng Pháp',    l10:'Chọn tổ hợp có Vật lý + Tiếng Pháp', nganh:'Kỹ thuật, CNTT hướng Pháp ngữ'},
  {dh:'D26',mon3:'Toán – Vật lý – Tiếng Đức',     l10:'Chọn tổ hợp có Vật lý + Tiếng Đức',  nganh:'Kỹ thuật, CNTT hướng Đức'},
  {dh:'D23',mon3:'Toán – Hóa học – Tiếng Nhật',   l10:'Chọn tổ hợp có Hóa học + Tiếng Nhật', nganh:'Hóa học, CN Thực phẩm hướng Nhật Bản'},
  {dh:'D24',mon3:'Toán – Hóa học – Tiếng Pháp',   l10:'Chọn tổ hợp có Hóa học + Tiếng Pháp', nganh:'Hóa học, CN Thực phẩm hướng Pháp ngữ'},
  // ── NHÓM D14/D15: VĂN – SỬ/ĐỊA – ANH ──────────────────────────────────
  {dh:'D14',mon3:'Ngữ văn – Lịch sử – Tiếng Anh', l10:'Học Tiếng Anh + chọn tổ hợp có Lịch sử', nganh:'Ngoại giao, Ngoại ngữ, QH Quốc tế, Sư phạm'},
  {dh:'D15',mon3:'Ngữ văn – Địa lý – Tiếng Anh',  l10:'Học Tiếng Anh + chọn tổ hợp có Địa lý',  nganh:'Ngoại giao, Du lịch, Khách sạn, Địa lý'},
  // ── NHÓM X: TỔ HỢP GDKTPL (CHƯƠNG TRÌNH 2018 MỚI) ────────────────────────────────
  {dh:'X01',mon3:'Ngữ văn – Toán – GDKTPL',       l10:'Chọn tổ hợp có GDKTPL',              nganh:'Thiết kế đồ họa, Game, Đa phương tiện, Kinh tế, Luật'},
  {dh:'X21',mon3:'Toán – Địa lý – GDKTPL',         l10:'Chọn tổ hợp có Địa lý + GDKTPL',   nganh:'Du lịch, Kinh tế, Quản lý đất đai, Địa lý'},
  {dh:'X70',mon3:'Ngữ văn – Lịch sử – GDKTPL',    l10:'Chọn tổ hợp có Lịch sử + GDKTPL',  nganh:'Luật, KHXH, Sư phạm, Văn hóa–Chính trị'},
  {dh:'X74',mon3:'Ngữ văn – Địa lý – GDKTPL',     l10:'Chọn tổ hợp có Địa lý + GDKTPL',   nganh:'Du lịch, Địa lý, KHXH, Sư phạm Địa lý'},
  {dh:'X78',mon3:'Ngữ văn – GDKTPL – Tiếng Anh',  l10:'Học Tiếng Anh + chọn tổ hợp có GDKTPL', nganh:'Truyền thông đa phương tiện, Luật QT, Kinh tế, Ngôn ngữ'},
  // ── NHÓM V: VẼ KỸ THUẬT ──────────────────────────────────────────────────────────────────
  {dh:'V00',mon3:'Toán – Vẽ kỹ thuật – Vật lý',   l10:'Học Vẽ KT riêng ngoài trường',      nganh:'Kiến trúc, Quy hoạch đô thị, Thiết kế nội thất'},
  // ── NHÓM H: NĂNG KHIẾU MỸ THUẬT ─────────────────────────────────────────────────
  {dh:'H00',mon3:'Ngữ văn – NK Vẽ 1 – NK Vẽ 2',  l10:'Luyện năng khiếu vẽ từ lớp 10',     nganh:'Mỹ thuật, Thiết kế đồ họa (thi năng khiếu riêng)'},
  {dh:'H01',mon3:'Ngữ văn – NK Vẽ 1 – Toán',      l10:'Luyện năng khiếu vẽ từ lớp 10',     nganh:'Mỹ thuật ứng dụng, Kiến trúc (một số trường)'},
  // ── NHÓM N: NĂNG KHIẾU ÂM NHẠC ──────────────────────────────────────────────────
  {dh:'N00',mon3:'Ngữ văn – Hòa âm – Hát',        l10:'Luyện âm nhạc chuyên sâu từ sớm',   nganh:'Âm nhạc, Biểu diễn, Thanh nhạc, SP Âm nhạc'},
  {dh:'N01',mon3:'Ngữ văn – Đàn – Nhạc lý',        l10:'Luyện âm nhạc chuyên sâu từ sớm',   nganh:'Biểu diễn nhạc cụ, Âm nhạc học'},
  // ── NHÓM T: NĂNG KHIẾU TDTT ───────────────────────────────────────────────────────
  {dh:'T00',mon3:'Toán – Sinh học – NK TDTT',       l10:'Rèn luyện thể thao chuyên sâu',      nganh:'Thể dục – Thể thao (thi năng khiếu TDTT riêng)'},
  {dh:'T01',mon3:'Toán – Ngữ văn – NK TDTT',        l10:'Rèn luyện thể thao chuyên sâu',      nganh:'Giáo dục thể chất, Huấn luyện thể thao'},
  {dh:'T02',mon3:'Ngữ văn – Sinh học – NK TDTT',    l10:'Rèn luyện thể thao chuyên sâu',      nganh:'Thể dục – Thể thao, Y học thể thao'},
  // ── NHÓM Q: ĐÁNH GIÁ TƯ DUY ───────────────────────────────────────────────────────────────
  {dh:'Q00',mon3:'Tư duy định lượng – Định tính – KH/Tiếng Anh', l10:'Ôn đề thi ĐGTD riêng', nganh:'Công an – Quân đội (thi Đánh giá tư duy BCA)'},
  // ── B08/D08: SINH – ANH ─────────────────────────────────────────────────────────────────
  {dh:'D08',mon3:'Toán – Sinh học – Tiếng Anh',     l10:'Chọn tổ hợp có Sinh học + Tiếng Anh', nganh:'Điều dưỡng, Y tế cộng đồng, CN Sinh học'},
  // ── BỔ SUNG ĐỦ TOP 50 ──────────────────────────────────────────────────────────────────
  {dh:'D27',mon3:'Toán – Vật lý – Tiếng Nga',       l10:'Chọn tổ hợp có Vật lý + Tiếng Nga',  nganh:'Kỹ thuật, Khoa học tự nhiên, Ngoại ngữ Nga'},
  {dh:'A08',mon3:'Toán – Vật lý – Hóa học – Tiếng Anh', l10:'Chọn tổ hợp có Vật lý + Hóa học', nganh:'CNTT, Kỹ thuật (chương trình quốc tế một số trường)'},
  {dh:'D11',mon3:'Ngữ văn – Sinh học – Tiếng Anh',  l10:'Chọn tổ hợp có Sinh học + Tiếng Anh', nganh:'Điều dưỡng, Y tế cộng đồng, SP Sinh học'},
  {dh:'C15',mon3:'Ngữ văn – Toán – Tiếng Anh',      l10:'Học Tiếng Anh tốt (thang điểm Anh văn)', nganh:'SP Tiếng Anh, Ngoại ngữ, Kinh tế (một số trường)'},
  {dh:'X25',mon3:'Toán – Hóa học – GDKTPL',         l10:'Chọn tổ hợp có Hóa học + GDKTPL',    nganh:'Kinh tế, Tài chính, CN Thực phẩm (tổ hợp mới 2025)'},
  {dh:'X26',mon3:'Toán – Sinh học – GDKTPL',         l10:'Chọn tổ hợp có Sinh học + GDKTPL',   nganh:'Nông nghiệp, Môi trường, Y tế cộng đồng (tổ hợp mới 2025)'},
  {dh:'X35',mon3:'Toán – Lịch sử – GDKTPL',          l10:'Chọn tổ hợp có Lịch sử + GDKTPL',   nganh:'Luật, Hành chính, KHXH (tổ hợp mới 2025)'},
];

function buildSchool(){
  const n=NGANH.find(x=>x.id===selN);if(!n)return;
  document.getElementById('school-input').value='';
  document.getElementById('school-search-result').innerHTML='';
  document.getElementById('school-result').innerHTML=`
    <div class="rcard hl">
      <div class="rl">Môn lựa chọn cần đăng ký khi nhập học lớp 10</div>
      <div class="tags" style="margin-top:6px">${n.tohop_l10.map(t=>`<span class="tag tag-amber">${t}</span>`).join('')}</div>
      <div class="divider"></div>
      <div class="rl">Lưu ý quan trọng</div>
      <div class="cdung">Môn bạn chọn ở lớp 10 sẽ học xuyên suốt 10–11–12 và quyết định trực tiếp tổ hợp thi tốt nghiệp + xét tuyển đại học. Chọn sai rất khó sửa — hãy quyết định kỹ!</div>
      ${n.warn?`<div class="warn-box">⚠️ ${n.warn}</div>`:''}
    </div>`;
  buildChung();
}

function searchSchool(val){
  const n=NGANH.find(x=>x.id===selN);
  const mainKey=n?n.dh[0].split(':')[0].trim():'A00';
  const box=document.getElementById('school-search-result');
  const q=val.trim().toLowerCase();
  if(q.length<2){box.innerHTML='';return;}
  const found=ALL_SCHOOLS.filter(s=>s.ten.toLowerCase().includes(q));
  if(found.length===0){
    box.innerHTML=`<div class="school-notfound">
      Không tìm thấy "<strong>${val}</strong>" trong dữ liệu.<br>
      Xem bảng tổ hợp chung bên dưới để biết môn cần chọn, hoặc liên hệ HNA để được tư vấn trực tiếp cho trường của bạn.
    </div>`;
  } else {
    box.innerHTML=found.map(s=>{
      const info=s.tohop[mainKey]||'Cần xác nhận thêm với nhà trường';
      return`<div class="school-found">
        <strong>${s.ten}</strong><br>
        Tổ hợp phù hợp: ${info}
      </div>`;
    }).join('');
  }
}

function buildChung(){
  const n=NGANH.find(x=>x.id===selN);

  // Tính mainKey thông minh: nếu HS đã chọn 2 môn thi TN → so khớp với dh array
  let mainKey='';
  if(n){
    if(selTnMons&&selTnMons.length===2){
      // Tổ hợp = Toán + Văn + 2 môn TN — so khớp với dh array
      const monIds=selTnMons.map(m=>m.id);
      const TH_MON_MAP={
        'A00':['ly','hoa'],'A01':['ly'],'B00':['hoa','sinh'],
        'D07':['hoa'],'C00':['dia','su'],'D01':[],'X06':['ly','tin'],
        'B03':['sinh'],'C04':['dia'],'D14':['su'],'D15':['dia'],
        'C00':['dia','su'],'C03':['su'],
      };
      // Tìm tổ hợp trong dh array khớp nhiều nhất với môn thi TN
      let bestCode='', bestScore=-1;
      n.dh.forEach(d=>{
        const code=d.split(':')[0].trim();
        const needed=TH_MON_MAP[code]||[];
        const score=needed.filter(m=>monIds.includes(m)).length - needed.filter(m=>!monIds.includes(m)).length;
        if(score>bestScore){bestScore=score;bestCode=code;}
      });
      mainKey=bestCode||n.dh[0].split(':')[0].trim();
    } else {
      mainKey=n.dh[0].split(':')[0].trim();
    }
  }

  const NGANH_DETAIL={
    'A00':{nganh_chi:'Kỹ thuật cơ khí, Kỹ thuật điện–điện tử, CNTT, Xây dựng, Hàng không, Hàng hải, Thủy lợi, Khí tượng–Thủy văn, CN Bán dẫn, Vật liệu, Môi trường',truong:'ĐH Bách Khoa HN/HCM, ĐH SP Kỹ Thuật HCM, ĐH Công Nghiệp HN/HCM, ĐH Hàng Hải VN, ĐH Thủy Lợi, ĐH Lạc Hồng'},
    'A01':{nganh_chi:'CNTT, Kỹ thuật điện tử, Cơ khí, Xây dựng, Hàng không, Ngoại thương, Công an–Quân đội ⭐ Xu hướng 2025–2026: nhiều trường kỹ thuật mở rộng xét A01 hơn A00 — nên ưu tiên giữ Tiếng Anh tốt',truong:'ĐH Bách Khoa HN/HCM, ĐH CNTT HCM, FPT University, ĐH Ngoại Thương, HV Cảnh Sát ND'},
    'B00':{nganh_chi:'Y khoa, Dược học, Điều dưỡng, RHM, CN Sinh–Hóa, Nông–Lâm–Thủy sản',truong:'ĐH Y Dược HCM, ĐH Y HN, ĐH Y Dược Huế, ĐH Nông Lâm HCM, ĐH Y khoa Phạm Ngọc Thạch'},
    'D01':{nganh_chi:'Kinh tế, QTKD, Luật, Du lịch, Báo chí, Ngoại giao, Sư phạm, Tâm lý',truong:'ĐH Kinh Tế QD, ĐH Kinh Tế HCM (UEH), ĐH Ngoại Thương, ĐH Luật HN/HCM, ĐH KHXH&NV'},
    'D07':{nganh_chi:'Tài chính, Ngân hàng, Kế toán, Kiểm toán, Ngoại thương, CN Thực phẩm',truong:'HV Tài Chính, HV Ngân Hàng, ĐH Kinh Tế QD, ĐH Kinh Tế HCM (UEH), ĐH Ngoại Thương'},
    'C00':{nganh_chi:'Luật, Sư phạm KHXH, Báo chí–Truyền thông, Tâm lý, Du lịch, Mỹ thuật–Âm nhạc',truong:'ĐH Luật HN/HCM, ĐH KHXH&NV HN/HCM, HV Báo Chí, ĐH SP HN/HCM'},
    'X06':{nganh_chi:'CNTT, An toàn mạng, KT Phần mềm (tổ hợp MỚI từ 2025)',truong:'ĐH Công Nghệ–ĐHQG HN, ĐH Bách Khoa HN, ĐH CNTT HCM'},
    'X01':{nganh_chi:'Thiết kế đồ họa, Game, Đa phương tiện',truong:'ĐH Mỹ Thuật VN/HCM, FPT University, ĐH Văn Lang, ĐH HUTECH'},
    'V00':{nganh_chi:'Kiến trúc, Quy hoạch đô thị, Thiết kế nội thất',truong:'ĐH Kiến Trúc HN/HCM, ĐH Xây Dựng HN'},
    'B03':{nganh_chi:'Bác sĩ thú y, Nông–Lâm–Thủy sản',truong:'ĐH Nông Lâm HCM/HN, ĐH Nha Trang, ĐH Cần Thơ'},
    'C04':{nganh_chi:'Du lịch–Khách sạn, Sư phạm Địa lý',truong:'ĐH Hoa Sen, ĐH Văn Lang, ĐH Đà Lạt, ĐH KHXH&NV HCM'},
    'D14':{nganh_chi:'Ngoại giao, Ngoại ngữ',truong:'HV Ngoại Giao, ĐH Ngoại Ngữ–ĐHQG HN, ĐH Hà Nội'},
    'D15':{nganh_chi:'Ngoại giao, Du lịch–Lữ hành',truong:'HV Ngoại Giao, ĐH Đà Lạt, ĐH KHXH&NV HCM'},
    'C01':{nganh_chi:'Điện–Điện tử, Hàng hải, Mỏ–Địa chất',truong:'ĐH Bách Khoa HN/HCM, ĐH Hàng Hải VN'},
    'C03':{nganh_chi:'Tâm lý, Quân đội Chính trị',truong:'ĐH KHXH&NV HN, Trường Sĩ Quan Chính Trị'},
    'H00':{nganh_chi:'Mỹ thuật, Thiết kế đồ họa (thi năng khiếu)',truong:'ĐH Mỹ Thuật VN, ĐH Mỹ Thuật HCM, ĐH Kiến Trúc'},
    'T00':{nganh_chi:'Thể dục–Thể thao (thi năng khiếu)',truong:'ĐH SP TDTT HN, ĐH SP TDTT HCM'},
    'T01':{nganh_chi:'Thể dục–Thể thao (thi năng khiếu)',truong:'ĐH SP TDTT HN, ĐH SP TDTT ĐN'},
    'A02':{nganh_chi:'Kỹ thuật Y học, Khoa học tự nhiên, Y tế cộng đồng',truong:'ĐH Bách Khoa HN/HCM, ĐH Khoa học TN HN/HCM'},
    'B08':{nganh_chi:'Điều dưỡng, Dinh dưỡng, Y tế cộng đồng, CN Sinh học',truong:'ĐH Y Dược HCM, ĐH Y HN, ĐH Nông Lâm HCM'},
    'C02':{nganh_chi:'Hóa học, CN Thực phẩm, Môi trường, Dược (một số trường)',truong:'ĐH Khoa học TN HN/HCM, ĐH Bách Khoa HN/HCM'},
    'D09':{nganh_chi:'Ngoại giao, Kinh tế, Luật, Sư phạm Lịch sử',truong:'HV Ngoại Giao, ĐH KHXH&NV HN/HCM, ĐH Luật HN'},
    'D10':{nganh_chi:'Du lịch, Địa lý học, Kinh tế, Ngoại giao',truong:'ĐH KHXH&NV HN/HCM, ĐH Đà Lạt, ĐH Hoa Sen'},
    'D08':{nganh_chi:'Điều dưỡng, Y tế cộng đồng, CN Sinh học',truong:'ĐH Y Dược HCM, ĐH Y HN, ĐH Nông Lâm HCM'},
    'D04':{nganh_chi:'Tiếng Trung, Ngoại ngữ, Kinh doanh QT',truong:'ĐH Ngoại Ngữ ĐHQG HN, ĐH KHXH&NV HCM, ĐH Hà Nội'},
    'D06':{nganh_chi:'Tiếng Nhật, Ngoại ngữ, Kinh doanh với Nhật Bản',truong:'ĐH Ngoại Ngữ ĐHQG HN, ĐH KHXH&NV HCM'},
    'D03':{nganh_chi:'Tiếng Pháp, Ngoại ngữ, Quan hệ QT',truong:'ĐH Ngoại Ngữ ĐHQG HN, ĐH Hà Nội'},
    'D02':{nganh_chi:'Tiếng Nga, Ngoại ngữ, Quan hệ QT',truong:'ĐH Ngoại Ngữ ĐHQG HN'},
    'D05':{nganh_chi:'Tiếng Đức, Ngoại ngữ, Quan hệ QT',truong:'ĐH Ngoại Ngữ ĐHQG HN'},
    'D27':{nganh_chi:'Kỹ thuật, Khoa học tự nhiên, Ngoại ngữ Nga',truong:'ĐH Bách Khoa HN, ĐH Ngoại Ngữ ĐHQG HN'},
    'D28':{nganh_chi:'Kỹ thuật điện tử, CNTT hướng Nhật Bản',truong:'ĐH Bách Khoa HN, FPT University'},
    'D29':{nganh_chi:'Kỹ thuật, CNTT hướng Pháp ngữ',truong:'ĐH Bách Khoa HN'},
    'D26':{nganh_chi:'Kỹ thuật, CNTT hướng Đức',truong:'ĐH Bách Khoa HN'},
    'D23':{nganh_chi:'Hóa học, CN Thực phẩm hướng Nhật Bản',truong:'ĐH Bách Khoa HN'},
    'D24':{nganh_chi:'Hóa học, CN Thực phẩm hướng Pháp ngữ',truong:'ĐH Bách Khoa HN'},
    'X21':{nganh_chi:'Du lịch, Kinh tế, Quản lý đất đai, Địa lý',truong:'ĐH Đà Lạt, ĐH Hoa Sen, ĐH Tài Nguyên Môi Trường'},
    'X70':{nganh_chi:'Luật, KHXH, Sư phạm, Văn hóa–Chính trị',truong:'ĐH Luật HN/HCM, ĐH KHXH&NV HN/HCM'},
    'X74':{nganh_chi:'Du lịch, Địa lý, KHXH, Sư phạm Địa lý',truong:'ĐH KHXH&NV HN/HCM, ĐH Đà Lạt'},
    'X78':{nganh_chi:'Truyền thông đa phương tiện, Luật QT, Kinh tế',truong:'HV Báo Chí, ĐH KHXH&NV HCM, ĐH Ngoại Thương'},
    'X25':{nganh_chi:'Kinh tế, Tài chính, CN Thực phẩm',truong:'Nhiều trường đang cập nhật đề án 2026'},
    'X26':{nganh_chi:'Nông nghiệp, Môi trường, Y tế cộng đồng',truong:'ĐH Nông Lâm HCM, ĐH Tài Nguyên Môi Trường'},
    'X35':{nganh_chi:'Luật, Hành chính, KHXH',truong:'ĐH Luật HN/HCM, ĐH KHXH&NV HN/HCM'},
    'H01':{nganh_chi:'Mỹ thuật ứng dụng, Kiến trúc (một số trường)',truong:'ĐH Mỹ Thuật Công Nghiệp HN, ĐH Kiến Trúc HN/HCM'},
    'N00':{nganh_chi:'Âm nhạc, Biểu diễn, Thanh nhạc, SP Âm nhạc',truong:'HV Âm Nhạc QG VN, ĐH Sân Khấu Điện Ảnh HN/HCM'},
    'N01':{nganh_chi:'Biểu diễn nhạc cụ, Âm nhạc học',truong:'HV Âm Nhạc QG VN, ĐH Sân Khấu Điện Ảnh'},
    'T02':{nganh_chi:'Thể dục–Thể thao, Y học thể thao',truong:'ĐH SP TDTT HN, ĐH SP TDTT HCM'},
    'Q00':{nganh_chi:'Công an–Quân đội (thi Đánh giá tư duy BCA)',truong:'HV Cảnh Sát ND, HV An Ninh ND'},
  };

  const cards=CHUNG_TABLE.map((r,i)=>{
    const isMain=r.dh===mainKey;
    const detail=NGANH_DETAIL[r.dh]||{nganh_chi:r.nganh,truong:'Liên hệ HNA: 096 937 4411 để được tư vấn cụ thể'};
    const uid=`acc-${i}`;
    return`<div class="acc-item${isMain?' acc-main':''}" id="${uid}">
      <button class="acc-head" onclick="toggleAcc('${uid}')" aria-expanded="false">
        <span class="acc-code${isMain?' acc-code-main':''}">${r.dh}${isMain?' ★':''}</span>
        <span class="acc-mon3">${r.mon3}</span>
        <span class="acc-chevron">▾</span>
      </button>
      <div class="acc-body" hidden>
        <div class="acc-row"><span class="acc-label">Môn cần chọn lớp 10</span><span class="acc-val accent">${r.l10}</span></div>
        <div class="acc-row"><span class="acc-label">Nhóm ngành phù hợp</span><span class="acc-val">${detail.nganh_chi}</span></div>
        <div class="acc-row"><span class="acc-label">Trường đào tạo tiêu biểu</span><span class="acc-val muted">${detail.truong}</span></div>
        ${isMain?`<div class="acc-highlight">★ Tổ hợp phù hợp với ngành <strong>${n?.ten||''}</strong> bạn đã chọn</div>`:''}
      </div>
    </div>`;
  }).join('');

  document.getElementById('chung-result').innerHTML=`
    <div class="rcard" style="margin-bottom:1rem">
      <div class="rl">Bảng tổ hợp chung — bấm vào tổ hợp để xem chi tiết</div>
      <p style="font-size:12px;color:var(--text3);margin:4px 0 10px">★ = tổ hợp ĐH phù hợp với ngành bạn đã chọn · Áp dụng cho mọi trường THPT</p>
      <div class="acc-list">${cards}</div>
    </div>
    <div class="hna-cta">
      <div class="hna-cta-txt">
        <div class="title">Cần tư vấn riêng cho từng học sinh?</div>
        <div class="sub">Liên hệ Hướng Nghiệp Alpha để được tư vấn chuyên sâu, cá nhân hóa theo năng lực, mục tiêu và định hướng phù hợp.</div>
      </div>
      <a href="tel:0969374411" class="btn-amber">📞 Gọi ngay 096 937 4411</a>
    </div>`;

  // Auto mở tổ hợp chủ lực
  if(mainKey){
    const mainEl=document.querySelector('.acc-main');
    if(mainEl){
      const btn=mainEl.querySelector('.acc-head');
      const body=mainEl.querySelector('.acc-body');
      if(btn&&body){body.hidden=false;btn.setAttribute('aria-expanded','true');btn.classList.add('open');}
    }
  }
}

function toggleAcc(uid){
  const item=document.getElementById(uid);
  if(!item)return;
  const btn=item.querySelector('.acc-head');
  const body=item.querySelector('.acc-body');
  const isOpen=!body.hidden;
  body.hidden=isOpen;
  btn.setAttribute('aria-expanded',String(!isOpen));
  btn.classList.toggle('open',!isOpen);
}


function goStep(s){
  if(s>=2&&selT.size<2)return;
  if(s>=3&&!selN)return;
  document.getElementById('flow-bar').style.display='flex';
  [1,2,3,4].forEach(i=>{
    document.getElementById('panel'+i).className='panel'+(i===s?' show':'');
    const f=document.getElementById('fs'+i);
    f.className='flow-step'+(i===s?' active':i<s?' done':'');
  });
  if(s===2)buildNganh();
  if(s===3)buildDH();
  if(s===4){buildSchool();buildMonChips();}
  window.scrollTo({top:0,behavior:'smooth'});
}

function resetAll(){
  selT.clear();selN=null;selMons=[];saOpenId=null;
  document.querySelectorAll('.tbtn').forEach(b=>b.classList.remove('sel'));
  document.getElementById('sbar-txt').textContent='Chưa chọn gì — hãy chọn ít nhất 2 mô tả bản thân';
  document.getElementById('sbar-cnt').textContent='0';
  document.getElementById('btn12').disabled=true;
  goStep(1);
}

const ALL_MONS=[
  {id:'ly',    label:'Vật lý'},
  {id:'hoa',   label:'Hóa học'},
  {id:'sinh',  label:'Sinh học'},
  {id:'tin',   label:'Tin học'},
  {id:'dia',   label:'Địa lý'},
  {id:'su',    label:'Lịch sử'},
  {id:'gdktpl',label:'GD KT&PL'},
  {id:'cn_cn', label:'CN Công nghiệp'},
  {id:'cn_nn', label:'CN Nông nghiệp'},
  {id:'am',    label:'Âm nhạc'},
  {id:'mt',    label:'Mỹ thuật'},
];

let selMons=[];

function buildMonChips(){
  selMons=[];
  document.getElementById('match-result').innerHTML='';
  document.getElementById('send-form').style.display='none';
  const el=document.getElementById('mon-chips');
  el.innerHTML=ALL_MONS.map(m=>
    `<button class="mon-chip" id="mc-${m.id}" onclick="toggleMon('${m.id}','${m.label}')">${m.label}</button>`
  ).join('');
  renderSlots();
}

function toggleMon(id,label){
  const idx=selMons.findIndex(m=>m.id===id);
  const btn=document.getElementById('mc-'+id);
  if(idx>=0){
    selMons.splice(idx,1);
    btn.classList.remove('picked');
  } else {
    if(selMons.length>=4){
      const first=selMons.shift();
      document.getElementById('mc-'+first.id)?.classList.remove('picked');
    }
    selMons.push({id,label});
    btn.classList.add('picked');
  }
  renderSlots();
}

function renderSlots(){
  const box=document.getElementById('tohop-slots');
  const btn=document.getElementById('btn-check');
  const tnSection=document.getElementById('tn-section');
  if(selMons.length===0){
    box.innerHTML='<span class="slots-hint">Chọn môn bên trên để thêm vào đây...</span>';
    btn.disabled=true;btn.style.opacity='.4';
    tnSection.classList.add('hidden');
  } else {
    box.innerHTML=selMons.map(m=>`
      <span class="slot-tag">${m.label}
        <button onclick="toggleMon('${m.id}','${m.label}')" aria-label="Xóa ${m.label}">×</button>
      </span>`).join('');
    const ready=selMons.length>=2;
    btn.disabled=!ready;btn.style.opacity=ready?'1':'.4';
    if(selMons.length>=2){
      tnSection.classList.remove('hidden');
      buildTnChips();
    } else {
      tnSection.classList.add('hidden');
    }
  }
}

let selTnMons=[];

function buildTnChips(){
  selTnMons=[];
  document.getElementById('tohop-xettuyen-result').innerHTML='';
  document.getElementById('tn-summary-bar').style.display='none';
  const el=document.getElementById('tn-chips');
  el.innerHTML=selMons.map(m=>
    `<button class="tn-chip" id="tn-${m.id}" onclick="toggleTnMon('${m.id}','${m.label}')">${m.label}</button>`
  ).join('');
}

function toggleTnMon(id,label){
  const idx=selTnMons.findIndex(m=>m.id===id);
  const btn=document.getElementById('tn-'+id);
  if(idx>=0){
    selTnMons.splice(idx,1);
    btn.classList.remove('picked');
  } else {
    if(selTnMons.length>=2){
      const first=selTnMons.shift();
      document.getElementById('tn-'+first.id)?.classList.remove('picked');
    }
    selTnMons.push({id,label});
    btn.classList.add('picked');
  }
  renderTnResult();
}

const TO_HOP_MAP={
  'ly-hoa':'A00','ly-tin':'X06','ly-sinh':'A02',
  'hoa-sinh':'B00','hoa-gdktpl':'X25',
  'dia-su':'C00','dia-gdktpl':'X74',
  'su-gdktpl':'X70',
  'ly-gdktpl':'X06','hoa-tin':'',
  'sinh-tin':'','sinh-dia':'','sinh-su':'B03','sinh-gdktpl':'X26',
};

const TH_NGANH_MAP={
  'A00':'Kỹ thuật, CNTT, Cơ khí, Y–Dược, Xây dựng',
  'A01':'CNTT quốc tế, Kỹ thuật điện tử, Ngoại thương',
  'A02':'Kỹ thuật Y học, Khoa học tự nhiên',
  'X06':'CNTT, An toàn mạng (chính thức 2026)',
  'B00':'Y khoa, Dược, Điều dưỡng, Nông–Lâm–Thủy sản',
  'B03':'Nông–Lâm, Bác sĩ thú y',
  'X25':'Kinh tế, Tài chính, CN Thực phẩm (mới 2025)',
  'X26':'Nông nghiệp, Môi trường, Y tế cộng đồng (mới 2025)',
  'C00':'Luật, Sư phạm XH, Báo chí, Tâm lý, Ngoại giao',
  'X70':'Luật, KHXH, Sư phạm, Văn hóa–Chính trị, Công tác xã hội',
  'X74':'Du lịch, Địa lý, KHXH, Sư phạm Địa lý',
};

function renderTnResult(){
  const bar=document.getElementById('tn-summary-bar');
  const resEl=document.getElementById('tohop-xettuyen-result');

  // Cập nhật progress
  const prog=document.getElementById('tn-progress');
  const hint=document.getElementById('tn-hint');
  if(prog) prog.textContent=`${selTnMons.length} / 2 môn`;
  if(hint){
    if(selTnMons.length===0) hint.textContent='← bấm vào môn bên dưới để chọn';
    else if(selTnMons.length===1) hint.textContent='Chọn thêm 1 môn nữa để xem sơ đồ';
    else hint.textContent='✓ Đủ 2 môn — sơ đồ hiện bên dưới';
  }

  if(selTnMons.length===0){
    bar.style.display='none';resEl.innerHTML='';return;
  }
  bar.style.display='flex';
  document.getElementById('tn-chosen-display').innerHTML=
    selTnMons.map(m=>`<span class="tn-chosen-pill">${m.label}</span>`).join('<span class="tn-plus" style="align-self:center">+</span>');

  if(selTnMons.length<2){resEl.innerHTML='';return;}

  const ids=selTnMons.map(m=>m.id).sort().join('-');
  const ids2=selTnMons.map(m=>m.id).sort((a,b)=>a>b?-1:1).join('-');

  const n=NGANH.find(x=>x.id===selN);
  // targetTH: tìm tổ hợp trong dh array của ngành khớp với môn HS đã chọn thi TN
  const TH_MON_MAP2={
    'A00':['ly','hoa'],'A01':['ly'],'B00':['hoa','sinh'],
    'D07':['hoa'],'C00':['dia','su'],'D01':[],'X06':['ly','tin'],
    'B03':['sinh'],'C04':['dia'],'D14':['su'],'D15':['dia'],'C03':['su'],
    'X70':['su','gdktpl'],'X35':['su','gdktpl'],'X01':['gdktpl'],
  };
  const tnIds=selTnMons.map(m=>m.id);
  let targetTH='';
  if(n){
    let bestCode='', bestScore=-1;
    n.dh.forEach(d=>{
      const code=d.split(':')[0].trim();
      const needed=TH_MON_MAP2[code]||[];
      // score = số môn khớp - số môn thiếu (ưu tiên khớp nhiều, thiếu ít)
      const matched=needed.filter(m=>tnIds.includes(m)).length;
      const missing=needed.filter(m=>!tnIds.includes(m)).length;
      const score=matched*2-missing;
      if(score>bestScore){bestScore=score;bestCode=code;}
    });
    targetTH=bestCode||n.dh[0].split(':')[0].trim();
  }

  const getMonName=id=>ALL_MONS.find(m=>m.id===id)?.label||id;

  const possibleTH=[ids,ids2].map(k=>TO_HOP_MAP[k]).filter(Boolean);
  const A01_open=selTnMons.some(m=>m.id==='ly');

  const allTH=[...new Set([...possibleTH,...(A01_open?['A01']:[])])];

  const D01_always=true;
  const allCards=[
    {code:'Toán+Văn+'+selTnMons[0].label, realCode: possibleTH[0]||'—', mons:`Toán, Ngữ văn, ${selTnMons[0].label}`},
    {code:'Toán+Văn+'+selTnMons[1].label, realCode: possibleTH[1]||possibleTH[0]||'—', mons:`Toán, Ngữ văn, ${selTnMons[1].label}`},
    {code:'Toán+'+selTnMons[0].label+'+'+selTnMons[1].label, realCode: TO_HOP_MAP[ids]||TO_HOP_MAP[ids2]||'—', mons:`Toán, ${selTnMons[0].label}, ${selTnMons[1].label}`},
    {code:'D01', realCode:'D01', mons:'Toán, Ngữ văn, Tiếng Anh (nếu học Anh văn tốt)'},
  ];

  const cards=CHUNG_TABLE.map(r=>{
    const mon3lower=r.mon3.toLowerCase();
    const tnIds=selTnMons.map(m=>m.id);
    const mons_map={ly:'vật lý',hoa:'hóa học',sinh:'sinh học',tin:'tin học',dia:'địa lý',su:'lịch sử',gdktpl:'gdktpl'};
    const hasMatch=tnIds.some(id=>mons_map[id]&&mon3lower.includes(mons_map[id]));
    const isTarget=r.dh===targetTH;
    if(!hasMatch&&!isTarget) return null;
    return{...r,isTarget,hasMatch};
  }).filter(Boolean);

  if(cards.length===0){
    resEl.innerHTML=`<div class="warn-box" style="margin-top:.75rem">Với 2 môn bạn chọn thi tốt nghiệp, chưa tạo được tổ hợp xét tuyển phổ biến nào. Hãy cân nhắc chọn lại hoặc liên hệ HNA để tư vấn.</div>`;
    return;
  }

  const sorted=cards.sort((a,b)=>b.isTarget-a.isTarget||b.hasMatch-a.hasMatch);

  resEl.innerHTML=`
    <p style="font-size:12px;color:var(--text3);margin-bottom:6px">
      4 môn thi TN của bạn: <strong>Toán, Ngữ văn, ${selTnMons.map(m=>m.label).join(', ')}</strong> → có thể đăng ký các tổ hợp xét tuyển ĐH sau:
    </p>
    <div class="tohop-result-grid">
      ${sorted.map(r=>`
        <div class="tohop-result-card ${r.isTarget?'match-card':''}">
          <span class="trc-badge ${r.isTarget?'badge-target':r.hasMatch?'badge-open':'badge-partial'}">
            ${r.isTarget?'★ Ngành bạn chọn':r.hasMatch?'Mở được':'Tham khảo'}
          </span>
          <div class="trc-code">${r.dh}</div>
          <div class="trc-mons">${r.mon3}</div>
          <div class="trc-nganh">${r.nganh}</div>
        </div>`).join('')}
    </div>
    <p style="font-size:11px;color:var(--text3);margin-top:8px">★ = tổ hợp phù hợp nhất với ngành <strong>${n?.ten||''}</strong> bạn đã chọn</p>`;

  buildFlowSVG();
}

function buildFlowSVG(){
  const wrap=document.getElementById('flow-svg-wrap');
  if(!wrap)return;
  const n=NGANH.find(x=>x.id===selN);
  if(!n||selMons.length<2||selTnMons.length<2){wrap.style.display='none';return;}

  // Tính mainTH thông minh dựa trên môn HS thực sự chọn thi TN
  const tnIds2=selTnMons.map(m=>m.id);
  const TH_MON_SVG={'A00':['ly','hoa'],'A01':['ly'],'B00':['hoa','sinh'],'D07':['hoa'],'C00':['dia','su'],'D01':[],'X06':['ly','tin'],'B03':['sinh'],'C04':['dia'],'D14':['su'],'D15':['dia'],'C03':['su'],'X70':['su','gdktpl'],'X35':['su','gdktpl'],'X01':['gdktpl']};
  let mainTH=n.dh[0].split(':')[0].trim();
  let bestScore2=-99;
  n.dh.forEach(d=>{
    const code=d.split(':')[0].trim();
    const needed=TH_MON_SVG[code]||[];
    const score=needed.filter(m=>tnIds2.includes(m)).length*2 - needed.filter(m=>!tnIds2.includes(m)).length;
    if(score>bestScore2){bestScore2=score;mainTH=code;}
  });
  const monL10=selMons.map(m=>m.label);
  const monTN=selTnMons.map(m=>m.label);
  const monKhong=selMons.filter(m=>!selTnMons.find(t=>t.id===m.id)).map(m=>m.label);

  const NAVY='#142768', AMBER='#FF9900', TEAL='#1D9E75', CORAL='#D85A30', GRAY='#888780';
  const TEAL_L='#E1F5EE', TEAL_S='#0F6E56';
  const AMBER_L='#FAEEDA', AMBER_S='#854F0B';
  const CORAL_L='#FAECE7', CORAL_S='#993C1D';
  const NAVY_L='#EAF0FB', NAVY_S='#0C447C';
  const GRAY_L='#F1EFE8', GRAY_S='#5F5E5A';

  const rowH=38, gap=8;
  const l10H=40+monL10.length*(rowH+gap)+gap;
  const svgH=Math.max(l10H+40, 460);

  const monColor=(label)=>{
    const isTN=monTN.includes(label);
    if(isTN) return {fill:AMBER_L,stroke:AMBER,txt:AMBER_S,bold:true};
    return {fill:GRAY_L,stroke:GRAY,txt:GRAY_S,bold:false};
  };

  const C1x=16,C1w=160, C2x=210,C2w=172, C3x=416,C3w=188;
  const headerH=34, headerY=16;
  const monStartY=headerY+headerH+gap;

  let l10Rows='', tnRows='', linesSVG='';
  const monY={};

  monL10.forEach((label,i)=>{
    const y=monStartY+i*(rowH+gap);
    monY[label]=y;
    const c=monColor(label);
    const fw=c.bold?'500':'400';
    l10Rows+=`
      <rect x="${C1x}" y="${y}" width="${C1w}" height="${rowH}" rx="6"
        fill="${c.fill}" stroke="${c.stroke}" stroke-width="${c.bold?1.5:0.5}" opacity="${c.bold?1:.55}"/>
      <text x="${C1x+C1w/2}" y="${y+rowH/2}" text-anchor="middle" dominant-baseline="central"
        font-size="12" font-weight="${fw}" fill="${c.txt}">${label}</text>`;
  });

  const fixedMons=['Toán','Ngữ văn'];
  const allTN=[...fixedMons,...monTN];
  allTN.forEach((label,i)=>{
    const y=monStartY+i*(rowH+gap);
    const isFixed=fixedMons.includes(label);
    const fill=isFixed?NAVY_L:AMBER_L;
    const stroke=isFixed?NAVY:AMBER;
    const txt=isFixed?NAVY_S:AMBER_S;
    const fw='500';
    tnRows+=`
      <rect x="${C2x}" y="${y}" width="${C2w}" height="${rowH}" rx="6"
        fill="${fill}" stroke="${stroke}" stroke-width="${isFixed?0.5:1.5}"/>
      <text x="${C2x+C2w/2}" y="${y+rowH/2}" text-anchor="middle" dominant-baseline="central"
        font-size="12" font-weight="${fw}" fill="${txt}">${label}${isFixed?' (bắt buộc)':''}</text>`;
  });

  if(monKhong.length>0){
    const y=monStartY+allTN.length*(rowH+gap)+4;
    monKhong.forEach((label,i)=>{
      const ky=y+i*(rowH+gap);
      tnRows+=`
        <rect x="${C2x}" y="${ky}" width="${C2w}" height="${rowH}" rx="6"
          fill="${GRAY_L}" stroke="${GRAY}" stroke-width="0.5" opacity=".4"/>
        <text x="${C2x+C2w/2}" y="${ky+rowH/2}" text-anchor="middle" dominant-baseline="central"
          font-size="11" fill="${GRAY_S}" opacity=".5">${label} — không thi</text>`;
    });
  }

  monTN.forEach(label=>{
    const srcY=monY[label];
    if(srcY===undefined)return;
    const srcMid=srcY+rowH/2;
    const dstIdx=fixedMons.length+monTN.indexOf(label);
    const dstMid=monStartY+dstIdx*(rowH+gap)+rowH/2;
    linesSVG+=`<path d="M${C1x+C1w} ${srcMid} C${C2x-30} ${srcMid} ${C2x-30} ${dstMid} ${C2x} ${dstMid}"
      fill="none" stroke="${AMBER}" stroke-width="1.5" stroke-dasharray="5 3" opacity=".7" marker-end="url(#arr)"/>`;
  });

  const thY=monStartY+2*(rowH+gap);
  const thCode=mainTH;
  const thEntry=n.dh.find(d=>d.split(':')[0].trim()===thCode)||n.dh[0];
  const thMons=thEntry.split(':')[1]?.trim().split('(')[0].trim()||'';
  const nganh=n.ten;

  linesSVG+=`<line x1="${C2x+C2w}" y1="${monStartY+(allTN.length/2)*(rowH+gap)}"
    x2="${C3x}" y2="${thY+40}"
    stroke="${TEAL}" stroke-width="1.5" marker-end="url(#arr)" fill="none"/>`;

  const svgContent=`
<svg width="100%" viewBox="0 0 620 ${svgH}" role="img">
  <title>Luồng tổ hợp môn</title>
  <defs>
    <marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
      <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
    </marker>
  </defs>

  <!-- COL 1 HEADER -->
  <rect x="${C1x}" y="${headerY}" width="${C1w}" height="${headerH}" rx="7"
    fill="${NAVY}" stroke="none"/>
  <text x="${C1x+C1w/2}" y="${headerY+headerH/2}" text-anchor="middle" dominant-baseline="central"
    font-size="12" font-weight="600" fill="white">Lớp 10 (4 môn chọn)</text>

  <!-- COL 2 HEADER -->
  <rect x="${C2x}" y="${headerY}" width="${C2w}" height="${headerH}" rx="7"
    fill="${NAVY}" stroke="none"/>
  <text x="${C2x+C2w/2}" y="${headerY+headerH/2}" text-anchor="middle" dominant-baseline="central"
    font-size="12" font-weight="600" fill="white">4 môn thi tốt nghiệp</text>

  <!-- COL 3 HEADER -->
  <rect x="${C3x}" y="${headerY}" width="${C3w}" height="${headerH}" rx="7"
    fill="${NAVY}" stroke="none"/>
  <text x="${C3x+C3w/2}" y="${headerY+headerH/2}" text-anchor="middle" dominant-baseline="central"
    font-size="12" font-weight="600" fill="white">Tổ hợp → Ngành</text>

  <!-- LINES -->
  ${linesSVG}

  <!-- L10 ROWS -->
  ${l10Rows}

  <!-- TN ROWS -->
  ${tnRows}

  <!-- TH BOX -->
  <rect x="${C3x}" y="${thY}" width="${C3w}" height="60" rx="10"
    fill="${TEAL_L}" stroke="${TEAL}" stroke-width="2"/>
  <text x="${C3x+C3w/2}" y="${thY+20}" text-anchor="middle" dominant-baseline="central"
    font-size="22" font-weight="700" fill="${TEAL_S}">${thCode}</text>
  <text x="${C3x+C3w/2}" y="${thY+44}" text-anchor="middle" dominant-baseline="central"
    font-size="11" fill="${TEAL_S}">${thMons}</text>

  <!-- NGANH BOX -->
  <rect x="${C3x}" y="${thY+76}" width="${C3w}" height="50" rx="8"
    fill="${CORAL_L}" stroke="${CORAL}" stroke-width="1.5"/>
  <line x1="${C3x+C3w/2}" y1="${thY+62}" x2="${C3x+C3w/2}" y2="${thY+74}"
    stroke="${TEAL}" stroke-width="1.5" marker-end="url(#arr)" fill="none"/>
  <text x="${C3x+C3w/2}" y="${thY+96}" text-anchor="middle" dominant-baseline="central"
    font-size="13" font-weight="600" fill="${CORAL_S}">${nganh.length>20?nganh.slice(0,20)+'…':nganh}</text>
  <text x="${C3x+C3w/2}" y="${thY+114}" text-anchor="middle" dominant-baseline="central"
    font-size="10" fill="${CORAL_S}" opacity=".8">${n&&n.truong?n.truong.split(',').slice(0,2).join(',')+('…'):'Liên hệ HNA: 096 937 4411'}</text>

  <!-- NOTE -->
  <rect x="${C1x}" y="${svgH-48}" width="${C3x+C3w-C1x}" height="36" rx="7"
    fill="#FFF4D8" stroke="${AMBER}" stroke-width="0.5"/>
  <text x="${(C1x+C3x+C3w)/2}" y="${svgH-36}" text-anchor="middle" dominant-baseline="central"
    font-size="11" fill="${AMBER_S}">Chọn sai môn lớp 10 → mất tổ hợp ${thCode} → không vào được ${nganh.length>18?nganh.slice(0,18)+'…':nganh}</text>
  <text x="${(C1x+C3x+C3w)/2}" y="${svgH-20}" text-anchor="middle" dominant-baseline="central"
    font-size="10" fill="${AMBER_S}" opacity=".7">Hướng Nghiệp Alpha — 096 937 4411</text>
</svg>`;

  wrap.style.display='block';
  wrap.innerHTML=`<div style="background:var(--bg);border:0.5px solid var(--border);border-radius:var(--r);padding:.75rem;margin-top:.75rem">
    <p style="font-size:12px;color:var(--text2);margin-bottom:.5rem;font-weight:500">Sơ đồ luồng chọn môn của bạn</p>
    ${svgContent}
  </div>`;
}

function checkMatch(){
  const n=NGANH.find(x=>x.id===selN);
  if(!n||selMons.length<2)return;

  const monIds=selMons.map(m=>m.id);
  const monNames=selMons.map(m=>m.label).join(', ');

  const NEED_MAP={
    'B00':['hoa','sinh'],'A00':['ly','hoa'],'A01':['ly'],
    'D07':['hoa'],'C00':['dia','su'],'D01':[],'X06':['ly','tin'],
    'D14':['su'],'D15':['dia'],'C04':['dia'],'B03':['sinh'],
    'V00':['ly'],'H00':['mt'],'C03':['su'],
  };

  const mainTH=n.dh[0].split(':')[0].trim();
  const needed=NEED_MAP[mainTH]||[];
  const matched=needed.filter(m=>monIds.includes(m));
  const missing=needed.filter(m=>!monIds.includes(m));

  let type,icon,title,detail;

  if(needed.length===0){
    type='match-yes';icon='✅';title='Tổ hợp của bạn phù hợp!';
    detail=`Tổ hợp <strong>${monNames}</strong> mở được tổ hợp xét tuyển <strong>${mainTH}</strong> vào ngành <strong>${n.ten}</strong>.<br>Bạn đang đi đúng hướng — tiếp tục học tốt các môn này nhé!`;
  } else if(missing.length===0){
    type='match-yes';icon='✅';title='Tổ hợp của bạn hoàn toàn phù hợp!';
    detail=`Tổ hợp <strong>${monNames}</strong> đã có đủ môn cần thiết cho tổ hợp xét tuyển <strong>${mainTH}</strong>.<br>Ngành <strong>${n.ten}</strong> — bạn đang trên đúng con đường!`;
  } else if(matched.length>0){
    type='match-partial';icon='⚠️';title='Tổ hợp phù hợp một phần';
    detail=`Bạn đã có: <strong>${matched.map(id=>ALL_MONS.find(m=>m.id===id)?.label||id).join(', ')}</strong>.<br>
    Còn thiếu: <strong style="color:#a32d2d">${missing.map(id=>ALL_MONS.find(m=>m.id===id)?.label||id).join(', ')}</strong> để xét tuyển tổ hợp <strong>${mainTH}</strong> vào ngành <strong>${n.ten}</strong>.<br>
    Nếu trường chưa có tổ hợp này, hãy liên hệ HNA để được tư vấn phương án thay thế.`;
  } else {
    type='match-no';icon='❌';title='Tổ hợp chưa phù hợp với ngành bạn chọn';
    detail=`Tổ hợp <strong>${monNames}</strong> chưa đáp ứng yêu cầu xét tuyển vào <strong>${n.ten}</strong> (cần tổ hợp ${mainTH}: ${n.dh[0].split(':')[1]?.trim()}).<br>
    Đừng lo — vẫn còn nhiều phương án. Hãy để HNA tư vấn cụ thể cho bạn!`;
  }

  document.getElementById('match-result').innerHTML=`
    <div class="match-result ${type}">
      <div class="match-icon">${icon}</div>
      <div class="match-title">${title}</div>
      <div class="match-detail">${detail}</div>
    </div>`;

  const sf=document.getElementById('send-form');
  sf.style.display='block';
  const schoolInput=document.getElementById('school-input').value.trim();
  if(schoolInput) document.getElementById('sf-school').value=schoolInput;
  document.getElementById('sf-summary').textContent=
    `Sẽ gửi: Ngành "${n.ten}" | Tổ hợp "${monNames}" | Kết quả: ${title}`;
  sf.scrollIntoView({behavior:'smooth',block:'nearest'});
}

function submitForm(){
  const name=document.getElementById('sf-name').value.trim();
  const phone=document.getElementById('sf-phone').value.trim();
  const school=document.getElementById('sf-school').value.trim();
  const lop=document.getElementById('sf-lop').value;
  const tinh=document.getElementById('sf-tinh').value;
  const status=document.getElementById('send-status');

  if(!name||!phone){
    status.className='send-status send-err';
    status.style.display='block';
    status.textContent='Vui lòng nhập họ tên và số điện thoại để HNA liên hệ hỗ trợ.';
    return;
  }

  const n=NGANH.find(x=>x.id===selN);
  const monNames=selMons.map(m=>m.label).join(', ');

  const entry={
    timestamp:new Date().toLocaleString('vi-VN'),
    name,phone,school,lop,tinh,
    nganh:n?.ten||'',
    tohop_truong:monNames,
    traits:[...selT].join(', '),
  };

  console.log('[HNA Data]',JSON.stringify(entry));

  const GOOGLE_FORM_URL='https://docs.google.com/forms/d/e/REPLACE_WITH_YOUR_FORM_ID/formResponse';
  status.className='send-status send-ok';
  status.style.display='block';
  status.innerHTML=`✅ <strong>Đã ghi nhận thông tin!</strong> HNA sẽ liên hệ <strong>${phone}</strong> trong vòng 24 giờ để tư vấn chi tiết.<br>
    <span style="font-size:11px;color:var(--text3)">Hoặc gọi ngay: <a href="tel:0969374411" style="color:var(--navy)">096 937 4411</a></span>`;
  document.querySelector('#send-form .btn-primary').disabled=true;
  document.querySelector('#send-form .btn-primary').style.opacity='.5';
}

function toggleCtruc(){
  const body=document.getElementById('ctruc-body');
  const btn=document.getElementById('ctruc-toggle-btn');
  const hidden=body.style.display==='none';
  body.style.display=hidden?'block':'none';
  btn.textContent=hidden?'Thu gọn ▲':'Mở rộng ▼';
}

function startTool(){
  document.getElementById('ctruc-body').style.display='none';
  document.getElementById('ctruc-toggle-btn').textContent='Mở rộng ▼';
  [1,2,3,4].forEach(i=>{
    const p=document.getElementById('panel'+i);
    if(p) p.className='panel'+(i===1?' show':'');
    const f=document.getElementById('fs'+i);
    if(f) f.className='flow-step'+(i===1?' active':'');
  });
  document.getElementById('flow-bar').scrollIntoView({behavior:'smooth',block:'start'});
}

buildTraits();
</script>
</body>
</html>
