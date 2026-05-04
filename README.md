# drkellys-leadership-vision
Manager vision
[index.html](https://github.com/user-attachments/files/27378654/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>2029 Vision | Dr. Kelly's Leadership Team</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;1,400&family=Outfit:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --navy: #1E3A52;
    --navy-mid: #2B4B6F;
    --navy-light: #3D6A96;
    --green: #8DC34A;
    --green-dark: #6A9A32;
    --green-glow: rgba(141,195,74,0.15);
    --bg: #0E1E2C;
    --bg2: #142333;
    --text: #E8EDF2;
    --text-dim: rgba(232,237,242,0.55);
    --text-faint: rgba(232,237,242,0.32);
    --border: rgba(255,255,255,0.08);
    --border-green: rgba(141,195,74,0.25);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Outfit', sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    overflow-x: hidden;
  }

  .bg-glow {
    position: fixed; inset: 0; pointer-events: none; z-index: 0;
    background:
      radial-gradient(ellipse at 15% 40%, rgba(43,75,111,0.35) 0%, transparent 55%),
      radial-gradient(ellipse at 85% 15%, rgba(141,195,74,0.08) 0%, transparent 45%),
      radial-gradient(ellipse at 50% 90%, rgba(30,58,82,0.3) 0%, transparent 50%);
  }

  .container {
    position: relative; z-index: 1;
    max-width: 740px; margin: 0 auto; padding: 0 28px 90px;
  }

  header {
    text-align: center;
    padding: 52px 0 44px;
    border-bottom: 0.5px solid var(--border);
    margin-bottom: 52px;
  }

  .logo-wrap {
    margin-bottom: 28px;
  }
  .logo-wrap img {
    height: 90px; width: auto;
    filter: drop-shadow(0 2px 12px rgba(141,195,74,0.2));
  }

  .org-label {
    font-size: 10px; letter-spacing: 4px; text-transform: uppercase;
    color: var(--green); margin-bottom: 6px; font-weight: 500;
  }

  .team-label {
    font-size: 11px; letter-spacing: 3px; text-transform: uppercase;
    color: var(--text-dim); margin-bottom: 20px; font-weight: 400;
  }

  h1 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(34px, 5vw, 52px);
    font-weight: 400;
    line-height: 1.1;
    color: var(--text);
    margin-bottom: 18px;
  }
  h1 em { font-style: italic; color: #A8C8E8; }

  .subtitle {
    font-size: 14px; color: var(--text-dim); line-height: 1.75;
    max-width: 460px; margin: 0 auto; font-weight: 300;
  }

  /* Progress */
  .progress-bar {
    height: 1.5px; background: rgba(255,255,255,0.06);
    border-radius: 1px; margin-bottom: 44px; overflow: hidden;
  }
  .progress-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--navy-light), var(--green));
    transition: width 0.5s cubic-bezier(.4,0,.2,1);
    width: 0%;
  }

  /* Section labels */
  .section-label {
    display: flex; align-items: center; gap: 12px; margin-bottom: 30px;
  }
  .section-icon {
    width: 34px; height: 34px; border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    font-size: 15px; flex-shrink: 0;
  }
  .icon-meta     { background: rgba(141,195,74,0.15); }
  .icon-growth   { background: rgba(61,106,150,0.25); }
  .icon-health   { background: rgba(141,195,74,0.15); }
  .icon-family   { background: rgba(43,75,111,0.35); }
  .icon-finance  { background: rgba(141,195,74,0.15); }
  .icon-career   { background: rgba(61,106,150,0.25); }
  .icon-impact   { background: rgba(43,75,111,0.35); }

  .section-title {
    font-size: 11px; font-weight: 500; letter-spacing: 2.5px;
    text-transform: uppercase;
  }
  .title-meta    { color: var(--green); }
  .title-growth  { color: #7EB8E0; }
  .title-health  { color: #A8D870; }
  .title-family  { color: #7EB8E0; }
  .title-finance { color: var(--green); }
  .title-career  { color: #A8C8E8; }
  .title-impact  { color: #7EB8E0; }

  /* Questions */
  .question-block {
    margin-bottom: 30px;
    animation: fadeUp 0.35s ease both;
  }
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(10px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  label {
    display: block;
    font-size: 15px; font-weight: 500; color: var(--text);
    margin-bottom: 6px; line-height: 1.5;
  }

  .hint {
    font-size: 12px; color: var(--text-faint);
    margin-bottom: 10px; line-height: 1.6; font-style: italic;
  }

  input[type=text], textarea {
    width: 100%;
    background: rgba(255,255,255,0.04);
    border: 0.5px solid rgba(255,255,255,0.1);
    border-radius: 10px;
    color: var(--text);
    font-family: 'Outfit', sans-serif;
    font-size: 14px; font-weight: 300;
    padding: 12px 16px;
    transition: border-color 0.2s, background 0.2s;
    resize: vertical; line-height: 1.6;
  }
  input[type=text]:focus, textarea:focus {
    outline: none;
    border-color: rgba(141,195,74,0.4);
    background: rgba(141,195,74,0.03);
  }
  textarea { min-height: 100px; }

  /* Nav */
  .nav-row {
    display: flex; align-items: center; justify-content: space-between;
    margin-top: 44px; padding-top: 28px;
    border-top: 0.5px solid var(--border);
    gap: 16px;
  }
  .step-indicator {
    font-size: 11px; color: var(--text-faint); letter-spacing: 0.5px;
  }
  .btn-row { display: flex; gap: 12px; }

  .btn {
    font-family: 'Outfit', sans-serif;
    font-size: 14px; font-weight: 500;
    border-radius: 10px; padding: 11px 26px;
    cursor: pointer; transition: all 0.2s; border: none;
  }
  .btn-back {
    background: transparent;
    border: 0.5px solid rgba(255,255,255,0.12);
    color: var(--text-dim);
  }
  .btn-back:hover { border-color: rgba(255,255,255,0.25); color: var(--text); }

  .btn-next {
    background: linear-gradient(135deg, var(--navy), var(--navy-light));
    color: #fff;
    box-shadow: 0 4px 18px rgba(43,75,111,0.5);
  }
  .btn-next:hover { transform: translateY(-1px); box-shadow: 0 6px 22px rgba(43,75,111,0.6); }
  .btn-next:active { transform: translateY(0); }
  .btn-next.final {
    background: linear-gradient(135deg, var(--green-dark), var(--green));
    box-shadow: 0 4px 18px rgba(141,195,74,0.3);
    color: #0E1E2C;
  }
  .btn-next.final:hover { box-shadow: 0 6px 22px rgba(141,195,74,0.4); }

  /* Output */
  #output-section { display: none; }

  .loading-state { text-align: center; padding: 72px 0; }
  .loader {
    display: inline-block; width: 36px; height: 36px;
    border: 1.5px solid rgba(141,195,74,0.2);
    border-top-color: var(--green);
    border-radius: 50%;
    animation: spin 0.75s linear infinite;
    margin-bottom: 20px;
  }
  @keyframes spin { to { transform: rotate(360deg); } }
  .loading-text {
    font-size: 15px; color: var(--text-dim);
    font-family: 'Cormorant Garamond', serif; font-style: italic;
  }

  .result-header { text-align: center; margin-bottom: 32px; }
  .result-header .org-label { margin-bottom: 6px; }
  .result-header h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 26px; font-weight: 400; color: var(--text);
  }

  .vision-wrapper {
    background: rgba(255,255,255,0.02);
    border: 0.5px solid var(--border-green);
    border-radius: 16px;
    padding: 44px;
  }

  .vision-output { font-size: 15px; line-height: 1.88; color: #D8E4EE; font-weight: 300; }
  .vision-output .doc-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 26px; font-weight: 400; color: var(--text);
    border-bottom: 0.5px solid var(--border-green);
    padding-bottom: 18px; margin-bottom: 30px;
  }
  .vision-output .doc-section-head {
    font-family: 'Cormorant Garamond', serif;
    font-size: 19px; font-weight: 400;
    margin: 32px 0 10px;
  }
  .vision-output .doc-section-head.growth  { color: #7EB8E0; }
  .vision-output .doc-section-head.health  { color: #A8D870; }
  .vision-output .doc-section-head.family  { color: #7EB8E0; }
  .vision-output .doc-section-head.finance { color: var(--green); }
  .vision-output .doc-section-head.career  { color: #A8C8E8; }
  .vision-output .doc-section-head.impact  { color: #7EB8E0; }
  .vision-output p { margin-bottom: 14px; }

  .doc-actions { display: flex; gap: 12px; margin-top: 24px; flex-wrap: wrap; }

  .btn-copy, .btn-print, .btn-restart {
    font-family: 'Outfit', sans-serif;
    font-size: 13px; font-weight: 500;
    padding: 10px 20px; border-radius: 8px; cursor: pointer;
    transition: all 0.2s;
  }
  .btn-copy {
    background: rgba(141,195,74,0.12); color: #A8D870;
    border: 0.5px solid rgba(141,195,74,0.25);
  }
  .btn-copy:hover { background: rgba(141,195,74,0.22); }
  .btn-print {
    background: rgba(61,106,150,0.15); color: #A8C8E8;
    border: 0.5px solid rgba(61,106,150,0.3);
  }
  .btn-print:hover { background: rgba(61,106,150,0.25); }
  .btn-restart {
    background: transparent; color: var(--text-faint);
    border: 0.5px solid var(--border);
  }
  .btn-restart:hover { color: var(--text); border-color: rgba(255,255,255,0.22); }

  @media print {
    body { background: #fff; color: #111; }
    .bg-glow, header, .doc-actions, #quiz-section { display: none !important; }
    #output-section { display: block !important; }
    .vision-wrapper { background: none; border: none; padding: 0; }
    .vision-output { color: #111; font-size: 13px; line-height: 1.75; }
    .vision-output .doc-title { color: #111; border-bottom-color: #ccc; }
    .vision-output .doc-section-head { color: #333 !important; }
    .loading-state { display: none; }
  }

  @media (max-width: 600px) {
    .container { padding: 0 16px 60px; }
    header { padding: 36px 0 28px; }
    .vision-wrapper { padding: 24px 18px; }
    .nav-row { flex-direction: column; align-items: flex-end; }
  }
</style>
</head>
<body>
<div class="bg-glow"></div>
<div class="container">

  <header>
    <div class="logo-wrap">
      <img src="data:image/png;base64,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7LP98of44/mio7o/oHooor+vj0gooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAP/S/v4ooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/LP/AIKD/wDI1eHP+vSf/wBDFfnnX6Gf8FB/+Rq8Of8AXpP/AOhivzzr+YeO/wDke4r1X/pMTgrfGwooor5EyCiiigAooooAKKKKACiiigAooooAK9R+CH/JZfCn/YXsv/Rq15dXqPwQ/wCSy+FP+wvZf+jVruyz/fKH+OP5oqO6P6B6KKK/r49IKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/0/7+KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAPyz/wCCg/8AyNXhz/r0n/8AQxX551+hn/BQf/kavDn/AF6T/wDoYr886/mHjv8A5HuK9V/6TE4K3xsKKKK+RMgooooAKKUAk4HU194/B/8AYe8R+LLKPX/iXcvo1rKAyWsag3TKc/e3fLH2wCGPqBXq5TkuMzKr7HB03J9eiXq3ov16FRg5OyPg2iv278O/se/ATw/JHO+kNfyx9Hu5nkB+qAqh/Fa9l0n4Z/DjQZVuNE0DTrSRejw20aMPxC5r7/C+FOPkr168I+l5fojZYd9Wfz22+maldp5tpbySr6ohYfpVN0eNzHICrDgg9RX9JT3+n27eVJNGhHGCwFYuu+EfB/jGBU8SabaanGB8v2iJJgM+m4HH4V6FXwjko3p4u784WX/pT/JlfVvM/nNor9Zfin+wv4L122l1H4YzNo96AWW3lZpLZz6ZOXT6gsB2WvzD8ZeCvE/w/wBfm8M+LrR7O8h6q/Rl7Mp6MpxwRwa/Pc94WzDKZL61D3XtJaxfz6PyaTMZ05R3OWr1H4If8ll8Kf8AYXsv/Rq15dXqPwQ/5LL4U/7C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KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/0v7+KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigArzrXfg/8ACTxQ8sniXwtpGotOCJTdWMMxcHru3oc5969FopqTWzFKKejR8d65/wAE8/2C/EdtNbat8F/BD+fne6aDZRS5JzkSJCrg+4YGvAr7/gi9/wAEwtQZmn+EemruOT5VzeRD8AlwuPwr9QaK3ji68fhqNfNnPPBYeXxU4v5I/Km3/wCCI3/BLe1fzI/hPaE/7eoai4/Jroivbvhz/wAEyf8Agn18KW83wb8H/C4lDrIs17YR6hMjL0KSXYmdMf7LCvuiinLGYiStKpJ/N/5ijgcNF3jSivkv8jM0fRNG8Paemk6BaQ2NrFnZDbxrFGueThVAAya06KK5mzqSCiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAP//T/v4ooooAKKKKACiiv5wvj3/wc7/sNfs8fHDxh8BPGPgzx5d6t4K1m+0O9nsrPT3tpLiwmeCRomk1CNyhZCVLIpI6gHigLH9HtFfy0/8AEWz/AME9v+hE+Iv/AIA6Z/8ALOk/4i2f+Ce3/QifEX/wB0z/AOWdA7M/qXor+Wj/AIi2f+Ce3/QifEX/AMAdM/8AlnXtHwf/AODoz/glz8S9Um03xlceKfh+kYBS417SfOhlJOML/Zk184I7l0Ue9AWZ/RfRXy/+zn+2t+yZ+1xpX9rfs3fEHRPFwVS8lvZXS/bIVBIzLavtnizjjzI1yORxX1BQIKKKKACiiv5v/jv/AMHPP7DP7Pnxv8YfAXxh4M8eXWreCtav9CvZ7Oz097aS40+Z4JGiZ9QRzGWQlSyKSMZAPFAWP6QKK/lo/wCItn/gnt/0InxF/wDAHTP/AJZ0v/EWz/wT2/6ET4i/+AOmf/LOgdmf1LUV/LSP+Dtn/gnr38CfEX/wB0z/AOWde5/Bz/g6C/4JafE+7ls/GOoeJfh9sICP4g0gypKT/dOmSX+0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DtS/+Vtf6FtFAJn+el/xCU/8FDP+h5+Hf/gdqX/yto/4hKf+Chn/AEPPw7/8DtS/+Vtf6FtFA+Zn+el/xCU/8FDP+h5+Hf8A4Hal/wDK2v05/wCCQn/Bv7+17/wT+/be0P8AaX+L/ijwfqmh6ZYajay2+j3V7Lds93A0SFVnsoUwGOWy4OOmelf16UUC5gooooEFfzM/8Fzv+CL37TX/AAU6+NHgn4j/AAL8Q+GNGsvDeiS6bcx69cXcMryvO0oKC3tbhSu045IOe1f0zUUAmfyc/wDBGD/gg5+1l/wTm/bFf9ob40eJvCWraM2g32lCDRLm8lufOuXhZW2z2cCbQIzk789MA1/WNRRQDYUUUUAFFFFABRRRQB+RX7bf/BD7/gnx+3TqV54x+IPhRvDXi29LvL4g8NOtheSyyMWaSdNj29w7Mcs80TyHpuFfze/Hv/g0V+N2jul3+zF8V9F8QRuzGS28S2s2lPGo+6FmtherKT3zHEP6f3b0UDuf5yrf8Gqf/BTZX2jUvA5HqNVucfrZZ/Sve/gn/wAGkH7WXiDXf+Mg/iV4X8L6SFJ3aIl1rF2zj+ExzR2Mag/3hKxH901/ffRQHMz8WP2BP+CDn7Cf7BWq2nxA0jSpvHXji02tFr3iIRztayqysHtLcKIbdgygpIFaZRkCXBOf2noooEFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAf/0f7+KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/9L+/iiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD8lP8AgrT/AMFI/EX7AHw98HeHPg/4bj8X/FH4pawNC8J6VcsUtnud0aNJNhkZlV5oUCK6FmkHzKATXw1e6Z/wc8fDPTZPjVPq/wAL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KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAP/V/v4ooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/1v7+KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/9f+/iiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAP/Z" alt="Dr. Kelly's Surgical Unit">
    </div>
    <div class="org-label">Dr. Kelly's Surgical Unit</div>
    <div class="team-label">Leadership Team · Pre-Work</div>
    <h1>Your <em>Vivid Vision</em><br>for 2029</h1>
    <p class="subtitle">Answer each question as if it's January 2030 and the last three years went exactly as you hoped. Be honest, specific, and unfiltered — this document is for you.</p>
  </header>

  <div id="quiz-section">
    <div class="progress-bar"><div class="progress-fill" id="progress"></div></div>
    <div id="step-container"></div>
    <div class="nav-row">
      <div class="step-indicator" id="step-ind"></div>
      <div class="btn-row">
        <button class="btn btn-back" id="btn-back" onclick="goBack()">← Back</button>
        <button class="btn btn-next" id="btn-next" onclick="goNext()">Continue →</button>
      </div>
    </div>
  </div>

  <div id="output-section">
    <div id="loading-state" class="loading-state">
      <div class="loader"></div>
      <div class="loading-text" id="loading-msg">Bringing your 2029 into focus...</div>
    </div>
    <div id="vision-result" style="display:none">
      <div class="result-header">
        <div class="org-label">Your document is ready</div>
        <h2>Your Vivid Vision · 2029</h2>
      </div>
      <div class="vision-wrapper">
        <div id="vision-content" class="vision-output"></div>
      </div>
      <div class="doc-actions">
        <button class="btn-copy" onclick="copyDoc()">Copy text</button>
        <button class="btn-print" onclick="window.print()">Print / Save PDF</button>
        <button class="btn-restart" onclick="restart()">Start over</button>
      </div>
    </div>
  </div>

</div>

<script>
const WORKER_URL = 'https://2026-retreat-vision.dougyfreshaz.workers.dev';

const steps = [
  {
    id: 'meta', iconClass: 'icon-meta', titleClass: 'title-meta', icon: '✦', label: 'About You',
    questions: [
      { id: 'name',     type: 'text',     label: "What's your name?",                                                   placeholder: 'Your full name',                                        hint: '' },
      { id: 'role',     type: 'text',     label: "What's your current role and company?",                               placeholder: 'e.g. Operations Manager, Dr. Kelly\'s Surgical Unit',   hint: '' },
      { id: 'function', type: 'text',     label: "What field or function are you in?",                                  placeholder: 'e.g. operations, sales, finance, HR, marketing',        hint: '' },
    ]
  },
  {
    id: 'growth', iconClass: 'icon-growth', titleClass: 'title-growth', icon: '◈', label: 'Personal Growth & Legacy',
    questions: [
      { id: 'g_become',       type: 'textarea', label: "Who have you become in the last 3+ years? What beliefs or habits have you shed or adopted?",                  placeholder: 'I used to believe... now I know... I\'ve let go of... I\'ve built the habit of...', hint: 'Think about identity shifts — the inner changes, not just the external ones.' },
      { id: 'g_adventures',   type: 'textarea', label: "What experiences, adventures, or bucket-list moments have you had?",                                         placeholder: 'I finally... I traveled to... I experienced... one unforgettable moment was...', hint: '' },
      { id: 'g_hobbies',      type: 'textarea', label: "What hobbies or activities bring you joy and recharge you?",                                                 placeholder: 'I regularly spend time on... I\'ve discovered... it brings me joy to...', hint: '' },
      { id: 'g_contribution', type: 'textarea', label: "How are you contributing beyond your work-life? What causes, community, or legacy matters to you?",          placeholder: 'I give back by... I\'m involved in... the legacy I\'m building is...', hint: '' },
      { id: 'g_identity',     type: 'textarea', label: "How do you describe yourself in 2029 — professionally and personally? Who have you become?",                 placeholder: 'I am someone who... people see me as... the word I\'d use to describe myself is...', hint: 'The most important question. Take your time.' },
      { id: 'g_goals',        type: 'textarea', label: "What goals are still on your greater list to be done?",                                                      placeholder: 'I still want to... on my list is... I haven\'t yet but plan to...', hint: 'The things still calling you forward.' },
    ]
  },
  {
    id: 'health', iconClass: 'icon-health', titleClass: 'title-health', icon: '◎', label: 'Health & Wellbeing',
    questions: [
      { id: 'h_physical', type: 'textarea', label: "How do you feel physically in 2029? Describe your health, fitness, energy, and your daily and weekly routine.", placeholder: 'I wake up feeling... my fitness routine includes... my energy throughout the day is... I sleep...', hint: 'Physical vitality underpins everything else.' },
      { id: 'h_mental',   type: 'textarea', label: "How do you show up mentally and emotionally? What practices keep you grounded and performing at your best?",    placeholder: 'My mindset is... I manage stress by... each morning I... I\'ve let go of the belief that...', hint: '' },
      { id: 'h_balance',  type: 'textarea', label: "What does rest, recovery, and balance look like in your life?",                                                placeholder: 'I protect time for... I disconnect from work by... my recovery practices include... I no longer...', hint: '' },
    ]
  },
  {
    id: 'family', iconClass: 'icon-family', titleClass: 'title-family', icon: '♡', label: 'Family & Relationships',
    questions: [
      { id: 'fam_home',        type: 'textarea', label: "What does your home life feel like in 2029? Where do you live and how do you spend your personal time?",      placeholder: 'We live in... our home feels... on evenings and weekends I...', hint: '' },
      { id: 'fam_relations',   type: 'textarea', label: "Describe your key relationships — partner, children, parents, close friends.",                               placeholder: 'My relationship with my partner is... my kids are... my friendships are...', hint: 'Quality of connection, not just the facts.' },
      { id: 'fam_traditions',  type: 'textarea', label: "What rituals, traditions, or experiences do you share with the people you love?",                            placeholder: 'Every year we... on weekends we... we have a tradition of...', hint: '' },
      { id: 'fam_role',        type: 'textarea', label: "How do the people closest to you describe you as a partner, parent, or friend?",                            placeholder: 'They would say I\'m... I show up for them by... they count on me to...', hint: '' },
      { id: 'fam_connections', type: 'textarea', label: "What connections are you still trying to make?",                                                            placeholder: 'I want to deepen my relationship with... I\'m still working toward connecting with... I hope to meet...', hint: 'Relationships still on your horizon.' },
    ]
  },
  {
    id: 'finance', iconClass: 'icon-finance', titleClass: 'title-finance', icon: '◉', label: 'Personal Finances',
    questions: [
      { id: 'fin_position', type: 'textarea', label: "It's the end of 2029. How much have you saved and what does your financial position look like? Equities, rental homes, growing a business, etc?", placeholder: 'I have $X saved... my investments include... my net worth is approximately... I own...', hint: 'Be as specific as you\'re comfortable with.' },
      { id: 'fin_habits',   type: 'textarea', label: "What financial habits or disciplines have you built in the last 3 years? Describe the system and outcome.",                                      placeholder: 'Every month I... I automated... I no longer spend on... the result has been...', hint: '' },
      { id: 'fin_feeling',  type: 'textarea', label: "Describe your relationship with money and how your current financial position makes you feel.",                                                  placeholder: 'I feel financially... money no longer causes me to... I am confident that... the word I\'d use is...', hint: 'Financial peace of mind is as important as the numbers.' },
    ]
  },
  {
    id: 'career', iconClass: 'icon-career', titleClass: 'title-career', icon: '★', label: 'Career Growth & Leadership',
    questions: [
      { id: 'c_role',        type: 'textarea', label: "It's the end of 2029. What is your role and title, and how has your career advanced in the last 3 years?",                                         placeholder: 'I am now... I\'ve been promoted to... my responsibilities include... my career has moved from...', hint: '' },
      { id: 'c_leader',      type: 'textarea', label: "What kind of leader have you become? How do the people you lead describe you?",                                                                    placeholder: 'I lead by... people say I\'m... the team describes me as... I\'m known for...', hint: '' },
      { id: 'c_skills',      type: 'textarea', label: "What new skills, capabilities, or areas of expertise have you developed? What learning and training have you attended, if any?",                  placeholder: 'I\'ve developed... I completed training in... I\'ve become known for... I attended...', hint: '' },
      { id: 'c_achievement', type: 'textarea', label: "What is the single biggest professional achievement you've unlocked by 2029? Any other recognition or accolades received?",                        placeholder: 'My biggest achievement was... I was recognized for... I received... I\'m proud of...', hint: '' },
    ]
  },
  {
    id: 'impact', iconClass: 'icon-impact', titleClass: 'title-impact', icon: '⬡', label: 'Impact & Influence',
    questions: [
      { id: 'i_reputation', type: 'textarea', label: "What does your reputation look like and what are people saying about you?",                                                        placeholder: 'People know me as... my colleagues say... my reputation is built on... I\'m seen as someone who...', hint: '' },
      { id: 'i_growth',     type: 'textarea', label: "How are you contributing to the growth and success of the people around you — your team, peers, or direct reports?",               placeholder: 'I invest in my team by... I\'ve helped... people grow under my leadership because... I mentor...', hint: '' },
      { id: 'i_day',        type: 'textarea', label: "What does your day look like? How do you spend your time and energy at work?",                                                     placeholder: 'I spend my mornings on... my best work happens when... I delegate... I focus my energy on...', hint: '' },
    ]
  },
];

const answers = {};
let currentStep = 0;
const totalSteps = steps.length;

const loadingMessages = [
  'Bringing your 2029 into focus...',
  'Weaving your story together...',
  'Crafting your vision document...',
  'Almost there — this is going to be powerful...',
  'Painting the details of your future...',
];

function renderStep() {
  const step = steps[currentStep];
  let html = `<div class="section-label">
    <div class="section-icon ${step.iconClass}">${step.icon}</div>
    <span class="section-title ${step.titleClass}">${step.label}</span>
  </div>`;

  step.questions.forEach((q, i) => {
    const val = answers[q.id] || '';
    html += `<div class="question-block" style="animation-delay:${i * 70}ms">
      <label for="${q.id}">${q.label}</label>
      ${q.hint ? `<div class="hint">${q.hint}</div>` : ''}
      ${q.type === 'textarea'
        ? `<textarea id="${q.id}" placeholder="${q.placeholder}" rows="4">${val}</textarea>`
        : `<input type="text" id="${q.id}" placeholder="${q.placeholder}" value="${val}">`
      }
    </div>`;
  });

  document.getElementById('step-container').innerHTML = html;
  const pct = Math.round((currentStep / totalSteps) * 100);
  document.getElementById('progress').style.width = pct + '%';
  document.getElementById('step-ind').textContent = `Step ${currentStep + 1} of ${totalSteps}`;
  document.getElementById('btn-back').style.visibility = currentStep === 0 ? 'hidden' : 'visible';

  const isLast = currentStep === totalSteps - 1;
  const btn = document.getElementById('btn-next');
  btn.textContent = isLast ? 'Generate My Vision →' : 'Continue →';
  btn.className = 'btn btn-next' + (isLast ? ' final' : '');
}

function saveCurrentAnswers() {
  steps[currentStep].questions.forEach(q => {
    const el = document.getElementById(q.id);
    if (el) answers[q.id] = el.value.trim();
  });
}

function goNext() {
  saveCurrentAnswers();
  if (currentStep < totalSteps - 1) {
    currentStep++;
    renderStep();
    window.scrollTo({ top: 0, behavior: 'smooth' });
  } else {
    generateVision();
  }
}

function goBack() {
  saveCurrentAnswers();
  if (currentStep > 0) {
    currentStep--;
    renderStep();
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
}

function buildPrompt() {
  const a = answers;
  return `Please write a vivid vision document for ${a.name || 'this person'}.

ABOUT THEM:
- Name: ${a.name}
- Current role & company: ${a.role}
- Function/field: ${a.function}

PERSONAL GROWTH & LEGACY:
- Who they've become, beliefs/habits shed or adopted: ${a.g_become}
- Adventures & bucket-list moments: ${a.g_adventures}
- Hobbies & joyful activities: ${a.g_hobbies}
- Contribution beyond work: ${a.g_contribution}
- How they describe themselves in 2029: ${a.g_identity}
- Goals still on the greater list: ${a.g_goals}

HEALTH & WELLBEING:
- Physical health, fitness, energy & routine: ${a.h_physical}
- Mental & emotional state & practices: ${a.h_mental}
- Rest, recovery & balance: ${a.h_balance}

FAMILY & RELATIONSHIPS:
- Home life & personal time: ${a.fam_home}
- Key relationships: ${a.fam_relations}
- Rituals & traditions: ${a.fam_traditions}
- How loved ones describe them: ${a.fam_role}
- Connections still to make: ${a.fam_connections}

PERSONAL FINANCES:
- Financial position & investments: ${a.fin_position}
- Financial habits & systems: ${a.fin_habits}
- Relationship with money: ${a.fin_feeling}

CAREER GROWTH & LEADERSHIP:
- Role & career advancement: ${a.c_role}
- Leadership style & how team describes them: ${a.c_leader}
- Skills, training & expertise developed: ${a.c_skills}
- Biggest achievement & accolades: ${a.c_achievement}

IMPACT & INFLUENCE:
- Reputation & what people say: ${a.i_reputation}
- Contributing to others' growth: ${a.i_growth}
- How they spend their day at work: ${a.i_day}

Write their vivid vision document now. Use FIRST PERSON, present tense, as if it is already January 2030. Structure it with 6 sections: Personal Growth & Legacy, Health & Wellbeing, Family & Relationships, Personal Finances, Career Growth & Leadership, and Impact & Influence. Write in rich evocative prose — no bullet points. Be specific, personal, and inspiring. Approximately 650-750 words. Start with a compelling opening paragraph. End with a stirring closing paragraph. Even if some answers are brief, use what is provided and always produce the full document.`;
}

function generateVision() {
  document.getElementById('quiz-section').style.display = 'none';
  document.getElementById('output-section').style.display = 'block';
  document.getElementById('loading-state').style.display = 'block';
  document.getElementById('vision-result').style.display = 'none';
  window.scrollTo({ top: 0, behavior: 'smooth' });

  let msgIdx = 0;
  const interval = setInterval(() => {
    msgIdx = (msgIdx + 1) % loadingMessages.length;
    const msgEl = document.getElementById('loading-msg');
    if (msgEl) msgEl.textContent = loadingMessages[msgIdx];
  }, 2500);

  fetch(WORKER_URL, {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ prompt: buildPrompt() })
  })
  .then(r => r.json())
  .then(data => {
    clearInterval(interval);
    const text = data.content && data.content[0] && data.content[0].text;
    if (!text) throw new Error('No content returned');
    document.getElementById('loading-state').style.display = 'none';
    document.getElementById('vision-result').style.display = 'block';
    document.getElementById('progress').style.width = '100%';
    renderVision(text);
  })
  .catch(err => {
    clearInterval(interval);
    document.getElementById('loading-state').innerHTML = `
      <div style="text-align:center;padding:40px 0;">
        <div style="font-size:28px;margin-bottom:16px;">⚠️</div>
        <p style="color:rgba(232,237,242,0.7);font-size:15px;line-height:1.7;margin-bottom:8px;">Something went wrong generating your vision.</p>
        <p style="color:rgba(232,237,242,0.4);font-size:13px;margin-bottom:28px;">Your answers have been saved. You can try again or go back and edit.</p>
        <div style="display:flex;gap:12px;justify-content:center;flex-wrap:wrap;">
          <button onclick="retryGeneration()" style="background:linear-gradient(135deg,#6A9A32,#8DC34A);color:#0E1E2C;border:none;padding:12px 24px;border-radius:10px;cursor:pointer;font-family:inherit;font-size:14px;font-weight:500;">Try Again</button>
          <button onclick="goBackToForm()" style="background:transparent;border:0.5px solid rgba(255,255,255,0.2);color:#E8EDF2;padding:12px 24px;border-radius:10px;cursor:pointer;font-family:inherit;font-size:14px;">← Edit My Answers</button>
        </div>
      </div>`;
  });
}

function retryGeneration() {
  document.getElementById('loading-state').innerHTML = `
    <div class="loader"></div>
    <div class="loading-text" id="loading-msg">Trying again — hang tight...</div>`;
  generateVision();
}

function goBackToForm() {
  document.getElementById('output-section').style.display = 'none';
  document.getElementById('quiz-section').style.display = 'block';
  currentStep = totalSteps - 1;
  renderStep();
  window.scrollTo({ top: 0, behavior: 'smooth' });
}

function renderVision(markdown) {
  let html = markdown
    .replace(/^# (.+)$/gm, '<div class="doc-title">$1</div>')
    .replace(/^## (.+)$/gm, (_, t) => {
      const tl = t.toLowerCase();
      let cls = 'career';
      if (tl.includes('growth') || tl.includes('legacy') || tl.includes('personal')) cls = 'growth';
      else if (tl.includes('health') || tl.includes('wellbeing')) cls = 'health';
      else if (tl.includes('family') || tl.includes('relation')) cls = 'family';
      else if (tl.includes('financ')) cls = 'finance';
      else if (tl.includes('impact') || tl.includes('influence')) cls = 'impact';
      return `<div class="doc-section-head ${cls}">${t}</div>`;
    })
    .replace(/\*\*(.+?)\*\*/g, '<strong>$1</strong>')
    .replace(/\n\n+/g, '</p><p>')
    .replace(/\n/g, ' ');
  document.getElementById('vision-content').innerHTML = '<p>' + html + '</p>';
}

function copyDoc() {
  const text = document.getElementById('vision-content').innerText;
  navigator.clipboard.writeText(text).then(() => {
    const btn = document.querySelector('.btn-copy');
    const orig = btn.textContent;
    btn.textContent = 'Copied!';
    setTimeout(() => btn.textContent = orig, 2200);
  });
}

function restart() {
  if (!confirm('This will clear all your answers and start over. Are you sure?')) return;
  currentStep = 0;
  Object.keys(answers).forEach(k => delete answers[k]);
  document.getElementById('output-section').style.display = 'none';
  document.getElementById('quiz-section').style.display = 'block';
  renderStep();
  window.scrollTo({ top: 0, behavior: 'smooth' });
}

renderStep();
</script>
</body>
</html>
