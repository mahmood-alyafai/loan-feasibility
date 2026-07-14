<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>دراسة جدوى القروض - بنك التنمية العماني</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;500;600;700&display=swap');
  :root {
    --navy: #1a3a5c;
    --navy-light: #2a4a6c;
    --gold: #c9a84c;
    --gold-light: #e8d5a3;
    --bg: #f5f7fa;
    --white: #ffffff;
    --text: #333333;
    --text-light: #666666;
    --border: #d0d5dd;
    --danger: #dc3545;
    --success: #28a745;
    --warning: #f0ad4e;
    --radius: 8px;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: 'Noto Naskh Arabic', 'Segoe UI', Tahoma, sans-serif; background: var(--bg); color: var(--text); line-height: 1.6; }
  .header { background: var(--navy); color: var(--white); padding: 12px 24px; display: flex; align-items: center; justify-content: space-between; border-bottom: 4px solid var(--gold); }
  .header-left { display: flex; align-items: center; gap: 16px; }
  .header-logo { height: 60px; width: auto; }
  .header-title { font-size: 18px; font-weight: 700; }
  .header-subtitle { font-size: 13px; color: var(--gold-light); }
  .header-right { text-align: left; }
  .header-date { font-size: 13px; color: var(--gold-light); }
  .nav { background: var(--white); border-bottom: 1px solid var(--border); padding: 0 24px; display: flex; gap: 4px; overflow-x: auto; position: sticky; top: 0; z-index: 100; }
  .nav-btn { padding: 12px 20px; border: none; background: transparent; color: var(--text-light); font-family: inherit; font-size: 14px; font-weight: 600; cursor: pointer; border-bottom: 3px solid transparent; white-space: nowrap; transition: all 0.2s; }
  .nav-btn:hover { color: var(--navy); background: #f0f4f8; }
  .nav-btn.active { color: var(--navy); border-bottom-color: var(--gold); }
  .container { max-width: 1200px; margin: 0 auto; padding: 24px; }
  .section { display: none; animation: fadeIn 0.3s ease; }
  .section.active { display: block; }
  @keyframes fadeIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: translateY(0); } }
  .card { background: var(--white); border: 1px solid var(--border); border-radius: var(--radius); padding: 20px; margin-bottom: 20px; }
  .card-title { font-size: 16px; font-weight: 700; color: var(--navy); margin-bottom: 16px; padding-bottom: 8px; border-bottom: 2px solid var(--gold); display: flex; align-items: center; gap: 8px; }
  .card-title .num { background: var(--navy); color: var(--gold); width: 28px; height: 28px; border-radius: 50%; display: inline-flex; align-items: center; justify-content: center; font-size: 13px; }
  .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
  .grid-3 { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 16px; }
  .grid-4 { display: grid; grid-template-columns: 1fr 1fr 1fr 1fr; gap: 16px; }
  @media (max-width: 768px) { .grid-2, .grid-3, .grid-4 { grid-template-columns: 1fr; } }
  .field { margin-bottom: 14px; }
  .field label { display: block; font-size: 13px; font-weight: 600; color: var(--navy); margin-bottom: 4px; }
  .field input, .field select, .field textarea { width: 100%; padding: 10px 12px; border: 1px solid var(--border); border-radius: var(--radius); font-family: inherit; font-size: 14px; background: var(--white); color: var(--text); outline: none; transition: border 0.2s; }
  .field input:focus, .field select:focus, .field textarea:focus { border-color: var(--navy); box-shadow: 0 0 0 3px rgba(26,58,92,0.1); }
  .field input[type="number"] { text-align: left; direction: ltr; }
  .field textarea { resize: vertical; min-height: 80px; }
  .file-upload { border: 2px dashed var(--border); border-radius: var(--radius); padding: 20px; text-align: center; cursor: pointer; transition: all 0.2s; background: #fafbfc; }
  .file-upload:hover { border-color: var(--navy); background: #f0f4f8; }
  .file-upload input { display: none; }
  .file-upload-icon { font-size: 32px; margin-bottom: 8px; }
  .file-upload-text { font-size: 13px; color: var(--text-light); }
  .file-upload-name { font-size: 12px; color: var(--success); margin-top: 8px; font-weight: 600; }
  .data-table { width: 100%; border-collapse: collapse; font-size: 13px; margin-bottom: 16px; }
  .data-table th, .data-table td { padding: 10px 12px; border: 1px solid var(--border); text-align: right; }
  .data-table th { background: var(--navy); color: var(--white); font-weight: 600; }
  .data-table tr:nth-child(even) { background: #f8f9fa; }
  .data-table tr:hover { background: #f0f4f8; }
  .data-table td input { width: 100%; border: none; background: transparent; font-family: inherit; font-size: 13px; padding: 4px; text-align: left; direction: ltr; }
  .data-table td input:focus { outline: 1px solid var(--navy); border-radius: 4px; }
  .btn { display: inline-flex; align-items: center; gap: 6px; padding: 10px 20px; border: none; border-radius: var(--radius); font-family: inherit; font-size: 14px; font-weight: 600; cursor: pointer; transition: all 0.2s; }
  .btn-primary { background: var(--navy); color: var(--white); }
  .btn-primary:hover { background: var(--navy-light); }
  .btn-gold { background: var(--gold); color: var(--navy); }
  .btn-gold:hover { background: var(--gold-light); }
  .btn-outline { background: transparent; color: var(--navy); border: 1px solid var(--navy); }
  .btn-outline:hover { background: var(--navy); color: var(--white); }
  .btn-success { background: var(--success); color: white; }
  .btn-group { display: flex; gap: 8px; flex-wrap: wrap; margin: 16px 0; }
  .report-preview { background: var(--white); border: 1px solid var(--border); border-radius: var(--radius); padding: 40px; margin-top: 20px; }
  .report-header { text-align: center; border-bottom: 3px double var(--navy); padding-bottom: 20px; margin-bottom: 30px; }
  .report-header img { height: 80px; margin-bottom: 12px; }
  .report-header h1 { font-size: 20px; color: var(--navy); margin-bottom: 8px; }
  .report-header h2 { font-size: 16px; color: var(--text-light); font-weight: 400; }
  .report-section { margin-bottom: 24px; }
  .report-section h3 { font-size: 15px; color: var(--navy); border-bottom: 2px solid var(--gold); padding-bottom: 6px; margin-bottom: 12px; }
  .report-section p { font-size: 13px; margin-bottom: 8px; text-align: justify; }
  .report-section table { width: 100%; border-collapse: collapse; font-size: 12px; margin: 8px 0; }
  .report-section th, .report-section td { border: 1px solid #999; padding: 6px 8px; text-align: right; }
  .report-section th { background: #e8e8e8; font-weight: 600; }
  .score-box { display: flex; align-items: center; gap: 20px; padding: 20px; background: linear-gradient(135deg, var(--navy) 0%, var(--navy-light) 100%); color: white; border-radius: var(--radius); margin-bottom: 20px; }
  .score-circle { width: 100px; height: 100px; border-radius: 50%; border: 4px solid var(--gold); display: flex; align-items: center; justify-content: center; flex-direction: column; flex-shrink: 0; }
  .score-value { font-size: 32px; font-weight: 700; color: var(--gold); }
  .score-label { font-size: 11px; }
  .score-details { flex: 1; }
  .score-details h3 { font-size: 16px; margin-bottom: 8px; color: var(--gold-light); }
  .score-details p { font-size: 13px; opacity: 0.9; }
  .rec-box { padding: 16px; border-radius: var(--radius); margin-bottom: 12px; border-right: 4px solid; }
  .rec-approve { background: #d4edda; border-color: var(--success); }
  .rec-conditional { background: #fff3cd; border-color: var(--warning); }
  .rec-reject { background: #f8d7da; border-color: var(--danger); }
  .rec-title { font-weight: 700; font-size: 15px; margin-bottom: 6px; }
  .rec-text { font-size: 13px; color: var(--text); }
  .swot-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
  .swot-box { padding: 14px; border-radius: var(--radius); }
  .swot-s { background: #d4edda; border-top: 4px solid var(--success); }
  .swot-w { background: #f8d7da; border-top: 4px solid var(--danger); }
  .swot-o { background: #d1ecf1; border-top: 4px solid #17a2b8; }
  .swot-t { background: #fff3cd; border-top: 4px solid var(--warning); }
  .swot-title { font-weight: 700; font-size: 14px; margin-bottom: 8px; }
  .sub-tabs { display: flex; gap: 8px; margin-bottom: 16px; border-bottom: 1px solid var(--border); }
  .sub-tab { padding: 8px 16px; border: none; background: transparent; font-family: inherit; font-size: 13px; font-weight: 600; color: var(--text-light); cursor: pointer; border-bottom: 2px solid transparent; }
  .sub-tab.active { color: var(--navy); border-bottom-color: var(--gold); }
  .metric-card { border: 1px solid var(--border); border-radius: 10px; padding: 14px; text-align: center; margin-bottom: 12px; }
  .metric-value { font-size: 24px; font-weight: 700; font-variant-numeric: tabular-nums; margin: 4px 0; }
  .metric-label { font-size: 12px; color: var(--text-light); }
  .hidden { display: none; }
  @media print {
    .nav, .btn-group, .file-upload { display: none !important; }
    .section { display: block !important; }
    .report-preview { border: none; padding: 0; }
    body { background: white; }
    .card { break-inside: avoid; }
  }
</style>
</head>
<body>

<div class="header">
  <div class="header-left">
    <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMgAAADICAYAAACtWK6eAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAACi6SURBVHgB7Z0JfFTV1cefuZNJyEIWQkLYSQIJhD0sYVdE3EBxQcW6oLZVq9VWq1Vr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr1VZr
