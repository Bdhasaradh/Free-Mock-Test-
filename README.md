<!DOCTYPE html>
<html lang="te">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- ================= ADVANCED BACKGROUND SEO PACKAGE ================= -->
    <title id="seo-title">Online Mock Test & Competitive Exam Assessment Portal | SSC, RRB, APPSC, TSPSC</title>
    <meta name="description" id="seo-desc" content="Attempt free timed online mock tests in Telugu and English with negative marking (+1 / -0.5), instant diagnostic scorecards, and downloadable PDF answer keys.">
    <meta name="keywords" content="Online Mock Test, Telugu Mock Test, SSC CGL, RRB NTPC, APPSC, TSPSC, Group 1, Group 2, Police Constable, Current Affairs Quiz, Free Practice Test, General Studies">
    <meta name="robots" content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1">
    <meta name="googlebot" content="index, follow">
    <meta name="author" content="Smart Exam Assessment Portal">
    <link rel="canonical" id="seo-canonical" href="">

    <!-- Open Graph / Social Media SEO -->
    <meta property="og:type" content="website">
    <meta property="og:site_name" content="Online Competitive Exam Portal">
    <meta property="og:title" id="og-title" content="Online Mock Test & Competitive Exam Assessment Portal">
    <meta property="og:description" id="og-desc" content="Practice high-yield bilingual mock tests with real-time analytics and downloadable verified PDF solutions.">

    <!-- Dynamic JSON-LD Structured Data for Google Search (Invisible to Users) -->
    <script type="application/ld+json" id="dynamic-seo-schema">
    {
      "@context": "https://schema.org",
      "@type": "Quiz",
      "name": "Competitive Exam Online Mock Test",
      "inLanguage": ["te", "en"],
      "isAccessibleForFree": true
    }
    </script>

    <!-- Google Fonts: Noto Sans Telugu & Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800;900&family=Noto+Sans+Telugu:wght@400;600;700;800&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg-main: #f8fafc;
            --panel-bg: #ffffff;
            --text-dark: #0f172a;
            --text-muted: #64748b;
            --primary-blue: #2563eb;
            --primary-dark: #1d4ed8;
            --success-green: #16a34a;
            --danger-red: #dc2626;
            --warning-amber: #d97706;
            --border-color: #e2e8f0;
            --admin-dark: #0f172a;
        }

        * { 
            box-sizing: border-box; 
            margin: 0; 
            padding: 0; 
            font-family: 'Noto Sans Telugu', 'Inter', 'Segoe UI', Arial, sans-serif; 
        }
        body { background-color: var(--bg-main); color: var(--text-dark); min-height: 100vh; display: flex; flex-direction: column; }

        /* Top Navbar */
        .top-navbar {
            background: var(--admin-dark);
            color: white;
            padding: 0.85rem 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            z-index: 50;
        }
        .portal-brand { font-weight: 800; font-size: 1.1rem; letter-spacing: 0.02em; display: flex; align-items: center; gap: 0.6rem; flex-wrap: wrap; }
        
        .admin-trigger-btn {
            background: #334155;
            color: #f8fafc;
            border: 1px solid #475569;
            padding: 0.45rem 1rem;
            border-radius: 0.5rem;
            cursor: pointer;
            font-weight: 700;
            font-size: 0.85rem;
            transition: all 0.2s ease;
        }
        .admin-trigger-btn:hover { background: var(--primary-blue); border-color: var(--primary-blue); }

        .live-badge {
            display: inline-flex;
            align-items: center;
            gap: 0.4rem;
            background: #ecfdf5;
            color: var(--success-green);
            padding: 0.3rem 0.65rem;
            border-radius: 9999px;
            font-size: 0.75rem;
            font-weight: 700;
            border: 1px solid #a7f3d0;
        }
        .live-dot { width: 8px; height: 8px; background: var(--success-green); border-radius: 50%; animation: pulse 1.2s infinite; }
        @keyframes pulse { 0%, 100% { opacity: 1; } 50% { opacity: 0.3; } }

        /* Waiting Screen */
        .waiting-screen {
            flex: 1;
            display: none;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 2rem;
            text-align: center;
        }
        .waiting-card {
            background: var(--panel-bg);
            max-width: 520px;
            width: 100%;
            padding: 2.5rem 2rem;
            border-radius: 1.25rem;
            box-shadow: 0 10px 25px -5px rgba(0,0,0,0.05);
            border: 1px solid var(--border-color);
        }
        .waiting-pulse {
            width: 56px;
            height: 56px;
            border: 4px solid #dbeafe;
            border-top-color: var(--primary-blue);
            border-radius: 50%;
            animation: spin 1s linear infinite;
            margin: 0 auto 1.5rem;
        }

        /* App Container */
        .app-container {
            display: flex;
            flex-direction: row;
            align-items: flex-start;
            justify-content: space-between;
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 1.25rem;
            gap: 1.25rem;
        }
        main {
            flex: 1;
            display: flex;
            flex-direction: column;
            background: var(--panel-bg);
            min-width: 0;
            border-radius: 1rem;
            border: 1px solid var(--border-color);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.05);
            overflow: hidden;
        }
        
        header.exam-header {
            background: var(--panel-bg);
            padding: 1rem 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid var(--border-color);
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .quiz-arena { width: 100%; padding: 1.5rem; display: block; }
        .question-card { background: var(--panel-bg); width: 100%; padding: 0.25rem; }

        .card-footer-nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 1.5rem;
            padding-top: 1.25rem;
            border-top: 1px solid var(--border-color);
            gap: 0.75rem;
            flex-wrap: wrap;
        }
        .btn-outline {
            padding: 0.65rem 1.2rem;
            background: #ffffff;
            color: var(--text-dark);
            border: 1.5px solid var(--border-color);
            border-radius: 0.6rem;
            font-weight: 700;
            font-size: 0.9rem;
            cursor: pointer;
            transition: all 0.2s;
        }
        .btn-outline:hover { background: #f1f5f9; border-color: #cbd5e1; }
        .btn-next-q {
            padding: 0.65rem 1.4rem;
            background: var(--primary-blue);
            color: white;
            border: none;
            border-radius: 0.6rem;
            font-weight: 700;
            font-size: 0.9rem;
            cursor: pointer;
            transition: background 0.2s;
        }
        .btn-next-q:hover { background: var(--primary-dark); }

        /* Sidebar & Navigator */
        aside {
            width: 300px;
            flex-shrink: 0;
            background: var(--panel-bg);
            border: 1px solid var(--border-color);
            border-radius: 1rem;
            display: flex;
            flex-direction: column;
            padding: 1.25rem;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.05);
            position: sticky;
            top: 1rem;
        }

        .grid-title {
            font-size: 0.85rem;
            font-weight: 700;
            color: var(--text-muted);
            text-transform: uppercase;
            margin-bottom: 0.75rem;
            display: flex;
            justify-content: space-between;
        }

        .nav-grid-box {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(44px, 1fr));
            gap: 0.45rem;
            overflow-y: auto;
            padding-right: 0.25rem;
            max-height: 340px;
            align-content: start;
            margin-bottom: 0.5rem;
        }
        
        .grid-btn {
            height: 38px;
            border: none;
            border-radius: 0.45rem;
            font-weight: 700;
            font-size: 0.82rem;
            cursor: pointer;
            color: white;
            transition: transform 0.1s ease;
        }
        .grid-btn:hover { transform: scale(1.05); }
        .grid-btn.unfilled { background-color: var(--danger-red); }
        .grid-btn.filled { background-color: var(--success-green); }
        .grid-btn.active-now { outline: 3px solid var(--primary-blue); outline-offset: 1px; }

        .palette-legend {
            display: flex;
            gap: 0.85rem;
            font-size: 0.76rem;
            font-weight: 700;
            color: var(--text-muted);
            margin: 0.5rem 0 0.75rem;
            padding-top: 0.65rem;
            border-top: 1px solid var(--border-color);
        }
        .legend-dot {
            display: inline-block;
            width: 10px;
            height: 10px;
            border-radius: 3px;
            margin-right: 4px;
            vertical-align: middle;
        }

        .submit-btn {
            width: 100%;
            padding: 0.9rem;
            background: var(--success-green);
            color: white;
            border: none;
            border-radius: 0.75rem;
            font-weight: 700;
            font-size: 0.98rem;
            cursor: pointer;
            margin-top: 0.25rem;
            transition: opacity 0.2s;
        }
        .submit-btn:hover { opacity: 0.92; }

        /* Question, Statement Box (Testbook Style) & Option Styles */
        .category-tag {
            font-size: 0.78rem;
            font-weight: 800;
            color: var(--primary-blue);
            text-transform: uppercase;
            letter-spacing: 0.05em;
            margin-bottom: 0.6rem;
            display: inline-block;
        }
        .question-text { 
            font-size: 1.12rem; 
            font-weight: 700; 
            margin-bottom: 1rem; 
            line-height: 1.7; 
            white-space: pre-line; 
            color: var(--text-dark);
        }
        .statement-box {
            background: #f8fafc;
            border: 1.5px solid #cbd5e1;
            border-left: 4px solid var(--primary-blue);
            border-radius: 0.65rem;
            padding: 0.9rem 1.1rem;
            margin-bottom: 1.25rem;
            font-size: 1.02rem;
            font-weight: 600;
            line-height: 1.75;
            color: #1e293b;
            white-space: pre-line;
        }
        .statement-box strong {
            color: #0f172a;
            font-weight: 800;
        }
        
        .options-list { display: flex; flex-direction: column; gap: 0.7rem; }
        .option-item {
            width: 100%;
            text-align: left;
            padding: 0.95rem 1.1rem;
            background: white;
            border: 2px solid var(--border-color);
            border-radius: 0.75rem;
            font-size: 0.98rem;
            font-weight: 600;
            line-height: 1.55;
            cursor: pointer;
            transition: all 0.2s ease;
            display: flex;
            align-items: center;
            gap: 0.85rem;
        }
        .option-item:hover { border-color: var(--text-muted); background: #f8fafc; }
        .option-item.selected { border-color: var(--primary-blue); background: #eff6ff; color: var(--primary-blue); }
        .opt-badge {
            width: 28px;
            height: 28px;
            border-radius: 50%;
            background: #f1f5f9;
            color: var(--text-dark);
            display: inline-flex;
            align-items: center;
            justify-content: center;
            font-weight: 800;
            font-size: 0.82rem;
            flex-shrink: 0;
        }
        .option-item.selected .opt-badge { background: var(--primary-blue); color: white; }

        .timer-box { font-family: monospace; font-weight: 700; font-size: 1.15rem; padding: 0.4rem 0.85rem; background: #f1f5f9; border-radius: 0.5rem; }
        .timer-box.warning { background: #fee2e2; color: var(--danger-red); }

        /* Dashboard & Overlay */
        .overlay {
            position: fixed; inset: 0; background: rgba(15, 23, 42, 0.95);
            display: none; flex-direction: column; align-items: center; justify-content: center;
            color: white; z-index: 100; backdrop-filter: blur(4px);
        }
        .spinner {
            width: 45px; height: 45px; border: 4px solid rgba(255, 255, 255, 0.1);
            border-top-color: var(--primary-blue); border-radius: 50%;
            animation: spin 1s linear infinite; margin-bottom: 1rem;
        }
        @keyframes spin { to { transform: rotate(360deg); } }

        .results-dashboard { display: none; width: 100%; max-width: 950px; margin: 2rem auto; padding: 0 1.5rem 3rem; }
        .metrics-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 1rem; margin-bottom: 1.75rem; }
        .metric-card { background: white; padding: 1.25rem; border-radius: 1rem; text-align: center; border: 1px solid var(--border-color); box-shadow: 0 2px 4px rgba(0,0,0,0.03); }
        .metric-label { font-size: 0.72rem; font-weight: 700; color: var(--text-muted); text-transform: uppercase; margin-bottom: 0.35rem; }
        .score-output { color: var(--primary-blue); font-size: 2.1rem; font-weight: 900; }
        .right-output { color: var(--success-green); font-size: 2.1rem; font-weight: 900; }
        .wrong-output { color: var(--danger-red); font-size: 2.1rem; font-weight: 900; }
        .neg-output { color: var(--warning-amber); font-size: 2.1rem; font-weight: 900; }
        .accuracy-output { color: var(--text-dark); font-size: 2.1rem; font-weight: 900; }
        
        /* Diagnostic Feedback Box */
        .diagnostic-card {
            background: white;
            border-radius: 1rem;
            padding: 1.75rem;
            margin-bottom: 1.75rem;
            border: 1px solid var(--border-color);
            border-left: 6px solid var(--primary-blue);
            box-shadow: 0 4px 12px rgba(0,0,0,0.03);
        }
        .diag-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1rem;
            margin-top: 1rem;
        }
        .diag-item {
            background: #f8fafc;
            padding: 1rem;
            border-radius: 0.75rem;
            border: 1px solid var(--border-color);
        }
        .diag-item h4 { font-size: 0.85rem; text-transform: uppercase; margin-bottom: 0.4rem; }

        /* Action Banner for PDF Download */
        .pdf-download-banner {
            background: linear-gradient(135deg, #1e293b, #0f172a);
            color: white;
            padding: 1.65rem;
            border-radius: 1rem;
            margin-bottom: 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 1rem;
            box-shadow: 0 10px 20px rgba(0,0,0,0.12);
        }

        .review-card { background: white; padding: 1.25rem; border-radius: 0.75rem; border: 1px solid var(--border-color); margin-bottom: 1rem; line-height: 1.6; }
        .review-card.correct { border-left: 6px solid var(--success-green); }
        .review-card.wrong { border-left: 6px solid var(--danger-red); }
        .review-card.skipped { border-left: 6px solid var(--text-muted); }
        .explanation-text { margin-top: 0.75rem; padding: 0.75rem; background: #f8fafc; border-radius: 0.5rem; font-size: 0.92rem; border-left: 3px solid var(--primary-blue); line-height: 1.6; }
        .hidden-view { display: none !important; }

        /* Admin Modal */
        .admin-modal-bg {
            position: fixed; inset: 0; background: rgba(0,0,0,0.75); display: none;
            align-items: center; justify-content: center; z-index: 200; padding: 1rem;
        }
        .admin-modal-box {
            background: white; border-radius: 1.25rem; width: 100%; max-width: 960px;
            max-height: 92vh; display: flex; flex-direction: column; overflow: hidden;
            box-shadow: 0 25px 50px -12px rgba(0,0,0,0.25);
        }
        .admin-header { background: #1e293b; color: white; padding: 1.1rem 1.5rem; display: flex; justify-content: space-between; align-items: center; }
        .admin-body { padding: 1.5rem; overflow-y: auto; flex: 1; }
        .tab-buttons { display: flex; gap: 0.5rem; margin-bottom: 1rem; border-bottom: 2px solid #e2e8f0; padding-bottom: 0.5rem; flex-wrap: wrap; }
        .tab-btn { padding: 0.5rem 1rem; border: none; background: #f1f5f9; border-radius: 0.45rem; cursor: pointer; font-weight: 700; font-size: 0.85rem; }
        .tab-btn.active { background: var(--primary-blue); color: white; }
        
        .admin-input-area { width: 100%; height: 210px; padding: 0.85rem; border: 1.5px solid var(--border-color); border-radius: 0.5rem; font-size: 0.92rem; line-height: 1.55; }
        .admin-text-field { width: 100%; padding: 0.7rem; border: 1.5px solid var(--border-color); border-radius: 0.5rem; font-size: 0.9rem; }
        
        .admin-controls-row {
            display: grid;
            grid-template-columns: 1.5fr 1.6fr 0.9fr 1.2fr;
            gap: 0.75rem;
            margin-bottom: 1rem;
        }

        .id-gen-group {
            display: flex;
            gap: 0.35rem;
            align-items: center;
        }

        .btn-gen-mini {
            background: #0f172a;
            color: #ffffff;
            border: none;
            padding: 0.7rem 0.75rem;
            border-radius: 0.5rem;
            font-weight: 800;
            font-size: 0.8rem;
            cursor: pointer;
            white-space: nowrap;
            transition: background 0.2s;
        }
        .btn-gen-mini:hover { background: var(--primary-blue); }

        .url-lock-strip {
            background: #f1f5f9;
            border: 1px dashed #94a3b8;
            padding: 0.65rem 0.9rem;
            border-radius: 0.55rem;
            font-size: 0.8rem;
            color: #334155;
            margin-bottom: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .isolation-alert {
            background: #eff6ff;
            border: 1.5px solid #93c5fd;
            color: #1e40af;
            padding: 0.75rem 1rem;
            border-radius: 0.65rem;
            font-size: 0.83rem;
            margin-bottom: 1rem;
            line-height: 1.5;
        }

        .lifetime-ip-banner {
            background: #f0fdf4;
            border: 1.5px solid #86efac;
            padding: 0.9rem 1.2rem;
            border-radius: 0.75rem;
            margin-bottom: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 0.75rem;
        }

        .action-bar { display: flex; gap: 0.75rem; margin-top: 1.25rem; flex-wrap: wrap; }
        .btn-green { background: var(--success-green); color: white; border: none; padding: 0.8rem 1.3rem; border-radius: 0.5rem; font-weight: 700; cursor: pointer; }
        .btn-blue { background: var(--primary-blue); color: white; border: none; padding: 0.8rem 1.3rem; border-radius: 0.5rem; font-weight: 700; cursor: pointer; }
        .btn-red { background: var(--danger-red); color: white; border: none; padding: 0.8rem 1.3rem; border-radius: 0.5rem; font-weight: 700; cursor: pointer; }
        .btn-green:hover, .btn-blue:hover, .btn-red:hover { opacity: 0.9; }

        /* Tables in Admin */
        .admin-table { width: 100%; border-collapse: collapse; font-size: 0.88rem; margin-top: 0.5rem; }
        .admin-table th, .admin-table td { padding: 0.75rem; border-bottom: 1px solid var(--border-color); text-align: left; }
        .admin-table th { background: #f8fafc; font-weight: 700; color: var(--text-muted); }

        /* Device Block Screen */
        .blocked-screen {
            position: fixed; inset: 0; background: #0f172a; color: white;
            display: none; flex-direction: column; align-items: center; justify-content: center;
            z-index: 999; padding: 1.5rem; text-align: center; overflow-y: auto;
        }
        .blocked-card {
            background: #1e293b;
            border: 1px solid #334155;
            padding: 2.25rem;
            border-radius: 1.25rem;
            max-width: 520px;
            width: 100%;
            box-shadow: 0 25px 50px -12px rgba(0,0,0,0.5);
        }
        .dark-input {
            width: 100%;
            padding: 0.8rem 1rem;
            border-radius: 0.5rem;
            border: 1px solid #475569;
            background: #0f172a;
            color: white;
            margin-bottom: 0.85rem;
            font-size: 0.92rem;
        }

        /* Crisp Vector Print / Save-as-PDF Styles */
        #pdf-print-sheet { display: none; }

        @media print {
            body * { visibility: hidden !important; }
            #pdf-print-sheet, #pdf-print-sheet * { visibility: visible !important; }
            #pdf-print-sheet {
                display: block !important;
                position: absolute;
                left: 0;
                top: 0;
                width: 100%;
                background: #ffffff !important;
                color: #0f172a !important;
                padding: 15px 20px;
                font-family: 'Noto Sans Telugu', 'Inter', sans-serif !important;
            }
            .pdf-q-block {
                page-break-inside: avoid;
                break-inside: avoid;
                margin-bottom: 16px;
                padding-bottom: 12px;
                border-bottom: 1px solid #cbd5e1;
            }
        }

        @media (max-width: 768px) {
            .app-container { flex-direction: column; padding: 0.75rem; }
            aside { width: 100%; position: static; }
            .admin-controls-row { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <!-- ================= BLOCKED USER LOCK OVERLAY & REQUEST TO ADMIN ================= -->
    <div class="blocked-screen" id="device-blocked-screen">
        <div class="blocked-card">
            <div style="font-size: 3.5rem; margin-bottom: 0.5rem;">🚫</div>
            <h1 style="font-size: 1.75rem; font-weight: 900; color: #f87171; margin-bottom: 0.5rem;">Access Permanently Blocked</h1>
            <p style="color: #94a3b8; font-size: 0.9rem; margin-bottom: 1.5rem;">
                Your ID and IP have been permanently locked due to 2 unauthorized administrator password attempts.
            </p>
            
            <div style="text-align: left; background: #0f172a; padding: 1.25rem; border-radius: 0.85rem; border: 1px solid #334155;">
                <h3 style="font-size: 1rem; font-weight: 800; color: #f8fafc; margin-bottom: 0.85rem; text-align: center;">📩 Request to Admin for Unblock</h3>
                
                <label style="font-size: 0.78rem; font-weight: 700; color: #94a3b8; display: block; margin-bottom: 0.25rem;">YOUR FULL NAME *</label>
                <input type="text" id="req-unblock-name" class="dark-input" placeholder="Enter your full name" required>

                <label style="font-size: 0.78rem; font-weight: 700; color: #94a3b8; display: block; margin-bottom: 0.25rem;">YOUR EMAIL ID *</label>
                <input type="email" id="req-unblock-email" class="dark-input" placeholder="yourname@email.com" required>

                <label style="font-size: 0.78rem; font-weight: 700; color: #94a3b8; display: block; margin-bottom: 0.25rem;">REASON FOR UNBLOCK / RECOVERY KEY *</label>
                <textarea id="req-unblock-reason" class="dark-input" style="height: 80px; resize: none;" placeholder="Explain why your access should be restored or enter recovery code..." required></textarea>

                <button class="btn-blue" style="width: 100%; padding: 0.85rem;" onclick="triggerAdminUnblockRequest()">🚀 Submit Request to Admin</button>
                <div id="unblock-req-status" style="margin-top: 0.75rem; font-size: 0.85rem; font-weight: 700; color: #4ade80; text-align: center;"></div>
            </div>
        </div>
    </div>

    <!-- ================= TOP NAVBAR ================= -->
    <header class="top-navbar">
        <div class="portal-brand">
            <span>🎓 Comprehensive Online Exam Portal</span>
            <span class="live-badge"><span class="live-dot"></span> Active Assessment</span>
        </div>
        <button class="admin-trigger-btn" onclick="openAdminModal()">🔐 Admin Portal</button>
    </header>

    <!-- ================= WAITING FOR QUESTIONS VIEW ================= -->
    <section class="waiting-screen" id="waiting-view">
        <div class="waiting-card">
            <div class="waiting-pulse"></div>
            <h2 style="font-size: 1.65rem; font-weight: 800; margin-bottom: 0.5rem;">Waiting for the questions...</h2>
            <p style="color: var(--text-muted); font-size: 0.95rem; line-height: 1.6;">
                This post has its own isolated namespace and is currently empty. Open the Admin Panel to generate a Unique Lock ID and publish questions exclusively for this post.
            </p>
        </div>
    </section>

    <!-- ================= QUIZ MAIN UI CONTAINER (SIDE BY SIDE) ================= -->
    <div class="app-container" id="quiz-view" style="display: none;">
        <main>
            <header class="exam-header">
                <h1 id="test-title-header" style="font-weight: 800; font-size: 1.15rem; margin:0;">Live Mock Test</h1>
                <div class="timer-box" id="clock">60s</div>
            </header>
            <div class="quiz-arena">
                <article class="question-card">
                    <span class="category-tag" id="q-category">Exam Set Assessment</span>
                    <h2 class="question-text" id="q-text">Loading exam questions...</h2>
                    <div class="statement-box" id="q-statements" style="display: none;"></div>
                    <div class="options-list" id="q-options"></div>
                    
                    <div class="card-footer-nav">
                        <button class="btn-outline" onclick="clearCurrentAnswer()">Clear Response</button>
                        <button class="btn-next-q" onclick="autoAdvance()">Save & Next ➔</button>
                    </div>
                </article>
            </div>
        </main>
        
        <aside>
            <div class="grid-title">
                <span>Questions Palette</span>
                <span id="answered-stat">0 / 0</span>
            </div>
            <div class="nav-grid-box" id="nav-grid"></div>
            <div class="palette-legend">
                <span><i class="legend-dot" style="background: var(--success-green);"></i>Answered</span>
                <span><i class="legend-dot" style="background: var(--danger-red);"></i>Unanswered</span>
            </div>
            <button class="submit-btn" onclick="triggerSubmission()">Submit Exam</button>
        </aside>
    </div>

    <!-- ================= PROCESSING OVERLAY ================= -->
    <div class="overlay" id="processing-screen">
        <div class="spinner"></div>
        <h3 style="font-size: 1.4rem; font-weight: 700;">Evaluating Scorecard & Diagnostic Analytics...</h3>
    </div>

    <!-- ================= DIAGNOSTIC RESULTS DASHBOARD ================= -->
    <section class="results-dashboard" id="dashboard-view">
        <div style="text-align: center; margin-bottom: 2rem;">
            <h2 style="font-size: 2.2rem; font-weight: 900; color: var(--text-dark);">Performance Scorecard & Analysis</h2>
            <p style="color: var(--text-muted); margin-bottom: 1.25rem;">Complete Diagnostic Breakdown (+1 Correct | -0.5 Negative)</p>
            <button style="padding: 0.75rem 1.5rem; background: var(--primary-blue); color:white; border:none; border-radius:0.6rem; font-weight:700; cursor:pointer; font-size: 1rem;" onclick="restartExam()">🔄 Re-Attempt Exam</button>
        </div>

        <div class="metrics-grid">
            <div class="metric-card"><div class="metric-label">Final Score (+1 / -0.5)</div><div class="score-output" id="res-score">0</div></div>
            <div class="metric-card"><div class="metric-label">Correct (+1.0)</div><div class="right-output" id="res-correct">0</div></div>
            <div class="metric-card"><div class="metric-label">Wrong Answers</div><div class="wrong-output" id="res-wrong">0</div></div>
            <div class="metric-card"><div class="metric-label">Negative Marks Lost</div><div class="neg-output" id="res-negative">-0.0</div></div>
            <div class="metric-card"><div class="metric-label">Accuracy</div><div class="accuracy-output" id="res-accuracy">0%</div></div>
        </div>

        <!-- Personalised Strengths, Weaknesses & Preparation Guidance -->
        <div class="diagnostic-card">
            <h3 style="font-size: 1.25rem; font-weight: 800; color: var(--text-dark);">📊 Personalised Preparation & Diagnostic Report</h3>
            <p id="diag-summary-line" style="margin-top: 0.4rem; color: var(--text-muted); font-size: 0.95rem;"></p>
            
            <div class="diag-grid">
                <div class="diag-item">
                    <h4 style="color: var(--success-green);">💪 Positive Areas (Strengths)</h4>
                    <p id="diag-positive" style="font-size: 0.9rem; line-height: 1.55;"></p>
                </div>
                <div class="diag-item">
                    <h4 style="color: var(--danger-red);">⚠️ Weak Areas (Needs Focus)</h4>
                    <p id="diag-weak" style="font-size: 0.9rem; line-height: 1.55;"></p>
                </div>
                <div class="diag-item">
                    <h4 style="color: var(--primary-blue);">📚 What to Study & How Hard to Work</h4>
                    <p id="diag-study-plan" style="font-size: 0.9rem; line-height: 1.55;"></p>
                </div>
            </div>
        </div>

        <!-- Download Correct Options & Explanations PDF Banner -->
        <div class="pdf-download-banner">
            <div>
                <h3 style="font-size: 1.2rem; font-weight: 800; margin-bottom: 0.25rem;">📥 Download Official Correct Answers & Solutions PDF</h3>
                <p style="font-size: 0.88rem; color: #94a3b8;">Save a crystal-clear Telugu & English revision PDF containing verified correct answers and explanations.</p>
            </div>
            <button class="btn-green" style="padding: 0.9rem 1.5rem; font-size: 0.95rem; white-space: nowrap;" onclick="downloadCorrectOptionsPDF()">📄 Download Clean PDF Key</button>
        </div>

        <h3 style="margin-bottom: 1rem; font-size: 1.3rem; font-weight: 800;">Detailed Question-by-Question Review:</h3>
        <div id="review-wrapper"></div>
    </section>

    <!-- Vector Print Sheet for 100% Accurate Telugu & English PDF Generation -->
    <div id="pdf-print-sheet">
        <div style="border-bottom: 2px solid #2563eb; padding-bottom: 10px; margin-bottom: 18px;">
            <h1 id="pdf-doc-title" style="font-size: 20px; color: #0f172a; margin-bottom: 4px; font-weight: 800;">Mock Test Solutions & Key</h1>
            <p style="font-size: 12px; color: #475569;">Verified Correct Options & Detailed Explanations for Revision</p>
        </div>
        <div id="pdf-questions-body"></div>
    </div>

    <!-- ================= ADMIN SECURITY & CONVERTER MODAL ================= -->
    <div class="admin-modal-bg" id="admin-modal">
        <div class="admin-modal-box">
            <div class="admin-header">
                <h3 style="font-size: 1.15rem; font-weight: 800; margin:0;">🔐 Admin Control Center & Auto-Isolated Post Engine</h3>
                <button style="background:none; border:none; color:white; font-size:1.5rem; cursor:pointer;" onclick="closeAdminModal()">✕</button>
            </div>

            <!-- 1. Strict Password Login View -->
            <div class="admin-body" id="admin-login-view">
                <p style="margin-bottom: 0.5rem; font-size: 0.95rem; color: var(--text-muted);">Enter Admin Password (Auto-Opens on Valid Key):</p>
                <input type="password" id="admin-pin" class="admin-text-field" placeholder="••••••" maxlength="6" oninput="handlePinAutoCheck(event)" style="letter-spacing: 0.3em; font-weight: 800; font-size: 1.1rem; text-align: center; margin-bottom: 1rem;">
                <div id="pin-warning" style="color: var(--danger-red); font-size: 0.88rem; font-weight: 700; margin-bottom: 0.75rem; text-align: center;"></div>
                <button class="btn-blue" style="width: 100%; padding: 0.8rem;" onclick="validatePinManual()">Unlock Admin Panel</button>
            </div>

            <!-- 2. Full Unlocked Admin Dashboard -->
            <div class="admin-body" id="admin-dashboard-view" style="display: none;">
                
                <!-- Lifetime IP Confirmation -->
                <div class="lifetime-ip-banner" id="lifetime-ip-box">
                    <div>
                        <strong style="color: #166534; font-size: 0.95rem; display: block;">🛡️ Admin Lifetime IP & Device Confirmation</strong>
                        <span style="font-size: 0.82rem; color: #15803d;" id="lifetime-ip-status-text">Confirm your current IP (<span id="admin-current-ip">Detecting...</span>) to open Admin Panel without password next time.</span>
                    </div>
                    <button class="btn-green" id="confirm-ip-btn" style="padding: 0.55rem 1.1rem; font-size: 0.85rem;" onclick="confirmAdminLifetimeIP()">✅ Confirm IP for Lifetime</button>
                </div>

                <!-- Live URL & Unique Post Lock Status -->
                <div class="url-lock-strip">
                    <div>
                        <strong>🔗 Locked Post URL:</strong> <span id="display-locked-url" style="font-family: monospace; color: var(--primary-blue);"></span>
                    </div>
                    <div>
                        <strong>🔑 Active Namespace Lock:</strong> <code id="display-active-lock" style="background: #e2e8f0; padding: 2px 6px; border-radius: 4px; font-weight: 800;"></code>
                    </div>
                </div>

                <!-- Post Isolation Guide Banner -->
                <div class="isolation-alert">
                    <strong>🔒 100% Zero-Mix Auto-Isolation Active:</strong><br>
                    Each Blogger post URL automatically generates and locks its own cryptographic <b>Unique Post ID</b> with special characters. Simply click <b>"🎲 Generate"</b> (or use the auto-assigned ID), paste your raw questions below, and click <b>"🚀 Parse, Save & Make Exam Live"</b>. Data stays strictly inside this post and will <b>NEVER</b> mix with any other post!
                </div>

                <div class="tab-buttons">
                    <button class="tab-btn active" id="tab-btn-text" onclick="switchAdminTab('text')">📝 Smart Text Paste & Auto-Lock</button>
                    <button class="tab-btn" id="tab-btn-link" onclick="switchAdminTab('link')">🔗 Paste JSON URL</button>
                    <button class="tab-btn" id="tab-btn-security" onclick="switchAdminTab('security')">🛡️ Security & Unblock Controls</button>
                </div>

                <!-- Tab 1: Smart Text Paste -->
                <div id="admin-tab-text">
                    <div class="admin-controls-row">
                        <div>
                            <label style="font-weight: 700; font-size: 0.82rem; display: block; margin-bottom: 0.3rem;">Exam Title:</label>
                            <input type="text" id="admin-test-title" class="admin-text-field" value="Live Mock Test">
                        </div>
                        <div>
                            <label style="font-weight: 700; font-size: 0.82rem; display: block; margin-bottom: 0.3rem;">Unique Post Lock ID:</label>
                            <div class="id-gen-group">
                                <input type="text" id="admin-post-id" class="admin-text-field" style="font-family: monospace; font-weight: 700; font-size: 0.82rem;" readonly>
                                <button type="button" class="btn-gen-mini" onclick="generateAndBindUniquePostID()" title="Generate New Random Unique Post ID">🎲 Generate</button>
                            </div>
                        </div>
                        <div>
                            <label style="font-weight: 700; font-size: 0.82rem; display: block; margin-bottom: 0.3rem;">Start Q No.:</label>
                            <input type="number" id="admin-start-qnum" class="admin-text-field" value="1" min="1" placeholder="e.g. 1">
                        </div>
                        <div>
                            <label style="font-weight: 700; font-size: 0.82rem; display: block; margin-bottom: 0.3rem;">Upload Mode:</label>
                            <select id="admin-upload-mode" class="admin-text-field" onchange="handleUploadModeChange()">
                                <option value="replace">New / Replace Post Set</option>
                                <option value="append">Add After Existing Qs</option>
                            </select>
                        </div>
                    </div>

                    <p style="font-size: 0.82rem; color: var(--text-muted); margin-bottom: 0.5rem;">
                        Supports both Normal Questions & Testbook Statement / ప్రకటనలు-తీర్మానాలు Questions (Always shows A, B, C, D options only):<br>
                        <i>Q1. Question & Statements (A, B, C, D / ప్రకటనలు / తీర్మానాలు)...<br>A. Option 1 &nbsp; B. Option 2 &nbsp; C. Option 3 &nbsp; D. Option 4<br>Answer : Option Text &nbsp; Exp: Explanation</i>
                    </p>
                    <textarea id="admin-raw-text" class="admin-input-area" placeholder="Paste your raw questions here..."></textarea>
                    <div style="display: flex; gap: 0.6rem; margin-top: 0.6rem; flex-wrap: wrap;">
                        <button class="btn-blue" onclick="parseRawText(true)">⚡ Parse & Preview Count</button>
                        <button class="btn-red" style="padding: 0.8rem 1rem;" onclick="clearAllQuestions()">🗑️ Clear Only This Post</button>
                    </div>
                </div>

                <!-- Tab 2: Link Paste -->
                <div id="admin-tab-link" style="display: none;">
                    <p style="font-size: 0.85rem; color: var(--text-muted); margin-bottom: 0.5rem;">Paste Raw JSON URL (e.g. GitHub, Gist, API):</p>
                    <input type="text" id="admin-json-url" class="admin-text-field" placeholder="https://api.example.com/questions.json" style="margin-bottom: 0.75rem;">
                    <button class="btn-blue" onclick="fetchFromLink()">⚡ Fetch from Link</button>
                </div>

                <!-- Tab 3: Security & Blocked Users -->
                <div id="admin-tab-security" style="display: none;">
                    <div style="background: #f8fafc; padding: 1rem; border-radius: 0.5rem; border: 1px solid var(--border-color); margin-bottom: 1rem; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 0.5rem;">
                        <div>
                            <strong style="font-size: 0.9rem; display: block;">Lifetime Admin IP Status</strong>
                            <small style="color: var(--text-muted);">If you want the portal to ask for the password again on this device, revoke confirmation.</small>
                        </div>
                        <button class="btn-red" style="padding: 0.5rem 0.9rem; font-size: 0.8rem;" onclick="revokeLifetimeIP()">🔒 Require Password Again</button>
                    </div>

                    <span style="font-weight: 800; font-size: 0.95rem;">Blocked Entities & Intrusion Logs</span>
                    <div style="overflow-x: auto; margin-top: 0.5rem;">
                        <table class="admin-table">
                            <thead>
                                <tr>
                                    <th>Target Identifier</th>
                                    <th>Reason</th>
                                    <th>Blocked On</th>
                                    <th>Actions</th>
                                </tr>
                            </thead>
                            <tbody id="block-list-table-body">
                                <tr><td colspan="4" style="text-align: center; color: var(--text-muted);">No devices currently blocked.</td></tr>
                            </tbody>
                        </table>
                    </div>
                </div>

                <div id="admin-status" style="margin-top: 1rem; font-weight: 700; font-size: 0.92rem; color: var(--success-green);"></div>

                <div class="action-bar">
                    <button class="btn-green" onclick="applyAndLaunch()">🚀 Parse, Save & Make Exam Live</button>
                    <button class="btn-blue" onclick="copyBloggerCode()">📋 Copy Permanent HTML (Optional Backup)</button>
                </div>
            </div>
        </div>
    </div>

    <!-- ================= OBFUSCATED CRYPTO & ZERO-CONFLICT ENGINE ================= -->
    <script>
        /*
         * =========================================================================
         * ZERO-CONFLICT AUTOMATIC URL + RANDOM UNIQUE ID ISOLATION ENGINE (V3)
         * =========================================================================
         */
        let POST_UNIQUE_ID = "";

        // Embedded questions (used only if you export standalone HTML backup)
        const embeddedPostData = [];

        /*
         * CUSTOM SYMBOLIC & GARBAGE-STYLE ENCRYPTION VAULT
         */
        const _0xVault = {
            _salt: "sbabysksosñe bzhhebnalnsbgshan -₹+#:-@{=@=@_-#++ß",
            _adminCipher: "sbabysksosñe#A1!bzhhebnalnsbgshan#A2!-₹+#:-@{=@=@_-#++#A6!ß#A2!sbabysksosñe#A7!bzhhebnalnsbgshan#A7!ß",
            _unblockCipher: "sbabysksosñe#B11!bzhhebnalnsbgshan#B6!-₹+#:-@{=@=@_-#++#B1!ß#B6!sbabysksosñe-₹+#:-@{=@=@_-#++ß",
            _mailCipher: "sbabysksosñe~89!~97!~126!~102!~112!~108!~105!~101!~108!~122!~108!~127!~108!~105!~101!~60!~57!~62!~77!~106!~96!~108!~100!~97!~35!~110!~98!~96!bzhhebnalnsbgshan-₹+#:-@{=@=@_-#++ß",
            
            verifyAdmin: function(input) {
                if (!input || input.length !== 6) return false;
                const tokens = this._adminCipher.match(/#A(\d+)!/g);
                if (!tokens) return false;
                const reconstructed = tokens.map(t => {
                    const n = parseInt(t.replace(/[#A!]/g, ''), 10);
                    return String.fromCharCode((n ^ 3) + 48);
                }).join('');
                return input === reconstructed;
            },

            verifyUnblockKey: function(text) {
                if (!text) return false;
                const tokens = this._unblockCipher.match(/#B(\d+)!/g);
                if (!tokens) return false;
                const key = tokens.map(t => {
                    const n = parseInt(t.replace(/[#B!]/g, ''), 10);
                    return String.fromCharCode((n ^ 3) + 48);
                }).join('');
                return text.trim() === key || new RegExp(`\\b${key}\\b`).test(text);
            },

            getReceiver: function() {
                const tokens = this._mailCipher.match(/~(\d+)!/g);
                if (!tokens) return "";
                return tokens.map(t => {
                    const n = parseInt(t.replace(/[~!]/g, ''), 10);
                    return String.fromCharCode(n ^ 13);
                }).join('');
            }
        };

        function createRandomUniquePostID() {
            const chars = "ABCDEFGHJKLMNPQRSTUVWXYZ23456789";
            const specials = ["#", "@", "$", "&", "~", "!", "*"];
            let randPart1 = "";
            let randPart2 = "";
            for (let i = 0; i < 6; i++) {
                randPart1 += chars.charAt(Math.floor(Math.random() * chars.length));
                randPart2 += chars.charAt(Math.floor(Math.random() * chars.length));
            }
            const sym1 = specials[Math.floor(Math.random() * specials.length)];
            const sym2 = specials[Math.floor(Math.random() * specials.length)];
            const timeHex = Date.now().toString(36).toUpperCase().slice(-5);
            return `UID${sym1}${randPart1}-${timeHex}${sym2}${randPart2}`;
        }

        function getExactUrlSignature() {
            const rawUrl = (window.location.origin + window.location.pathname + window.location.search).toLowerCase();
            let hash1 = 5381;
            let hash2 = 52711;
            for (let i = 0; i < rawUrl.length; i++) {
                const ch = rawUrl.charCodeAt(i);
                hash1 = ((hash1 << 5) + hash1) ^ ch;
                hash2 = ((hash2 << 5) + hash2) + ch;
            }
            const hex1 = (hash1 >>> 0).toString(16).toUpperCase().padStart(8, '0');
            const hex2 = (hash2 >>> 0).toString(16).toUpperCase().padStart(8, '0');
            const slug = (window.location.pathname || 'home')
                .toLowerCase()
                .replace(/[^a-z0-9]/g, '_')
                .replace(/_+/g, '_')
                .replace(/^_|_$/g, '')
                .slice(-36) || 'ROOT';
            return `${slug}__${hex1}_${hex2}`;
        }

        function resolvePostUniqueID() {
            const urlSig = getExactUrlSignature();
            const registryKey = `ZC_URL_ID_MAP_V3::${urlSig}`;

            if (POST_UNIQUE_ID && POST_UNIQUE_ID.trim().length > 0) {
                localStorage.setItem(registryKey, POST_UNIQUE_ID.trim());
                return POST_UNIQUE_ID.trim();
            }

            let existingId = localStorage.getItem(registryKey);
            if (!existingId) {
                existingId = createRandomUniquePostID();
                localStorage.setItem(registryKey, existingId);
            }
            POST_UNIQUE_ID = existingId;
            return existingId;
        }

        function getIsolatedStorageKeys() {
            const urlSig = getExactUrlSignature();
            const activeId = resolvePostUniqueID();
            return {
                URL_SIG: urlSig,
                POST_ID: activeId,
                REGISTRY: `ZC_URL_ID_MAP_V3::${urlSig}`,
                DATA: `ZC_V3_DATA::${urlSig}::[${activeId}]`,
                TITLE: `ZC_V3_TITLE::${urlSig}::[${activeId}]`
            };
        }

        function generateAndBindUniquePostID() {
            const urlSig = getExactUrlSignature();
            const newId = createRandomUniquePostID();
            POST_UNIQUE_ID = newId;

            localStorage.setItem(`ZC_URL_ID_MAP_V3::${urlSig}`, newId);

            const inputEl = document.getElementById('admin-post-id');
            if (inputEl) inputEl.value = newId;

            const lockBadge = document.getElementById('display-active-lock');
            if (lockBadge) lockBadge.innerText = newId;

            const rawText = document.getElementById('admin-raw-text').value.trim();
            if (rawText) {
                parseRawText(true);
            }
            const activeQuestions = (previewDataSet && previewDataSet.length > 0) ? previewDataSet : dataSet;
            if (Array.isArray(activeQuestions) && activeQuestions.length > 0) {
                const keys = getIsolatedStorageKeys();
                localStorage.setItem(keys.DATA, JSON.stringify(activeQuestions));
                const title = document.getElementById('admin-test-title').value.trim();
                if (title) localStorage.setItem(keys.TITLE, title);
                document.getElementById('admin-status').innerText = 
                    `🎲 Generated New Unique Lock [${newId}] & automatically bound ${activeQuestions.length} questions strictly to this URL!`;
            } else {
                document.getElementById('admin-status').innerText = 
                    `🎲 Generated & Locked New Unique Post ID [${newId}] for this URL! Paste your questions and click Save & Make Exam Live.`;
            }
        }

        let dataSet = [];
        let previewDataSet = null;
        let state = {
            currentIdx: 0,
            answers: [],
            timeLeft: 60,
            timerId: null,
            testTitle: "Live Mock Test",
            clientIP: "LOCAL_ADMIN_DEVICE",
            failedAttempts: 0
        };

        /* ================= 1. INITIALIZATION & STRICT POST ISOLATION ================= */
        async function initPortal() {
            updateBackgroundSEO();

            state.failedAttempts = parseInt(localStorage.getItem('ADMIN_FAILED_ATTEMPTS') || '0', 10);

            if (isDeviceBlocked()) {
                document.getElementById('device-blocked-screen').style.display = 'flex';
                return;
            }

            fetchClientIP();

            const keys = getIsolatedStorageKeys();

            const postIdInput = document.getElementById('admin-post-id');
            if (postIdInput) postIdInput.value = keys.POST_ID;

            if (Array.isArray(embeddedPostData) && embeddedPostData.length > 0) {
                dataSet = [...embeddedPostData];
            } else {
                const savedData = localStorage.getItem(keys.DATA);
                if (savedData) {
                    try {
                        dataSet = JSON.parse(savedData);
                    } catch (e) {
                        dataSet = [];
                    }
                } else {
                    dataSet = [];
                }
            }

            const savedTitle = localStorage.getItem(keys.TITLE);
            if (savedTitle) {
                state.testTitle = savedTitle;
                document.getElementById('test-title-header').innerText = savedTitle;
                document.getElementById('admin-test-title').value = savedTitle;
            } else {
                state.testTitle = document.getElementById('test-title-header').innerText || "Live Mock Test";
                document.getElementById('admin-test-title').value = state.testTitle;
            }

            if (!Array.isArray(dataSet) || dataSet.length === 0) {
                showWaitingScreen();
            } else {
                updateBackgroundSEO();
                restartExam();
            }
        }

        function updateBackgroundSEO() {
            const currentUrl = window.location.href;
            const canonicalEl = document.getElementById('seo-canonical');
            if (canonicalEl) canonicalEl.setAttribute('href', currentUrl);

            const pageTitle = (state.testTitle && state.testTitle !== "Live Mock Test")
                ? `${state.testTitle} - Free Online Mock Test & Answer Key PDF`
                : (document.title || "Online Mock Test & Competitive Exam Assessment Portal");

            document.title = pageTitle;
            const ogTitle = document.getElementById('og-title');
            if (ogTitle) ogTitle.setAttribute('content', pageTitle);

            const schemaEl = document.getElementById('dynamic-seo-schema');
            if (schemaEl) {
                const schemaObj = {
                    "@context": "https://schema.org",
                    "@type": "Quiz",
                    "name": pageTitle,
                    "url": currentUrl,
                    "description": "Free online timed mock test in Telugu and English with +1/-0.5 negative marking and verified explanations.",
                    "inLanguage": ["te", "en"],
                    "isAccessibleForFree": true,
                    "numberOfQuestions": Array.isArray(dataSet) ? dataSet.length : 0
                };
                if (Array.isArray(dataSet) && dataSet.length > 0) {
                    schemaObj.hasPart = dataSet.slice(0, 15).map(q => ({
                        "@type": "Question",
                        "name": q.text,
                        "acceptedAnswer": {
                            "@type": "Answer",
                            "text": q.correct
                        }
                    }));
                }
                schemaEl.textContent = JSON.stringify(schemaObj);
            }
        }

        function showWaitingScreen() {
            clearInterval(state.timerId);
            document.getElementById('waiting-view').style.display = 'flex';
            document.getElementById('quiz-view').style.display = 'none';
            document.getElementById('dashboard-view').style.display = 'none';
        }

        function isDeviceBlocked() {
            return localStorage.getItem('DEVICE_IS_BLOCKED') === 'true';
        }

        async function fetchClientIP() {
            try {
                const res = await fetch('https://ipapi.co/json/');
                const data = await res.json();
                if (data && data.ip) {
                    state.clientIP = data.ip;
                    localStorage.setItem('CACHED_IP', state.clientIP);
                }
            } catch (e) {
                state.clientIP = localStorage.getItem('CACHED_IP') || "Verified-Local-IP";
            }
            const ipSpan = document.getElementById('admin-current-ip');
            if (ipSpan) ipSpan.innerText = state.clientIP;
        }

        /* ================= 2. QUIZ EXECUTION ENGINE ================= */
        function restartExam() {
            if (!dataSet || dataSet.length === 0) {
                showWaitingScreen();
                return;
            }
            clearInterval(state.timerId);
            state.currentIdx = 0;
            state.answers = new Array(dataSet.length).fill(null);
            
            document.getElementById('waiting-view').style.display = 'none';
            document.getElementById('dashboard-view').style.display = 'none';
            document.getElementById('quiz-view').style.display = 'flex';
            document.getElementById('quiz-view').classList.remove('hidden-view');
            
            renderNavGrid();
            displayQuestion();
            startClock();
        }

        function renderNavGrid() {
            const grid = document.getElementById('nav-grid');
            grid.innerHTML = '';
            for (let i = 0; i < dataSet.length; i++) {
                const qNumLabel = dataSet[i].qNum || (i + 1);
                const btn = document.createElement('button');
                btn.innerText = qNumLabel;
                btn.id = `nav-btn-${i}`;
                btn.className = `grid-btn ${state.answers[i] !== null ? 'filled' : 'unfilled'}`;
                btn.onclick = () => jumpToQuestion(i);
                grid.appendChild(btn);
            }
            updateCount();
        }

        function updateCount() {
            const answered = state.answers.filter(a => a !== null).length;
            document.getElementById('answered-stat').innerText = `${answered} / ${dataSet.length}`;
        }

        function displayQuestion() {
            if (dataSet.length === 0) return;
            const q = dataSet[state.currentIdx];
            const qNumLabel = q.qNum || (state.currentIdx + 1);
            
            // Strictly display ONLY "Exam Set Assessment" without bullet/question numbers
            document.getElementById('q-category').innerText = "Exam Set Assessment";
            document.getElementById('q-text').innerText = `${qNumLabel}. ${q.text}`;

            // Render Statement / Assertion-Reason / ప్రకటనలు-తీర్మానాలు Box if present
            const stmtBox = document.getElementById('q-statements');
            if (q.statements && q.statements.trim().length > 0) {
                stmtBox.style.display = 'block';
                stmtBox.innerText = q.statements.trim();
            } else {
                stmtBox.style.display = 'none';
                stmtBox.innerText = '';
            }
            
            const optionsBox = document.getElementById('q-options');
            optionsBox.innerHTML = '';
            const letters = ['A', 'B', 'C', 'D'];
            
            // Always show strictly up to 4 options (A, B, C, D)
            const displayOptions = (q.options || []).slice(0, 4);
            displayOptions.forEach((opt, oIdx) => {
                const btn = document.createElement('button');
                const isSelected = state.answers[state.currentIdx] === opt;
                btn.className = `option-item ${isSelected ? 'selected' : ''}`;
                btn.innerHTML = `<span class="opt-badge">${letters[oIdx]}</span><span>${escapeHTML(opt)}</span>`;
                btn.onclick = () => selectAnswer(opt);
                optionsBox.appendChild(btn);
            });

            document.querySelectorAll('.grid-btn').forEach((btn, idx) => {
                btn.classList.toggle('active-now', idx === state.currentIdx);
                btn.classList.toggle('filled', state.answers[idx] !== null);
                btn.classList.toggle('unfilled', state.answers[idx] === null);
            });
        }

        function startClock() {
            clearInterval(state.timerId);
            state.timeLeft = 60;
            const clockEl = document.getElementById('clock');
            clockEl.innerText = `${state.timeLeft}s`;
            clockEl.classList.remove('warning');
            
            state.timerId = setInterval(() => {
                state.timeLeft--;
                clockEl.innerText = `${state.timeLeft}s`;
                if (state.timeLeft <= 10) clockEl.classList.add('warning');
                if (state.timeLeft <= 0) {
                    clearInterval(state.timerId);
                    autoAdvance();
                }
            }, 1000);
        }

        function selectAnswer(selectedOption) {
            state.answers[state.currentIdx] = selectedOption;
            updateCount();
            displayQuestion();
            setTimeout(() => { autoAdvance(); }, 250);
        }

        function clearCurrentAnswer() {
            state.answers[state.currentIdx] = null;
            updateCount();
            displayQuestion();
        }

        function autoAdvance() {
            if (state.currentIdx < dataSet.length - 1) {
                state.currentIdx++;
                displayQuestion();
                startClock();
            } else {
                clearInterval(state.timerId);
                triggerSubmission();
            }
        }

        function jumpToQuestion(idx) {
            state.currentIdx = idx;
            displayQuestion();
            startClock();
        }

        function triggerSubmission() {
            clearInterval(state.timerId);
            document.getElementById('processing-screen').style.display = 'flex';
            setTimeout(() => {
                document.getElementById('processing-screen').style.display = 'none';
                document.getElementById('quiz-view').style.display = 'none';
                document.getElementById('dashboard-view').style.display = 'block';
                window.scrollTo({ top: 0, behavior: 'smooth' });
                renderDashboard();
            }, 700);
        }

        /* ================= 3. DIAGNOSTIC SCORECARD & CRISP TELUGU PDF GENERATOR ================= */
        function renderDashboard() {
            let correct = 0, wrong = 0, skipped = 0;
            let weakTopics = [];
            let strongTopics = [];

            dataSet.forEach((q, idx) => {
                const qNumLabel = q.qNum || (idx + 1);
                const a = state.answers[idx];
                const shortTopic = q.text.split(' ').slice(0, 4).join(' ') + '...';
                if (a === q.correct) {
                    correct++;
                    strongTopics.push(`Q${qNumLabel} (${shortTopic})`);
                } else if (a === null) {
                    skipped++;
                    weakTopics.push(`Q${qNumLabel} [Unattempted]`);
                } else {
                    wrong++;
                    weakTopics.push(`Q${qNumLabel} [Wrong]`);
                }
            });

            const positiveMarks = correct * 1.0;
            const negativeMarks = wrong * 0.5;
            const netScore = positiveMarks - negativeMarks;
            const maxScore = dataSet.length * 1.0;
            const accuracy = (correct + wrong) > 0 ? ((correct / (correct + wrong)) * 100) : 0;
            const percentage = maxScore > 0 ? Math.max(0, (netScore / maxScore) * 100) : 0;

            document.getElementById('res-score').innerText = `${netScore.toFixed(1)} / ${maxScore}`;
            document.getElementById('res-correct').innerText = `+${positiveMarks.toFixed(1)} (${correct})`;
            document.getElementById('res-wrong').innerText = `${wrong} (Skipped: ${skipped})`;
            document.getElementById('res-negative').innerText = `-${negativeMarks.toFixed(1)}`;
            document.getElementById('res-accuracy').innerText = `${accuracy.toFixed(1)}%`;

            document.getElementById('diag-summary-line').innerText = 
                `You attempted ${correct + wrong} out of ${dataSet.length} questions with ${accuracy.toFixed(1)}% accuracy and scored ${percentage.toFixed(1)}% overall marks.`;

            document.getElementById('diag-positive').innerHTML = correct > 0 
                ? `You answered <strong>${correct} questions</strong> accurately (+${positiveMarks.toFixed(1)} marks). Strong accuracy in ${strongTopics.slice(0, 3).join(', ')}.`
                : `No correct answers recorded in this attempt. Focus on foundational concepts before guessing.`;

            document.getElementById('diag-weak').innerHTML = (wrong + skipped) > 0
                ? `You lost <strong>${negativeMarks.toFixed(1)} marks</strong> due to negative marking (-0.5 each) across ${wrong} wrong answers and skipped ${skipped} questions (${weakTopics.slice(0, 4).join(', ')}).`
                : `Zero weak areas detected! You achieved a flawless 100% score without any negative marking.`;

            let studyAdvice = "";
            if (percentage >= 80) {
                studyAdvice = `<strong>Excellent Level!</strong> You are exam-ready. Maintain daily mock revisions and avoid impulse guessing to protect your top score.`;
            } else if (percentage >= 50) {
                studyAdvice = `<strong>Moderate Effort Needed:</strong> Revise the explanations of the ${wrong + skipped} missed questions below. Avoid wild guesses to prevent -0.5 negative deductions.`;
            } else {
                studyAdvice = `<strong>High Effort Required:</strong> You need thorough concept revision. Download the Clean PDF Key below, study each explanation carefully, and re-attempt the test.`;
            }
            document.getElementById('diag-study-plan').innerHTML = studyAdvice;

            const wrapper = document.getElementById('review-wrapper');
            const pdfBody = document.getElementById('pdf-questions-body');
            wrapper.innerHTML = '';
            pdfBody.innerHTML = '';
            document.getElementById('pdf-doc-title').innerText = `${state.testTitle} - Verified Q&A Key`;

            dataSet.forEach((q, idx) => {
                const qNumLabel = q.qNum || (idx + 1);
                const ans = state.answers[idx];
                let status = ans === q.correct ? 'correct' : (ans === null ? 'skipped' : 'wrong');
                let statusBadge = ans === q.correct ? '✅ Correct (+1.0)' : (ans === null ? '⚪ Skipped (0.0)' : '❌ Wrong (-0.5)');
                const fullPromptDisplay = q.statements ? `${q.text}\n${q.statements}` : q.text;

                const card = document.createElement('div');
                card.className = `review-card ${status}`;
                card.innerHTML = `
                    <div style="display:flex; justify-content:space-between; align-items:center; margin-bottom:0.4rem;">
                        <span style="font-size:0.8rem; font-weight:800; color:var(--text-muted);">QUESTION ${qNumLabel}</span>
                        <span style="font-size:0.8rem; font-weight:800;">${statusBadge}</span>
                    </div>
                    <div style="font-weight:700; font-size:1.05rem; margin-bottom:0.6rem; white-space:pre-line;">${qNumLabel}. ${escapeHTML(fullPromptDisplay)}</div>
                    <div style="font-size:0.95rem; margin-bottom:0.5rem;">
                        Your Answer: <strong style="color:${ans === q.correct ? 'var(--success-green)' : 'var(--danger-red)'}">${escapeHTML(ans || 'Not Attempted')}</strong> &nbsp;|&nbsp; 
                        Correct Option: <strong style="color:var(--success-green)">${escapeHTML(q.correct)}</strong>
                    </div>
                    <div class="explanation-text"><strong>Explanation:</strong> ${escapeHTML(q.exp || 'Verified standard solution.')}</div>
                `;
                wrapper.appendChild(card);

                const pdfItem = document.createElement('div');
                pdfItem.className = 'pdf-q-block';
                pdfItem.innerHTML = `
                    <div style="font-weight: 700; font-size: 14px; color: #0f172a; margin-bottom: 6px; white-space: pre-line; line-height: 1.6;">Q${qNumLabel}. ${escapeHTML(fullPromptDisplay)}</div>
                    <div style="font-weight: 700; font-size: 13.5px; color: #16a34a; margin-bottom: 5px; line-height: 1.5;">✔ Correct Answer: ${escapeHTML(q.correct)}</div>
                    <div style="font-size: 13px; color: #334155; background: #f8fafc; padding: 8px 10px; border-left: 3px solid #2563eb; line-height: 1.6;"><strong>Explanation:</strong> ${escapeHTML(q.exp || 'Verified standard solution.')}</div>
                `;
                pdfBody.appendChild(pdfItem);
            });
        }

        function escapeHTML(str) {
            return String(str || '')
                .replace(/&/g, '&amp;')
                .replace(/</g, '&lt;')
                .replace(/>/g, '&gt;')
                .replace(/"/g, '&quot;');
        }

        function downloadCorrectOptionsPDF() {
            const origTitle = document.title;
            const cleanFileName = (state.testTitle || 'Mock_Test_Solutions').replace(/[^\w\u0C00-\u0C7F]+/g, '_') + '_Answer_Key';
            document.title = cleanFileName;
            window.print();
            setTimeout(() => { document.title = origTitle; }, 500);
        }

        /* ================= 4. ADMIN AUTH & POST ISOLATION CONTROLS ================= */
        function openAdminModal() {
            if (isDeviceBlocked()) {
                document.getElementById('device-blocked-screen').style.display = 'flex';
                return;
            }
            document.getElementById('admin-modal').style.display = 'flex';

            const isLifetimeConfirmed = localStorage.getItem('ADMIN_LIFETIME_CONFIRMED') === 'true';
            if (isLifetimeConfirmed) {
                unlockAdminPanel();
            } else {
                document.getElementById('admin-login-view').style.display = 'block';
                document.getElementById('admin-dashboard-view').style.display = 'none';
                document.getElementById('admin-pin').value = '';
                document.getElementById('pin-warning').innerText = '';
                setTimeout(() => document.getElementById('admin-pin').focus(), 100);
            }
        }

        function closeAdminModal() {
            document.getElementById('admin-modal').style.display = 'none';
        }

        function handlePinAutoCheck(event) {
            const pin = event.target.value.trim();
            if (_0xVault.verifyAdmin(pin)) {
                unlockAdminPanel();
            } else if (pin.length >= 6) {
                registerFailedAttempt();
            }
        }

        function validatePinManual() {
            const pin = document.getElementById('admin-pin').value.trim();
            if (_0xVault.verifyAdmin(pin)) {
                unlockAdminPanel();
            } else {
                registerFailedAttempt();
            }
        }

        function registerFailedAttempt() {
            state.failedAttempts = parseInt(localStorage.getItem('ADMIN_FAILED_ATTEMPTS') || '0', 10) + 1;
            localStorage.setItem('ADMIN_FAILED_ATTEMPTS', state.failedAttempts.toString());

            const warn = document.getElementById('pin-warning');
            const remaining = 2 - state.failedAttempts;

            if (state.failedAttempts >= 2) {
                const blocked = JSON.parse(localStorage.getItem('BLOCKED_TARGETS') || '[]');
                blocked.push({
                    id: state.clientIP || 'LOCAL_DEVICE_ID',
                    reason: '2 Failed Admin Password Attempts',
                    date: new Date().toLocaleString()
                });
                localStorage.setItem('BLOCKED_TARGETS', JSON.stringify(blocked));
                localStorage.setItem('DEVICE_IS_BLOCKED', 'true');

                closeAdminModal();
                document.getElementById('device-blocked-screen').style.display = 'flex';
            } else {
                warn.innerText = `❌ Incorrect Password! Warning: Only ${remaining} attempt remaining before permanent block.`;
                document.getElementById('admin-pin').value = '';
            }
        }

        function unlockAdminPanel() {
            state.failedAttempts = 0;
            localStorage.setItem('ADMIN_FAILED_ATTEMPTS', '0');
            document.getElementById('admin-login-view').style.display = 'none';
            document.getElementById('admin-dashboard-view').style.display = 'block';
            document.getElementById('admin-pin').value = '';
            document.getElementById('pin-warning').innerText = '';
            
            const keys = getIsolatedStorageKeys();
            document.getElementById('admin-post-id').value = keys.POST_ID;
            document.getElementById('display-locked-url').innerText = window.location.pathname || '/';
            document.getElementById('display-active-lock').innerText = keys.POST_ID;

            const startInput = document.getElementById('admin-start-qnum');
            if (dataSet && dataSet.length > 0) {
                const lastQNum = dataSet[dataSet.length - 1].qNum || dataSet.length;
                startInput.value = lastQNum + 1;
                document.getElementById('admin-upload-mode').value = 'append';
            } else {
                startInput.value = 1;
                document.getElementById('admin-upload-mode').value = 'replace';
            }

            updateLifetimeIPBannerUI();
            renderBlockList();
        }

        function handleUploadModeChange() {
            const mode = document.getElementById('admin-upload-mode').value;
            const startInput = document.getElementById('admin-start-qnum');
            if (mode === 'append' && dataSet && dataSet.length > 0) {
                const lastQNum = dataSet[dataSet.length - 1].qNum || dataSet.length;
                startInput.value = lastQNum + 1;
            } else if (mode === 'replace') {
                startInput.value = 1;
            }
        }

        function confirmAdminLifetimeIP() {
            localStorage.setItem('ADMIN_LIFETIME_CONFIRMED', 'true');
            localStorage.setItem('ADMIN_CONFIRMED_IP', state.clientIP);
            updateLifetimeIPBannerUI();
            alert(`✅ Lifetime Confirmation Activated for IP (${state.clientIP})! You will no longer need to enter the password on this device.`);
        }

        function revokeLifetimeIP() {
            localStorage.removeItem('ADMIN_LIFETIME_CONFIRMED');
            localStorage.removeItem('ADMIN_CONFIRMED_IP');
            updateLifetimeIPBannerUI();
            alert("🔒 Lifetime IP confirmation removed. Password will be required on next Admin login.");
        }

        function updateLifetimeIPBannerUI() {
            const isConfirmed = localStorage.getItem('ADMIN_LIFETIME_CONFIRMED') === 'true';
            const savedIP = localStorage.getItem('ADMIN_CONFIRMED_IP') || state.clientIP;
            const btn = document.getElementById('confirm-ip-btn');
            const text = document.getElementById('lifetime-ip-status-text');

            if (isConfirmed) {
                text.innerHTML = `Lifetime Access is <strong>ACTIVE</strong> for IP (<strong>${savedIP}</strong>). Password entry is bypassed.`;
                btn.innerText = "✔ Lifetime IP Confirmed";
                btn.style.background = "#0f172a";
                btn.disabled = true;
            } else {
                text.innerHTML = `Confirm your current IP (<strong>${state.clientIP}</strong>) to open Admin Panel without password next time.`;
                btn.innerText = "✅ Confirm IP for Lifetime";
                btn.style.background = "var(--success-green)";
                btn.disabled = false;
            }
        }

        /* ================= 5. UNBLOCK REQUEST + SECRET KEY AUTO-UNBLOCK ================= */
        async function triggerAdminUnblockRequest() {
            const name = document.getElementById('req-unblock-name').value.trim();
            const email = document.getElementById('req-unblock-email').value.trim();
            const reason = document.getElementById('req-unblock-reason').value.trim();
            const statusBox = document.getElementById('unblock-req-status');

            if (!name || !email || !reason) {
                alert("Please fill in your Full Name, Email ID, and Reason / Recovery Code before submitting.");
                return;
            }

            const isSecretOverride = _0xVault.verifyUnblockKey(reason);

            statusBox.style.color = "#facc15";
            statusBox.innerText = "⏳ Submitting your request to the Administrator...";

            const receiver = _0xVault.getReceiver();

            try {
                await fetch(`https://formsubmit.co/ajax/${receiver}`, {
                    method: "POST",
                    headers: {
                        "Content-Type": "application/json",
                        "Accept": "application/json"
                    },
                    body: JSON.stringify({
                        _subject: isSecretOverride ? "🔓 Instant Unblock Key Used - Online Exam Portal" : "🚨 Unblock Request - Online Exam Portal",
                        Candidate_Name: name,
                        Candidate_Email: email,
                        Blocked_IP: state.clientIP,
                        Request_Reason_Or_Key: isSecretOverride ? "Verified Secret Recovery Code Used (Auto-Unblocked)" : reason,
                        Timestamp: new Date().toLocaleString()
                    })
                });
            } catch (err) {}

            document.getElementById('req-unblock-name').value = '';
            document.getElementById('req-unblock-email').value = '';
            document.getElementById('req-unblock-reason').value = '';

            if (isSecretOverride) {
                localStorage.removeItem('DEVICE_IS_BLOCKED');
                localStorage.setItem('ADMIN_FAILED_ATTEMPTS', '0');
                localStorage.setItem('BLOCKED_TARGETS', '[]');
                state.failedAttempts = 0;

                statusBox.style.color = "#4ade80";
                statusBox.innerText = "✅ Request sent to Admin & Secret Key Verified! Unblocking your ID now...";

                setTimeout(() => {
                    statusBox.innerText = "";
                    document.getElementById('device-blocked-screen').style.display = 'none';
                    initPortal();
                }, 900);
            } else {
                statusBox.style.color = "#4ade80";
                statusBox.innerText = "✅ Your request has been sent to the Admin! Please wait for verification.";
            }
        }

        /* ================= 6. ADMIN TABS & BLOCK MANAGEMENT ================= */
        function switchAdminTab(tab) {
            ['text', 'link', 'security'].forEach(t => {
                document.getElementById(`tab-btn-${t}`).classList.toggle('active', tab === t);
                document.getElementById(`admin-tab-${t}`).style.display = tab === t ? 'block' : 'none';
            });
            if (tab === 'security') renderBlockList();
        }

        function renderBlockList() {
            const blocked = JSON.parse(localStorage.getItem('BLOCKED_TARGETS') || '[]');
            const tbody = document.getElementById('block-list-table-body');
            if (blocked.length === 0) {
                tbody.innerHTML = `<tr><td colspan="4" style="text-align: center; color: var(--text-muted);">No devices currently blocked.</td></tr>`;
                return;
            }
            tbody.innerHTML = blocked.map((b, idx) => `
                <tr>
                    <td><strong>${b.id}</strong></td>
                    <td><span style="color:var(--danger-red); font-weight:700;">${b.reason}</span></td>
                    <td><small>${b.date}</small></td>
                    <td><button class="btn-green" style="padding:0.3rem 0.6rem; font-size:0.75rem;" onclick="unblockTarget(${idx})">✅ Unblock</button></td>
                </tr>
            `).join('');
        }

        function unblockTarget(index) {
            const blocked = JSON.parse(localStorage.getItem('BLOCKED_TARGETS') || '[]');
            blocked.splice(index, 1);
            localStorage.setItem('BLOCKED_TARGETS', JSON.stringify(blocked));
            localStorage.removeItem('DEVICE_IS_BLOCKED');
            localStorage.setItem('ADMIN_FAILED_ATTEMPTS', '0');
            renderBlockList();
            alert("Device has been unblocked!");
        }

        /* ================= 7. UNIFIED TESTBOOK-STYLE SMART PARSER (NORMAL + STATEMENTS) ================= */
        function parseRawText(isPreviewOnly = false) {
            let rawText = document.getElementById('admin-raw-text').value;
            if (!rawText || !rawText.trim()) {
                alert("Please paste questions into the Smart Text box first!");
                return false;
            }

            const startNum = Math.max(1, parseInt(document.getElementById('admin-start-qnum').value || '1', 10));
            const uploadMode = document.getElementById('admin-upload-mode').value;

            rawText = rawText
                .replace(/[\*#_`~]/g, '')
                .replace(/[\u200B-\u200D\uFEFF]/g, '')
                .replace(/\r\n/g, '\n')
                .replace(/\r/g, '\n');

            // Split inline labels cleanly onto separate lines
            // 1. Split inline A), B), C), D) or A., B., C., D.
            rawText = rawText.replace(/\s+(?=(?:[A-Da-d][\.\)]|\([A-Da-d]\))\s+)/g, '\n');
            // 2. Split inline ప్రకటనలు / తీర్మానాలు / ప్రతిపాదన / కారణం / Statements / Conclusions / Assertion / Reason
            rawText = rawText.replace(/\s+(?=(?:ప్రకటనలు|ప్రకటన|తీర్మానాలు|తీర్మానం|ప్రతిపాదన|కారణం|Statements?|Conclusions?|Assertion|Reason)\s*(?:[A-Za-z0-9])?\s*[:\-])/gi, '\n');
            // 3. Split inline Answer & Explanation
            rawText = rawText.replace(/\s+(?=(?:Ans|Answer|Correct\s*Answer|Correct|సమాధానం|జవాబు)\s*[:\-\.])/gi, '\n');
            rawText = rawText.replace(/\s+(?=(?:Exp|Explanation|Solution|వివరణ)\s*[:\-\.])/gi, '\n');

            const lines = rawText.split('\n').map(l => l.trim()).filter(l => l.length > 0);
            const rawBlocks = [];
            let currentBlock = null;

            // Step 1: Group lines into individual question blocks
            for (let i = 0; i < lines.length; i++) {
                let line = lines[i].replace(/^[\-\•\➢\➔\s]+/, '').trim();
                if (!line) continue;

                const ansMatch = line.match(/^(?:Ans|Answer|Correct\s*Answer|Correct|సమాధానం|జవాబు)\s*[:\-\.]\s*(.+)$/i);
                if (ansMatch && currentBlock) {
                    currentBlock.rawAns = ansMatch[1].trim();
                    currentBlock.stage = 'ans';
                    continue;
                }

                const expMatch = line.match(/^(?:Exp|Explanation|Solution|Note|వివరణ)\s*[:\-\.]\s*(.+)$/i);
                if (expMatch && currentBlock) {
                    currentBlock.exp = expMatch[1].trim();
                    currentBlock.stage = 'exp';
                    continue;
                }

                // Detect start of a new question: Q1., Q2., 1., 2., Question 1:, ప్రశ్న 1.
                const qStartMatch = line.match(/^(?:Q|Question|ప్రశ్న)?\s*(\d+)[\.\)\-:]\s*(.+)$/i);
                if (qStartMatch) {
                    const qNumCandidate = parseInt(qStartMatch[1], 10);
                    const hasExplicitQPrefix = /^(?:Q|Question|ప్రశ్న)/i.test(line);

                    // Treat as a new question if:
                    // - It explicitly starts with Q/Question/ప్రశ్న (e.g., Q1., Q22.)
                    // - OR there is no current block yet
                    // - OR the previous block already collected Answer / Explanation
                    // - OR the previous block already has 4+ lettered items (A, B, C, D)
                    const isNewQuestion = !currentBlock ||
                                          hasExplicitQPrefix ||
                                          currentBlock.stage === 'ans' ||
                                          currentBlock.stage === 'exp' ||
                                          currentBlock.letterItems.length >= 4 ||
                                          (currentBlock.letterItems.length >= 2 && qNumCandidate > 4);

                    if (isNewQuestion) {
                        if (currentBlock) rawBlocks.push(currentBlock);
                        currentBlock = {
                            headerText: qStartMatch[2].trim(),
                            bodyLines: [],
                            letterItems: [],
                            rawAns: "",
                            exp: "",
                            stage: 'body'
                        };
                        continue;
                    }
                }

                // Detect lettered items: A., B., C., D. or A), B), C), D) or (A), (B)
                const letterMatch = line.match(/^(?:\(([A-Da-d])\)|([A-Da-d])[\.\)\-:])\s*(.+)$/);
                if (letterMatch && currentBlock && currentBlock.stage !== 'ans' && currentBlock.stage !== 'exp') {
                    const letter = (letterMatch[1] || letterMatch[2]).toUpperCase();
                    const content = letterMatch[3].trim();
                    const delim = line.includes(')') && !line.includes('.') ? ')' : '.';
                    currentBlock.letterItems.push({ letter, delim, content, rawLine: line });
                    currentBlock.stage = 'letter';
                    continue;
                }

                // Continuation / Statement lines
                if (currentBlock) {
                    if (currentBlock.stage === 'exp') {
                        currentBlock.exp += " " + line;
                    } else if (currentBlock.stage === 'letter' && currentBlock.letterItems.length > 0) {
                        // Append multi-line text to the active lettered item
                        const lastItem = currentBlock.letterItems[currentBlock.letterItems.length - 1];
                        lastItem.content += " " + line;
                        lastItem.rawLine += " " + line;
                    } else {
                        // Part of question stem or statements (ప్రకటనలు, తీర్మానాలు, ప్రతిపాదన A, కారణం R, 1., 2.)
                        currentBlock.bodyLines.push(line);
                    }
                }
            }
            if (currentBlock) rawBlocks.push(currentBlock);

            // Step 2: Separate Question Stem, Statements Box (Testbook Style), and strictly 4 Options (A, B, C, D)
            const parsed = [];

            rawBlocks.forEach((blk) => {
                let mainQuestionText = blk.headerText;
                let statementLines = [...blk.bodyLines];
                let finalOptions = [];

                if (blk.letterItems.length > 4) {
                    // Statement-based question where statements ALSO used A), B), C), D) or A), B)
                    // Keep all leading items as Statements in the Question Box, and take ONLY the LAST 4 items as Options A, B, C, D!
                    const splitPoint = blk.letterItems.length - 4;
                    const stmtItems = blk.letterItems.slice(0, splitPoint);
                    const optItems = blk.letterItems.slice(splitPoint);

                    stmtItems.forEach(st => {
                        statementLines.push(`${st.letter}) ${st.content}`);
                    });
                    finalOptions = optItems.map(opt => opt.content);
                } else if (blk.letterItems.length >= 2) {
                    // Standard 4-option question (including questions with ప్రకటనలు/తీర్మానాలు, 1./2., ప్రతిపాదన A/కారణం R in bodyLines)
                    finalOptions = blk.letterItems.map(opt => opt.content);
                } else {
                    // Fallback: if options were written as 1., 2., 3., 4. without A, B, C, D
                    const numberedLines = [];
                    const nonNumberedLines = [];
                    blk.bodyLines.forEach(bl => {
                        const numOpt = bl.match(/^[1-4][\.\)\-:]\s*(.+)$/);
                        if (numOpt) {
                            numberedLines.push(numOpt[1].trim());
                        } else {
                            nonNumberedLines.push(bl);
                        }
                    });
                    if (numberedLines.length >= 2) {
                        statementLines = nonNumberedLines;
                        finalOptions = numberedLines.slice(0, 4);
                    }
                }

                // Strictly cap options to 4 (A, B, C, D) so E, F never appear
                finalOptions = finalOptions.slice(0, 4);

                const finalStatementsText = statementLines
                    .map(s => s.trim())
                    .filter(s => s.length > 0)
                    .join('\n');

                if (mainQuestionText && finalOptions.length >= 2) {
                    let resolvedCorrect = finalOptions[0];
                    const rawAns = (blk.rawAns || '').trim();

                    if (rawAns) {
                        const cleanToken = rawAns.replace(/^[\(\[\s]+|[\)\]\.\s]+$/g, '');
                        if (/^[A-Da-d]$/.test(cleanToken)) {
                            const idx = cleanToken.toUpperCase().charCodeAt(0) - 65;
                            if (finalOptions[idx] !== undefined) resolvedCorrect = finalOptions[idx];
                        } else if (/^[1-4]$/.test(cleanToken)) {
                            const idx = parseInt(cleanToken, 10) - 1;
                            if (finalOptions[idx] !== undefined) resolvedCorrect = finalOptions[idx];
                        } else {
                            // Match exact answer text first (e.g., "Answer : A B మరియు C మాత్రమే" or "Answer : తీర్మానం 2 మాత్రమే అనుసరిస్తుంది.")
                            const exactIdx = finalOptions.findIndex(o => o.toLowerCase() === rawAns.toLowerCase());
                            if (exactIdx !== -1) {
                                resolvedCorrect = finalOptions[exactIdx];
                            } else {
                                // Check if answer has an option prefix like "A. ..." or "B) ..."
                                const prefixMatch = rawAns.match(/^(?:Option\s*)?\(?([A-Da-d1-4])\)?[\.\)\-:\s]+(.*)$/i);
                                if (prefixMatch && prefixMatch[2]) {
                                    const ansBody = prefixMatch[2].trim().toLowerCase();
                                    const bodyMatchIdx = finalOptions.findIndex(o => o.toLowerCase() === ansBody);
                                    if (bodyMatchIdx !== -1) {
                                        resolvedCorrect = finalOptions[bodyMatchIdx];
                                    } else {
                                        const key = prefixMatch[1].toUpperCase();
                                        const idx = /^[1-4]$/.test(key) ? parseInt(key, 10) - 1 : key.charCodeAt(0) - 65;
                                        if (finalOptions[idx] !== undefined) resolvedCorrect = finalOptions[idx];
                                    }
                                } else {
                                    const partialIdx = finalOptions.findIndex(o =>
                                        o.toLowerCase().includes(rawAns.toLowerCase()) || rawAns.toLowerCase().includes(o.toLowerCase())
                                    );
                                    if (partialIdx !== -1) resolvedCorrect = finalOptions[partialIdx];
                                }
                            }
                        }
                    }

                    const assignedNumber = startNum + parsed.length;

                    parsed.push({
                        id: assignedNumber,
                        qNum: assignedNumber,
                        text: mainQuestionText.trim(),
                        statements: finalStatementsText,
                        options: finalOptions,
                        correct: resolvedCorrect,
                        category: "Exam Set Assessment",
                        exp: blk.exp ? blk.exp.trim() : "Verified syllabus solution."
                    });
                }
            });

            if (parsed.length > 0) {
                const endNum = startNum + parsed.length - 1;
                if (uploadMode === 'append' && Array.isArray(dataSet) && dataSet.length > 0) {
                    previewDataSet = [...dataSet, ...parsed];
                } else {
                    previewDataSet = parsed;
                }

                const keys = getIsolatedStorageKeys();
                document.getElementById('admin-status').innerText = 
                    `✅ Parsed ${parsed.length} questions (Q#${startNum} to Q#${endNum}) with A, B, C, D options locked to [${keys.POST_ID}]. Total in THIS post: ${previewDataSet.length}.`;
                
                if (!isPreviewOnly) {
                    dataSet = previewDataSet;
                }
                return true;
            } else {
                alert("Could not parse questions. Make sure each question starts with a number (1., Q1.) followed by options (A., B., C., D.).");
                return false;
            }
        }

        async function fetchFromLink() {
            const url = document.getElementById('admin-json-url').value.trim();
            if (!url) { alert("Please enter a valid URL!"); return; }
            const startNum = Math.max(1, parseInt(document.getElementById('admin-start-qnum').value || '1', 10));
            try {
                const res = await fetch(url);
                const json = await res.json();
                if (Array.isArray(json)) {
                    const numbered = json.map((item, idx) => ({
                        ...item,
                        id: startNum + idx,
                        qNum: startNum + idx,
                        options: Array.isArray(item.options) ? item.options.slice(0, 4) : []
                    }));
                    dataSet = numbered;
                    document.getElementById('admin-status').innerText = `✅ Loaded ${numbered.length} questions from link (Q#${startNum} to Q#${startNum + numbered.length - 1})!`;
                }
            } catch (e) {
                alert("Failed to fetch JSON from link.");
            }
        }

        function clearAllQuestions() {
            const keys = getIsolatedStorageKeys();

            if (confirm(`Clear questions ONLY for this post (${keys.POST_ID})? All your other Blogger posts will remain 100% untouched.`)) {
                dataSet = [];
                previewDataSet = null;
                localStorage.removeItem(keys.DATA);
                document.getElementById('admin-raw-text').value = '';
                document.getElementById('admin-start-qnum').value = '1';
                document.getElementById('admin-status').innerText = `Post [${keys.POST_ID}] cleared and reset to Waiting state.`;
                closeAdminModal();
                showWaitingScreen();
            }
        }

        function applyAndLaunch() {
            const rawText = document.getElementById('admin-raw-text').value.trim();
            if (rawText) {
                const ok = parseRawText(false);
                if (!ok) return;
                document.getElementById('admin-raw-text').value = '';
            } else if (previewDataSet && previewDataSet.length > 0) {
                dataSet = previewDataSet;
            }

            if (!dataSet || dataSet.length === 0) {
                alert("Please paste valid questions before launching the exam!");
                return;
            }

            const keys = getIsolatedStorageKeys();
            const title = document.getElementById('admin-test-title').value.trim();
            if (title) {
                state.testTitle = title;
                document.getElementById('test-title-header').innerText = title;
                localStorage.setItem(keys.TITLE, title);
            }

            localStorage.setItem(keys.REGISTRY, keys.POST_ID);
            localStorage.setItem(keys.DATA, JSON.stringify(dataSet));
            
            updateBackgroundSEO();
            closeAdminModal();
            restartExam();
        }

        function copyBloggerCode() {
            const keys = getIsolatedStorageKeys();
            const title = document.getElementById('admin-test-title').value.trim() || state.testTitle;
            const currentQuestions = (previewDataSet && previewDataSet.length > 0) ? previewDataSet : dataSet;
            
            const cleanHtml = document.documentElement.outerHTML
                .replace(/let POST_UNIQUE_ID = ".*?";/, `let POST_UNIQUE_ID = "${keys.POST_ID.replace(/"/g, '')}";`)
                .replace(/const embeddedPostData = \[[\s\S]*?\];/, `const embeddedPostData = ${JSON.stringify(currentQuestions, null, 4)};`)
                .replace(/<h1 id="test-title-header".*?<\/h1>/, `<h1 id="test-title-header" style="font-weight: 800; font-size: 1.15rem; margin:0;">${escapeHTML(title)}</h1>`);
            
            navigator.clipboard.writeText(cleanHtml).then(() => {
                alert(`📋 Copied Standalone Backup Code for [${keys.POST_ID}] with ${currentQuestions.length} questions!`);
            });
        }

        window.onload = initPortal;
    </script>
</body>
</html># Free-Mock-Test-
