# JHA.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Daily Hazard Assessment</title>
    <script src="https://cdn.jsdelivr.net/npm/signature_pad@4.1.7/dist/signature_pad.umd.min.js"></script>

    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-title" content="Hazard App">
    <link rel="apple-touch-icon" href="https://via.placeholder.com/180/000000/ffffff?text=Hazard">

    <style>
        :root { --primary-bg: #ffffff; --input-bg: #f4f4f7; --border-color: #000000; }
        body { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Arial, sans-serif; margin: 0; padding: 0; background-color: #f0f0f5; color: #000000; }
        .red-text { color: #D32F2F; }
        .app-container { padding: calc(15px + env(safe-area-inset-top)) 12px calc(80px + env(safe-area-inset-bottom)) 12px; max-width: 800px; margin: 0 auto; }
        .document-canvas { background: var(--primary-bg); padding: 20px; border: 2px solid #000; border-radius: 4px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); box-sizing: border-box; line-height: 1.2; font-size: 12px; }
        
        input[type="checkbox"] {
            -webkit-appearance: none; appearance: none;
            border: 1px solid #000; cursor: pointer;
            display: inline-block; position: relative;
            width: 12px; height: 12px; vertical-align: middle;
        }
        input[type="checkbox"]:checked::after {
            content: "✕"; position: absolute;
            top: 50%; left: 50%; transform: translate(-50%, -50%);
            font-size: 10px; font-weight: bold; color: #000;
        }

        .header-border-group { border: 1px solid #000; padding: 10px; margin-bottom: 12px; display: inline-block; width: 100%; box-sizing: border-box; }
        .doc-header { text-align: center; margin-bottom: 8px; position: relative; min-height: 30px; }
        .doc-header h1 { font-size: 18px; font-weight: 900; text-transform: uppercase; margin: 0; letter-spacing: 0.5px; }
        
        .logo-container { position: absolute; top: 0; right: 0; }
        .logo-container img { height: 40px; width: auto; }
        
        .type-selector-row { display: flex; justify-content: center; gap: 15px; margin: 0; font-weight: bold; font-size: 10px; }
        .type-item { display: flex; align-items: center; font-size: 10px; }
        .type-item input[type="checkbox"] { width: 12px; height: 12px; margin-right: 4px; }
        
        .grid-table { width: 100%; border-collapse: collapse; margin-bottom: 10px; }
        .grid-table td { border: none; padding: 5px 6px; vertical-align: middle; }
        
        .task-table { border: 1px solid var(--border-color); }
        .task-table td, .task-table th { border: 1px solid var(--border-color); }
        
        .section-banner { background-color: #e5e5ea; font-weight: bold; text-transform: uppercase; font-size: 12px; padding: 5px 6px; border: 1px solid #000; border-bottom: none; }
        
        /* Unified input styling for perfect vertical alignment */
        input[type="text"], input[type="date"], textarea { width: 100%; border: none; background: var(--input-bg); box-sizing: border-box; font-size: 12px; padding: 4px; color: #000; font-family: inherit; }
        .perfect-input { height: 18px !important; padding: 2px !important; vertical-align: middle; margin: 0 !important; }
        
        .check-cell-content { display: flex; align-items: center; width: 100%; }
        .check-cell-content input[type="checkbox"] { width: 16px; height: 16px; margin-right: 6px; flex-shrink: 0; }
        .check-label { font-size: 11px; white-space: nowrap; }
        
        .hz-check { width: 10px; height: 10px; margin: 0 auto; display: block; cursor: pointer; }
        .hz-table { font-size: 8px !important; }
        .hz-table th, .hz-table td { padding: 2px !important; }

        .task-table td { padding: 1px !important; }
        .task-table textarea, .task-table input { font-size: 9px !important; padding: 2px !important; margin: 0; }
        
        .sig-pad { border: 1px solid #000; width: 100%; height: 60px; background: #fafafa; touch-action: none; margin-top: 5px; }
        .floating-action-panel { position: fixed; bottom: 0; left: 0; right: 0; background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(15px); padding: 12px 16px calc(12px + env(safe-area-inset-bottom)) 16px; border-top: 1px solid #c6c6c8; z-index: 9999; }
        .action-btn { background-color: #007aff; color: #ffffff; font-size: 16px; font-weight: 600; border: none; border-radius: 10px; padding: 14px; width: 100%; box-shadow: 0 4px 10px rgba(0,122,255,0.25); }
        
        @media print { 
            @page { size: portrait; margin: 0.15in; }
            body { background: #ffffff; color: #000000; overflow: hidden; } 
            .app-container { padding: 0 !important; margin: 0 !important; width: 100% !important; } 
            .document-canvas { 
                box-shadow: none !important; 
                padding: 10px !important; 
                transform: scale(0.85); 
                transform-origin: top left; 
                width: 115%; 
                break-inside: avoid; 
                page-break-after: avoid;
                border: 2px solid #000;
            }
            .hz-table td:nth-child(1), .hz-table td:nth-child(2), 
            .hz-table td:nth-child(4), .hz-table td:nth-child(5),
            .hz-table td:nth-child(7), .hz-table td:nth-child(8) {
                padding: 0px !important;
                width: 15px !important;
                text-align: center;
            }
            .floating-action-panel, .clear-btn { display: none !important; } 
            input[type="text"], input[type="date"], textarea { background: transparent !important; border-bottom: 1px solid #000 !important; padding: 1px 0 !important; } 
            textarea { overflow: visible; height: auto !important; }
            .section-banner { border: 1px solid #000 !important; }
        }
    </style>
</head>
<body>

<div class="app-container">
    <div class="document-canvas" id="pdfDocument">
        
        <div class="doc-header">
            <div class="logo-container">
                <img src="https://i.postimg.cc/yYx2tzBL/IMG-7182.webp" alt="Company Logo">
            </div>
            <h1>DAILY HAZARD ASSESSMENT</h1> 
        </div>

        <div class="header-border-group">
            <div class="type-selector-row">
                <div class="type-item"><input type="checkbox" id="preHazard"> <span class="red-text">Pre-Hazard Assessment</span> </div>
                <div class="type-item"><input type="checkbox" id="dailyInspect"> <span class="red-text">Daily Inspection</span> </div>
            </div>
        </div>

        <table class="grid-table">
            <tr>
                <td style="width: 15%; font-weight: bold;">Company Name:</td> 
                <td style="width: 35%;"><input type="text"></td>
                <td style="width: 12%; font-weight: bold;">Location:</td> 
                <td style="width: 38%;"><input type="text" placeholder="Highway #, Rte #, Mile Marker, Road, Street, Closest Civic address, etc."> </td>
            </tr>
            <tr>
                <td style="font-weight: bold;">Foreman:</td> <td><input type="text"></td>
                <td style="font-weight: bold;">Safety Rep:</td> <td><input type="text"></td>
            </tr>
        </table>

        <div class="section-banner red-text">Pre-Start Checklist</div> 
        <table class="grid-table">
            <tr>
                <td style="width: 50%; font-size: 10px; vertical-align: middle;"><strong class="red-text">Completed By:</strong> <input type="text" class="perfect-input" style="width:60%; display:inline-block;"></td> 
                <td style="width: 50%; font-size: 10px; vertical-align: middle;"><strong class="red-text">Date:</strong> <input type="date" class="perfect-input" style="width:75%; display:inline-block;"></td> 
            </tr>
        </table>

        <table class="grid-table" style="margin-top: -11px;">
            <tr>
                <td style="width: 33%; padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Traffic Control</span></div> </td>
                <td style="width: 33%; padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Sub-Contractor</span></div> </td>
                <td style="width: 33%; padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">PPE Reqs</span></div> </td>
            </tr>
            <tr>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Revolving lights</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Black Bag</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Overhead Wires</span></div> </td>
            </tr>
            <tr>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">SDS Sheets</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Comm. Device</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Water Course</span></div> </td>
            </tr>
            <tr>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Fire Ext.</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">First Aid</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">SWP/SJP</span></div> </td>
            </tr>
            <tr>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Sanitation</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content"><input type="checkbox" style="width:10px; height:10px;"><span class="check-label" style="font-size: 8px;">Permits</span></div> </td>
                <td style="padding: 1px 2px;"><div class="check-cell-content" style="gap:4px;"><span class="check-label" style="font-size: 8px;"><strong>Other:</strong></span> <input type="text" style="padding: 2px;"></div> </td>
            </tr>
            <tr>
                <td colspan="3" style="text-align: center; font-style: italic; font-size: 10px; padding: 4px;"><span class="red-text">Note: If any items are missing, correct prior to startup.</span> </td>
            </tr>
        </table>

        <div class="section-banner red-text">Hazard/Inspection Checklist</div> 
        <table class="grid-table">
            <tr>
                <td style="width: 50%; font-size: 10px; vertical-align: middle;"><strong class="red-text">Completed By:</strong> <input type="text" class="perfect-input" style="width:60%; display:inline-block;"></td> 
                <td style="width: 50%; font-size: 10px; vertical-align: middle;"><strong class="red-text">Date:</strong> <input type="date" class="perfect-input" style="width:75%; display:inline-block;"></td> 
            </tr>
        </table>

        <table class="grid-table hz-table" style="margin-top: -11px; text-align: left;">
            <thead>
                <tr style="background-color: #fafafa; font-weight: bold;">
                    <th>OK</th><th>Fix</th><th>Item</th><th>OK</th><th>Fix</th><th>Item</th><th>OK</th><th>Fix</th><th>Item</th>
                </tr>
            </thead>
            <tbody>
                <tr><td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Emerg. Resp</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Guards</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>PPE</td></tr>
                <tr><td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Lockout</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Tools</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Alarms</td></tr>
                <tr><td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Haz. Storage</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Power Lines</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Fire Ext.</td></tr>
                <tr><td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Housekeep.</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Access</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Ladders</td></tr>
                <tr><td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Heavy Equip</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Manual Hand</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Noise</td></tr>
                <tr><td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Traffic Cntrl</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Grounds</td> <td><input type="checkbox" class="hz-check"></td><td><input type="checkbox" class="hz-check"></td><td>Other</td></tr>
            </tbody>
        </table>

        <div style="margin: 5px 0 10px 0;"><input type="text" placeholder="Notes/Additional Hazards..." style="border-bottom: 1px solid #000 !important; background: transparent;"></div>

        <div style="text-align: center; margin-top: 5px; margin-bottom: 2px; font-weight: bold; font-size: 9px;"><span class="red-text">Identify the task and rank hazards, and then identify the plans to eliminate or control the hazard</span> <br><span class="red-text" style="font-size: 8px;">Rank Matrix System: 1-Immediate danger, 2-Serious injury, 3-Minor, 4-Negligible, 5-Not applicable &bull; A-Likely, B-Probable, C-Possible, D-Unlikely </span></div>
        
        <table class="grid-table task-table" style="font-size: 9px;">
            <thead>
                <tr style="background-color: #e5e5ea; font-weight: bold; text-align: center;">
                    <th style="padding: 2px; width: 22%;">Task</th> <th style="padding: 2px; width: 22%;">Hazard</th> <th style="padding: 2px; width: 10%;">Rank</th> <th style="padding: 2px; width: 24%;">Control(s)</th> <th style="padding: 2px; width: 11%;">Date</th> <th style="padding: 2px; width: 11%;">By Whom</th> 
                </tr>
            </thead>
            <tbody>
                <tr><td><textarea rows="1"></textarea></td><td><textarea rows="1"></textarea></td><td><input type="text" style="text-align:center;"></td><td><textarea rows="1"></textarea></td><td><input type="date"></td><td><input type="text"></td></tr>
                <tr><td><textarea rows="1"></textarea></td><td><textarea rows="1"></textarea></td><td><input type="text" style="text-align:center;"></td><td><textarea rows="1"></textarea></td><td><input type="date"></td><td><input type="text"></td></tr>
                <tr><td><textarea rows="1"></textarea></td><td><textarea rows="1"></textarea></td><td><input type="text" style="text-align:center;"></td><td><textarea rows="1"></textarea></td><td><input type="date"></td><td><input type="text"></td></tr>
            </tbody>
        </table>
        
        <table class="grid-table">
            <tr>
                <td style="width: 25%;"><strong class="red-text">Ambulance:</strong> <input type="text" value="911" style="width:60%; display:inline-block;"></td>
                <td style="width: 25%;"><strong class="red-text">Fire:</strong> <input type="text" value="911" style="width:60%; display:inline-block;"></td>
                <td style="width: 25%;"><strong class="red-text">Medical:</strong> <input type="text" style="width:60%; display:inline-block;"></td>
                <td style="width: 25%;"><strong class="red-text">Police:</strong> <input type="text" value="911" style="width:60%; display:inline-block;"></td>
            </tr>
        </table>
        <table class="grid-table" style="margin-top: -11px;">
            <tr>
                <td colspan="2"><strong>Comments:</strong> <textarea rows="2" style="margin-top: 4px;"></textarea></td>
            </tr>
            <tr>
                <td style="width: 50%; vertical-align: top; padding-bottom: 15px;">
                    <strong>Employee Signatures:</strong> 
                    <canvas class="sig-pad"></canvas>
                    <button type="button" class="clear-btn" onclick="clearSig()" style="font-size: 10px; cursor: pointer; display: block; margin-top: 2px;">Clear Signature</button>
                </td>
                <td style="width: 50%; vertical-align: top;">
                    <div style="margin-bottom: 12px;"><strong class="red-text">Date Reviewed with crew:</strong> <input type="date" style="width: 50%; display: inline-block; background: var(--input-bg);"></div>
                    <div><strong class="red-text">First Aid Attendant:</strong> <input type="text" style="width: 55%; display: inline-block; background: var(--input-bg);"></div>
                </td>
            </tr>
        </table>
    </div>
</div>

<div class="floating-action-panel">
    <button type="button" class="action-btn" onclick="executeNativePrint()">Generate Form PDF</button>
</div>

<script>
    const canvas = document.querySelector(".sig-pad");
    const signaturePad = new SignaturePad(canvas);
    function clearSig() { signaturePad.clear(); }
    function executeNativePrint() { window.print(); }
</script>

</body>
</html>
