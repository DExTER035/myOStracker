<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>LifeOS Student</title>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.2.0/umd/react.production.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.2.0/umd/react-dom.production.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/7.23.2/babel.min.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;0,9..40,700;1,9..40,400&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet"/>
  <style>
    /* ── CSS Reset & Variables ─────────────────────────────────── */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --mint:    #6EE7B7;
      --indigo:  #818cf8;
      --pink:    #f472b6;
      --amber:   #fbbf24;
      --sky:     #38bdf8;
      --red:     #f87171;
      --green:   #34d399;
      --orange:  #fb923c;

      /* Dark theme defaults */
      --bg:        #0c0f1a;
      --bg2:       #111827;
      --bg3:       #1a2235;
      --card:      #131b2e;
      --border:    rgba(255,255,255,0.07);
      --border2:   rgba(255,255,255,0.12);
      --text:      #e8edf5;
      --text2:     #94a3b8;
      --text3:     #64748b;
      --shadow:    0 4px 24px rgba(0,0,0,0.4);
      --shadow-lg: 0 8px 40px rgba(0,0,0,0.5);
      --glass:     rgba(255,255,255,0.03);
      --glass2:    rgba(255,255,255,0.06);
    }

    [data-theme="light"] {
      --bg:        #f1f5fb;
      --bg2:       #e8edf8;
      --bg3:       #dde4f0;
      --card:      #ffffff;
      --border:    rgba(0,0,0,0.07);
      --border2:   rgba(0,0,0,0.12);
      --text:      #0f172a;
      --text2:     #475569;
      --text3:     #94a3b8;
      --shadow:    0 4px 24px rgba(0,0,0,0.08);
      --shadow-lg: 0 8px 40px rgba(0,0,0,0.12);
      --glass:     rgba(255,255,255,0.6);
      --glass2:    rgba(255,255,255,0.8);
    }

    html { font-size: 15px; }
    body {
      font-family: 'DM Sans', system-ui, sans-serif;
      background: var(--bg);
      color: var(--text);
      min-height: 100vh;
      overflow-x: hidden;
      transition: background 0.3s, color 0.3s;
    }

    /* ── Scrollbar ──────────────────────────────────────────────── */
    ::-webkit-scrollbar { width: 5px; height: 5px; }
    ::-webkit-scrollbar-track { background: transparent; }
    ::-webkit-scrollbar-thumb { background: var(--border2); border-radius: 99px; }

    /* ── Animations ─────────────────────────────────────────────── */
    @keyframes fadeUp   { from { opacity:0; transform:translateY(16px); } to { opacity:1; transform:translateY(0); } }
    @keyframes slideIn  { from { opacity:0; transform:translateX(24px); } to { opacity:1; transform:translateX(0); } }
    @keyframes pulse    { 0%,100% { opacity:1; } 50% { opacity:.5; } }
    @keyframes spin     { to { transform: rotate(360deg); } }
    @keyframes shimmer  { from { background-position:-400px 0; } to { background-position:400px 0; } }
    @keyframes popIn    { 0% { transform:scale(0.8); opacity:0; } 60% { transform:scale(1.05); } 100% { transform:scale(1); opacity:1; } }
    @keyframes timerPulse { 0%,100% { text-shadow: 0 0 0 transparent; } 50% { text-shadow: 0 0 20px rgba(110,231,183,0.4); } }

    .fade-up   { animation: fadeUp  0.4s ease both; }
    .slide-in  { animation: slideIn 0.3s ease both; }
    .pop-in    { animation: popIn   0.35s ease both; }

    /* ── Layout ─────────────────────────────────────────────────── */
    #app { display: flex; flex-direction: column; min-height: 100vh; }

    .app-layout { display: flex; flex: 1; overflow: hidden; height: calc(100vh - 60px); }

    /* ── Sidebar ────────────────────────────────────────────────── */
    .sidebar {
      width: 64px;
      background: var(--card);
      border-right: 1px solid var(--border);
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 12px 0;
      gap: 4px;
      flex-shrink: 0;
      overflow: hidden;
      transition: width 0.3s cubic-bezier(.4,0,.2,1);
      z-index: 50;
    }
    .sidebar.expanded { width: 200px; align-items: flex-start; padding: 12px 8px; }

    .sidebar-logo {
      width: 40px; height: 40px; border-radius: 12px;
      background: linear-gradient(135deg, var(--mint), var(--indigo));
      display: flex; align-items: center; justify-content: center;
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700; font-size: 16px; color: #0a0d14;
      margin-bottom: 8px; flex-shrink: 0;
      box-shadow: 0 4px 16px rgba(110,231,183,0.3);
    }
    .sidebar.expanded .sidebar-logo { margin-left: 4px; }

    .nav-btn {
      display: flex; align-items: center; gap: 10px;
      width: 44px; height: 44px; border-radius: 12px;
      border: none; cursor: pointer;
      background: transparent;
      color: var(--text3);
      transition: all 0.2s ease;
      justify-content: center;
      position: relative;
      flex-shrink: 0;
      font-family: inherit;
      font-size: 13px; font-weight: 500;
      white-space: nowrap; overflow: hidden;
    }
    .sidebar.expanded .nav-btn { width: 100%; justify-content: flex-start; padding: 0 10px; }
    .nav-btn:hover { background: var(--bg3); color: var(--text); transform: translateX(2px); }
    .nav-btn.active {
      background: linear-gradient(135deg, rgba(110,231,183,0.15), rgba(129,140,248,0.15));
      color: var(--mint);
      box-shadow: inset 0 0 0 1px rgba(110,231,183,0.2);
    }
    .nav-btn .nav-label { display: none; }
    .sidebar.expanded .nav-btn .nav-label { display: block; }

    /* ── Header ─────────────────────────────────────────────────── */
    .header {
      height: 60px;
      background: rgba(var(--bg-rgb, 12,15,26), 0.85);
      backdrop-filter: blur(20px) saturate(180%);
      -webkit-backdrop-filter: blur(20px) saturate(180%);
      border-bottom: 1px solid var(--border);
      display: flex; align-items: center;
      padding: 0 20px; gap: 16px;
      position: sticky; top: 0; z-index: 100;
      transition: background 0.3s;
    }
    [data-theme="light"] .header { background: rgba(241,245,251,0.85); }

    .header-title {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700; font-size: 18px;
      letter-spacing: -0.5px;
      background: linear-gradient(135deg, var(--mint), var(--indigo));
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .xp-section { display: flex; align-items: center; gap: 10px; margin-left: auto; }
    .xp-ring-wrap { position: relative; width: 34px; height: 34px; }
    .xp-ring-wrap svg { transform: rotate(-90deg); }
    .xp-ring-label {
      position: absolute; inset: 0;
      display: flex; align-items: center; justify-content: center;
      font-size: 9px; font-weight: 700; color: var(--mint);
    }
    .xp-info { line-height: 1; }
    .xp-level { font-size: 11px; color: var(--text2); }
    .xp-val   { font-size: 13px; font-weight: 700; }

    .header-btn {
      padding: 6px 14px; border-radius: 10px;
      border: 1px solid var(--border2);
      background: var(--glass2); color: var(--text);
      font-family: inherit; font-size: 12px; font-weight: 500;
      cursor: pointer; transition: all 0.2s;
      backdrop-filter: blur(8px);
      display: flex; align-items: center; gap: 6px;
    }
    .header-btn:hover { background: var(--bg3); border-color: var(--mint); }

    /* ── Main content ───────────────────────────────────────────── */
    .main { flex: 1; overflow-y: auto; padding: 24px; }

    /* ── Cards ──────────────────────────────────────────────────── */
    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 20px;
      box-shadow: var(--shadow);
      transition: box-shadow 0.2s, transform 0.2s;
    }
    .card:hover { box-shadow: var(--shadow-lg); }
    .card-sm { padding: 16px; border-radius: 16px; }
    .card-title {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 14px; font-weight: 600;
      color: var(--text2); margin-bottom: 14px;
      text-transform: uppercase; letter-spacing: 0.5px;
    }

    /* ── Grid helpers ───────────────────────────────────────────── */
    .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
    .grid-3 { display: grid; grid-template-columns: repeat(3,1fr); gap: 16px; }
    .grid-auto { display: grid; grid-template-columns: repeat(auto-fit, minmax(140px,1fr)); gap: 12px; }
    .flex { display: flex; }
    .flex-col { display: flex; flex-direction: column; }
    .gap-2 { gap: 8px; }
    .gap-3 { gap: 12px; }
    .gap-4 { gap: 16px; }
    .mb-3 { margin-bottom: 12px; }
    .mb-4 { margin-bottom: 16px; }
    .mb-5 { margin-bottom: 20px; }

    /* ── Stat pills ─────────────────────────────────────────────── */
    .stat-pill {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px; padding: 14px 16px;
      display: flex; align-items: center; gap: 12px;
      box-shadow: var(--shadow);
      transition: transform 0.2s, box-shadow 0.2s;
      animation: fadeUp 0.4s ease both;
    }
    .stat-pill:hover { transform: translateY(-2px); box-shadow: var(--shadow-lg); }
    .stat-icon {
      width: 40px; height: 40px; border-radius: 12px;
      display: flex; align-items: center; justify-content: center;
      flex-shrink: 0;
    }
    .stat-label { font-size: 11px; color: var(--text2); margin-bottom: 2px; }
    .stat-value { font-size: 20px; font-weight: 700; line-height: 1; }

    /* ── Inputs ─────────────────────────────────────────────────── */
    input, textarea, select {
      background: var(--bg3);
      border: 1px solid var(--border2);
      color: var(--text);
      padding: 9px 13px;
      border-radius: 10px;
      font-family: inherit;
      font-size: 13px;
      outline: none;
      transition: border-color 0.2s, box-shadow 0.2s;
      width: 100%;
    }
    input:focus, textarea:focus, select:focus {
      border-color: var(--mint);
      box-shadow: 0 0 0 3px rgba(110,231,183,0.12);
    }
    select { cursor: pointer; }
    textarea { resize: vertical; min-height: 80px; }

    /* ── Buttons ────────────────────────────────────────────────── */
    .btn {
      padding: 9px 18px; border-radius: 10px;
      border: none; cursor: pointer;
      font-family: inherit; font-size: 13px; font-weight: 600;
      display: inline-flex; align-items: center; gap: 6px;
      transition: all 0.15s ease; white-space: nowrap;
    }
    .btn:hover  { transform: translateY(-1px); box-shadow: 0 4px 12px rgba(0,0,0,0.2); }
    .btn:active { transform: translateY(0); }
    .btn-primary   { background: linear-gradient(135deg,var(--mint),var(--indigo)); color:#0a0d14; }
    .btn-secondary { background: var(--bg3); color: var(--text); border: 1px solid var(--border2); }
    .btn-danger    { background: rgba(248,113,113,0.15); color:var(--red); border:1px solid rgba(248,113,113,0.3); }
    .btn-sm { padding: 6px 12px; font-size: 12px; border-radius: 8px; }
    .btn-icon { width:36px; height:36px; padding:0; justify-content:center; }

    /* ── Progress bars ──────────────────────────────────────────── */
    .progress-track {
      background: var(--bg3);
      border-radius: 99px; overflow: hidden;
      height: 6px;
    }
    .progress-bar {
      height: 100%; border-radius: 99px;
      transition: width 0.5s cubic-bezier(.4,0,.2,1);
    }

    /* ── Badges ─────────────────────────────────────────────────── */
    .badge {
      display: inline-flex; align-items: center; gap: 4px;
      padding: 3px 10px; border-radius: 99px;
      font-size: 11px; font-weight: 600;
    }
    .badge-mint   { background: rgba(110,231,183,0.15); color:var(--mint); }
    .badge-indigo { background: rgba(129,140,248,0.15); color:var(--indigo); }
    .badge-red    { background: rgba(248,113,113,0.15); color:var(--red); }
    .badge-amber  { background: rgba(251,191,36,0.15);  color:var(--amber); }
    .badge-pink   { background: rgba(244,114,182,0.15); color:var(--pink); }
    .badge-sky    { background: rgba(56,189,248,0.15);  color:var(--sky); }

    /* ── Toast ──────────────────────────────────────────────────── */
    .toast-wrap {
      position: fixed; bottom: 24px; right: 24px;
      z-index: 9999; display: flex; flex-direction: column; gap: 8px;
      pointer-events: none;
    }
    .toast {
      background: var(--card);
      border: 1px solid var(--border2);
      padding: 12px 18px; border-radius: 14px;
      font-size: 13px; font-weight: 500;
      box-shadow: var(--shadow-lg);
      display: flex; align-items: center; gap: 10px;
      max-width: 300px; pointer-events: all;
      animation: slideIn 0.3s ease;
    }
    .toast-dot { width:8px; height:8px; border-radius:50%; flex-shrink:0; }

    /* ── Tags ───────────────────────────────────────────────────── */
    .tag {
      padding: 3px 10px; border-radius: 99px;
      font-size: 11px; font-weight: 600;
      border: 1px solid var(--border2);
      color: var(--text2); cursor: pointer;
      transition: all 0.15s;
    }
    .tag.active, .tag:hover { border-color: var(--mint); color: var(--mint); background: rgba(110,231,183,0.08); }

    /* ── Pomodoro timer ─────────────────────────────────────────── */
    .pomo-display {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 52px; font-weight: 700;
      letter-spacing: 2px; text-align: center;
      transition: color 0.3s;
    }
    .pomo-display.work  { color: var(--mint); animation: timerPulse 2s ease infinite; }
    .pomo-display.break { color: var(--sky); }
    .pomo-display.idle  { color: var(--text); }

    /* ── Schedule widget ────────────────────────────────────────── */
    .schedule-slot {
      display: flex; gap: 12px; align-items: center;
      padding: 10px 0; border-bottom: 1px solid var(--border);
    }
    .schedule-slot:last-child { border-bottom: none; }
    .schedule-time { font-size: 12px; color: var(--text2); width: 50px; flex-shrink: 0; }
    .schedule-subject {
      font-size: 13px; font-weight: 600; flex: 1;
    }
    .schedule-now {
      background: linear-gradient(135deg, rgba(110,231,183,0.12), rgba(129,140,248,0.12));
      border-radius: 10px; padding: 2px 8px; font-size: 11px;
      color: var(--mint); font-weight: 600;
    }

    /* ── Habit dots ─────────────────────────────────────────────── */
    .habit-dots { display: flex; gap: 4px; }
    .habit-dot {
      flex: 1; aspect-ratio: 1; border-radius: 6px;
      transition: all 0.3s;
    }

    /* ── Water glasses ──────────────────────────────────────────── */
    .water-glasses { display: flex; gap: 5px; flex-wrap: wrap; }
    .water-glass {
      width: 32px; height: 42px; border-radius: 8px;
      border: 1px solid var(--border2);
      cursor: pointer; transition: all 0.25s ease;
      position: relative; overflow: hidden;
    }
    .water-glass.filled { background: var(--sky); border-color: var(--sky); box-shadow: 0 0 10px rgba(56,189,248,0.3); }
    .water-glass:not(.filled):hover { border-color: var(--sky); transform: scale(1.05); }

    /* ── Donut chart ────────────────────────────────────────────── */
    .donut-wrap { display: flex; align-items: center; gap: 16px; }
    .donut-legend { flex: 1; display: flex; flex-direction: column; gap: 6px; }
    .donut-legend-item { display: flex; align-items: center; gap: 8px; font-size: 12px; }
    .donut-dot { width: 8px; height: 8px; border-radius: 50%; flex-shrink: 0; }

    /* ── Bar chart ──────────────────────────────────────────────── */
    .bar-chart { display: flex; align-items: flex-end; gap: 4px; }
    .bar-col { flex: 1; display: flex; flex-direction: column; align-items: center; gap: 4px; }
    .bar-rect { width: 100%; border-radius: 6px 6px 0 0; transition: height 0.5s cubic-bezier(.4,0,.2,1); min-height: 2px; }
    .bar-label { font-size: 9px; color: var(--text3); }

    /* ── Notes ──────────────────────────────────────────────────── */
    .note-area {
      background: var(--bg3); border: 1px solid var(--border2);
      border-radius: 14px; padding: 16px;
      font-family: inherit; font-size: 14px; line-height: 1.7;
      color: var(--text); resize: none; width: 100%;
      min-height: 200px; outline: none;
      transition: border-color 0.2s, box-shadow 0.2s;
    }
    .note-area:focus { border-color: var(--mint); box-shadow: 0 0 0 3px rgba(110,231,183,0.1); }

    /* ── Priority indicators ────────────────────────────────────── */
    .priority-dot { width: 6px; border-radius: 3px; height: 36px; flex-shrink: 0; }

    /* ── Task item ──────────────────────────────────────────────── */
    .task-item {
      background: var(--card); border: 1px solid var(--border);
      border-radius: 14px; padding: 12px 16px;
      display: flex; align-items: center; gap: 12px;
      transition: all 0.2s; animation: fadeUp 0.3s ease both;
    }
    .task-item:hover { border-color: var(--border2); box-shadow: var(--shadow); }
    .task-item.done { opacity: 0.55; }
    .task-item.overdue .task-title { color: var(--red) !important; }

    .check-btn {
      width: 22px; height: 22px; border-radius: 50%;
      border: 2px solid var(--border2); background: transparent;
      display: flex; align-items: center; justify-content: center;
      cursor: pointer; flex-shrink: 0; transition: all 0.2s;
    }
    .check-btn.checked { background: var(--mint); border-color: var(--mint); }
    .check-btn:hover:not(.checked) { border-color: var(--mint); }

    /* ── Gamification badges ────────────────────────────────────── */
    .badge-card {
      width: 60px; height: 60px; border-radius: 16px;
      display: flex; flex-direction: column; align-items: center;
      justify-content: center; gap: 3px;
      border: 1.5px solid var(--border2);
      transition: all 0.3s;
    }
    .badge-card.earned {
      border-color: var(--mint);
      background: rgba(110,231,183,0.1);
      box-shadow: 0 0 16px rgba(110,231,183,0.15);
      animation: popIn 0.4s ease;
    }
    .badge-card.locked { opacity: 0.3; }
    .badge-card span { font-size: 8px; color: var(--text2); text-align: center; line-height: 1.2; }

    /* ── Export/Import ──────────────────────────────────────────── */
    .export-row { display: flex; gap: 10px; flex-wrap: wrap; }

    /* ── Responsive ─────────────────────────────────────────────── */
    @media (max-width: 768px) {
      .sidebar { width: 56px; }
      .sidebar.expanded { width: 180px; }
      .main { padding: 16px; }
      .grid-2, .grid-3 { grid-template-columns: 1fr; }
      .pomo-display { font-size: 40px; }
      .xp-info { display: none; }
    }
    @media (max-width: 480px) {
      .header { padding: 0 12px; gap: 10px; }
      .main { padding: 12px; }
      .stat-value { font-size: 16px; }
    }

    /* ── Section page title ─────────────────────────────────────── */
    .page-title {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 24px; font-weight: 700;
      letter-spacing: -0.5px; margin-bottom: 20px;
    }
    .page-subtitle { color: var(--text2); font-size: 13px; margin-top: 2px; }

    /* ── Input row ──────────────────────────────────────────────── */
    .input-row { display: flex; gap: 8px; flex-wrap: wrap; align-items: flex-end; }
    .input-group { display: flex; flex-direction: column; gap: 5px; }
    .input-label { font-size: 11px; color: var(--text2); font-weight: 600; text-transform: uppercase; letter-spacing: 0.5px; }

    /* ── Section separator ──────────────────────────────────────── */
    .sep { height: 1px; background: var(--border); margin: 20px 0; }

    /* ── Win items ──────────────────────────────────────────────── */
    .win-item {
      display: flex; align-items: center; gap: 10px;
      padding: 8px 0; border-bottom: 1px solid var(--border);
      font-size: 13px;
    }
    .win-item:last-child { border-bottom: none; }

    /* ── GPA display ────────────────────────────────────────────── */
    .gpa-ring {
      width: 80px; height: 80px; border-radius: 50%;
      background: conic-gradient(var(--mint) var(--pct, 0%), var(--bg3) 0%);
      display: flex; align-items: center; justify-content: center;
      position: relative;
    }
    .gpa-inner {
      width: 60px; height: 60px; border-radius: 50%;
      background: var(--card);
      display: flex; align-items: center; justify-content: center;
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700; font-size: 16px; color: var(--mint);
    }

    /* ── Overflow utility ───────────────────────────────────────── */
    .truncate { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }

    /* Section staggered animation */
    .card:nth-child(1) { animation-delay: 0.0s; }
    .card:nth-child(2) { animation-delay: 0.05s; }
    .card:nth-child(3) { animation-delay: 0.10s; }
    .card:nth-child(4) { animation-delay: 0.15s; }
    .stat-pill:nth-child(1) { animation-delay: 0.0s; }
    .stat-pill:nth-child(2) { animation-delay: 0.05s; }
    .stat-pill:nth-child(3) { animation-delay: 0.10s; }
    .stat-pill:nth-child(4) { animation-delay: 0.15s; }
    .stat-pill:nth-child(5) { animation-delay: 0.20s; }
    .stat-pill:nth-child(6) { animation-delay: 0.25s; }
  </style>
</head>
<body>
<div id="app"></div>
<script type="text/babel">
/* ================================================================
   LifeOS Student — Complete Single-File App
   React 18 + Babel Standalone + localStorage
   ================================================================ */

const { useState, useEffect, useRef, useCallback, useMemo } = React;

/* ── Helpers ───────────────────────────────────────────────────── */
const uid    = () => Math.random().toString(36).slice(2, 9);
const today  = () => new Date().toISOString().slice(0, 10);
const fmt2   = n  => String(n).padStart(2, '0');
const fmtDate = d => new Date(d).toLocaleDateString('en', { month:'short', day:'numeric' });
const isOverdue = date => date && date < today();

/* ── localStorage hook ─────────────────────────────────────────── */
function useLS(key, init) {
  const [val, setVal] = useState(() => {
    try { const s = localStorage.getItem(key); return s !== null ? JSON.parse(s) : init; }
    catch { return init; }
  });
  const set = useCallback(v => {
    setVal(prev => {
      const next = typeof v === 'function' ? v(prev) : v;
      try { localStorage.setItem(key, JSON.stringify(next)); } catch {}
      return next;
    });
  }, [key]);
  return [val, set];
}

/* ── Inline SVG icons ─────────────────────────────────────────── */
function Icon({ name, size=18, color='currentColor', style={} }) {
  const paths = {
    overview: <><circle cx="12" cy="12" r="3"/><path d="M3 12h3m12 0h3M12 3v3m0 12v3m-6.36-2.64 2.12-2.12m8.49-8.49 2.12-2.12M5.64 5.64l2.12 2.12m8.49 8.49 2.12 2.12"/></>,
    tasks:    <><path d="M9 11l3 3L22 4"/><path d="M21 12v7a2 2 0 01-2 2H5a2 2 0 01-2-2V5a2 2 0 012-2h11"/></>,
    habits:   <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/>,
    time:     <><circle cx="12" cy="12" r="10"/><polyline points="12,6 12,12 16,14"/></>,
    money:    <><line x1="12" y1="1" x2="12" y2="23"/><path d="M17 5H9.5a3.5 3.5 0 000 7h5a3.5 3.5 0 010 7H6"/></>,
    food:     <><path d="M18 8h1a4 4 0 010 8h-1"/><path d="M2 8h16v9a4 4 0 01-4 4H6a4 4 0 01-4-4V8z"/><line x1="6" y1="1" x2="6" y2="4"/><line x1="10" y1="1" x2="10" y2="4"/><line x1="14" y1="1" x2="14" y2="4"/></>,
    notes:    <><path d="M14 2H6a2 2 0 00-2 2v16a2 2 0 002 2h12a2 2 0 002-2V8z"/><polyline points="14,2 14,8 20,8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10,9 9,9 8,9"/></>,
    plus:     <><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></>,
    trash:    <><polyline points="3,6 5,6 21,6"/><path d="M19 6l-1 14H6L5 6"/><path d="M10 11v6m4-6v6"/><path d="M9 6V4h6v2"/></>,
    check:    <polyline points="20,6 9,17 4,12"/>,
    play:     <polygon points="5,3 19,12 5,21 5,3"/>,
    pause:    <><rect x="6" y="4" width="4" height="16"/><rect x="14" y="4" width="4" height="16"/></>,
    stop:     <rect x="3" y="3" width="18" height="18" rx="2" ry="2"/>,
    coffee:   <><path d="M18 8h1a4 4 0 010 8h-1"/><path d="M2 8h16v9a4 4 0 01-4 4H6a4 4 0 01-4-4V8z"/></>,
    trophy:   <><path d="M6 9H4.5a2.5 2.5 0 010-5H6"/><path d="M18 9h1.5a2.5 2.5 0 000-5H18"/><path d="M4 22h16"/><path d="M10 14.66V17c0 .55-.47.98-.97 1.21C7.85 18.75 7 20.24 7 22"/><path d="M14 14.66V17c0 .55.47.98.97 1.21C16.15 18.75 17 20.24 17 22"/><path d="M18 2H6v7a6 6 0 0012 0V2z"/></>,
    fire:     <path d="M8.5 14.5A2.5 2.5 0 0011 12c0-1.38-.5-2-1-3-1.072-2.143-.224-4.054 2-6 .5 2.5 2 4.9 4 6.5 2 1.6 3 3.5 3 5.5a7 7 0 11-14 0c0-1.153.433-2.294 1-3a2.5 2.5 0 002.5 2.5z"/>,
    star:     <polygon points="12,2 15.09,8.26 22,9.27 17,14.14 18.18,21.02 12,17.77 5.82,21.02 7,14.14 2,9.27 8.91,8.26 12,2"/>,
    droplet:  <path d="M12 2.69l5.66 5.66a8 8 0 11-11.31 0z"/>,
    zap:      <polygon points="13,2 3,14 12,14 11,22 21,10 12,10 13,2"/>,
    book:     <><path d="M4 19.5A2.5 2.5 0 016.5 17H20"/><path d="M6.5 2H20v20H6.5A2.5 2.5 0 014 19.5v-15A2.5 2.5 0 016.5 2z"/></>,
    sun:      <><circle cx="12" cy="12" r="5"/><line x1="12" y1="1" x2="12" y2="3"/><line x1="12" y1="21" x2="12" y2="23"/><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"/><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"/><line x1="1" y1="12" x2="3" y2="12"/><line x1="21" y1="12" x2="23" y2="12"/><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"/><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"/></>,
    moon:     <path d="M21 12.79A9 9 0 1111.21 3 7 7 0 0021 12.79z"/>,
    download: <><path d="M21 15v4a2 2 0 01-2 2H5a2 2 0 01-2-2v-4"/><polyline points="7,10 12,15 17,10"/><line x1="12" y1="15" x2="12" y2="3"/></>,
    upload:   <><path d="M21 15v4a2 2 0 01-2 2H5a2 2 0 01-2-2v-4"/><polyline points="17,8 12,3 7,8"/><line x1="12" y1="3" x2="12" y2="15"/></>,
    menu:     <><line x1="3" y1="6" x2="21" y2="6"/><line x1="3" y1="12" x2="21" y2="12"/><line x1="3" y1="18" x2="21" y2="18"/></>,
    clock:    <><circle cx="12" cy="12" r="10"/><polyline points="12,6 12,12 16,14"/></>,
    alert:    <><path d="M10.29 3.86L1.82 18a2 2 0 001.71 3h16.94a2 2 0 001.71-3L13.71 3.86a2 2 0 00-3.42 0z"/><line x1="12" y1="9" x2="12" y2="13"/><line x1="12" y1="17" x2="12.01" y2="17"/></>,
    chart:    <><line x1="18" y1="20" x2="18" y2="10"/><line x1="12" y1="20" x2="12" y2="4"/><line x1="6" y1="20" x2="6" y2="14"/></>,
  };
  return (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none"
      stroke={color} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round" style={style}>
      {paths[name]}
    </svg>
  );
}

/* ── Donut chart component ─────────────────────────────────────── */
function DonutChart({ data, size=110, thickness=13 }) {
  const r = (size - thickness) / 2;
  const cx = size / 2;
  const circ = 2 * Math.PI * r;
  const total = data.reduce((s, d) => s + (d.value||0), 0) || 1;
  let offset = 0;
  return (
    <svg width={size} height={size} style={{ transform: 'rotate(-90deg)', flexShrink:0 }}>
      {data.map((d, i) => {
        const pct = (d.value||0) / total;
        const dash = circ * pct;
        const el = (
          <circle key={i} cx={cx} cy={cx} r={r}
            fill="none" stroke={d.color} strokeWidth={thickness}
            strokeDasharray={`${dash} ${circ - dash}`}
            strokeDashoffset={-offset * circ}
            strokeLinecap="round"
            style={{ transition: 'stroke-dasharray 0.6s ease' }}
          />
        );
        offset += pct;
        return el;
      })}
    </svg>
  );
}

/* ── Bar chart component ───────────────────────────────────────── */
function BarChart({ data, color='var(--mint)', height=60 }) {
  const max = Math.max(...data.map(d => d.value||0), 1);
  return (
    <div className="bar-chart" style={{ height }}>
      {data.map((d, i) => (
        <div key={i} className="bar-col">
          <div className="bar-rect" style={{
            height: `${((d.value||0)/max) * (height-18)}px`,
            background: color,
            opacity: 0.6 + ((d.value||0)/max)*0.4,
          }}/>
          <span className="bar-label">{d.label}</span>
        </div>
      ))}
    </div>
  );
}

/* ── Toast system ──────────────────────────────────────────────── */
function ToastContainer({ toasts, remove }) {
  const colors = { success:'var(--mint)', warn:'var(--amber)', error:'var(--red)', info:'var(--indigo)' };
  return (
    <div className="toast-wrap">
      {toasts.map(t => (
        <div key={t.id} className="toast" onClick={() => remove(t.id)} style={{ cursor:'pointer' }}>
          <div className="toast-dot" style={{ background: colors[t.type||'success'] }}/>
          <span>{t.message}</span>
        </div>
      ))}
    </div>
  );
}

/* ── Gamification config ───────────────────────────────────────── */
const BADGE_DEFS = [
  { id:'first_task',  icon:'zap',    label:'First Step',   desc:'Complete first task' },
  { id:'streak_3',    icon:'fire',   label:'On Fire',      desc:'3-day habit streak' },
  { id:'streak_7',    icon:'star',   label:'Week Warrior', desc:'7-day habit streak' },
  { id:'hydrated',    icon:'droplet',label:'Hydrated',     desc:'8 glasses in a day' },
  { id:'pomodoro_5',  icon:'coffee', label:'Focus Master', desc:'5 Pomodoro sessions' },
  { id:'budget_kept', icon:'trophy', label:'Saver',        desc:'Stay under budget' },
  { id:'centurion',   icon:'zap',    label:'Centurion',    desc:'Reach 1000 XP' },
  { id:'bookworm',    icon:'book',   label:'Bookworm',     desc:'Log 100 reading pages' },
];

/* ── Class schedule (hardcoded for student demo) ───────────────── */
const CLASS_SCHEDULE = [
  { time:'08:00', subject:'Mathematics',   room:'A-101', color:'var(--indigo)' },
  { time:'10:00', subject:'Physics',       room:'B-203', color:'var(--mint)' },
  { time:'12:00', subject:'Lunch Break',   room:'—',     color:'var(--amber)' },
  { time:'14:00', subject:'Chemistry',     room:'C-105', color:'var(--pink)' },
  { time:'16:00', subject:'English Lit',   room:'A-210', color:'var(--sky)' },
];

const NOTE_SUBJECTS = ['Math','Physics','Chemistry','English','History','Biology','General'];
const EXPENSE_CATS  = ['Food','Transport','Books','Entertainment','Health','Other'];
const TIME_CATS     = ['Study','Project','Reading','Revision','Lab','Other'];
const PRIORITY_COLORS = { high:'var(--red)', medium:'var(--amber)', low:'var(--mint)' };
const CAT_COLORS = {
  Food:'var(--pink)', Transport:'var(--indigo)', Books:'var(--mint)',
  Entertainment:'var(--amber)', Health:'var(--green)', Other:'var(--text3)',
  Study:'var(--mint)', Project:'var(--indigo)', Reading:'var(--sky)',
  Revision:'var(--amber)', Lab:'var(--pink)',
};

/* ================================================================
   MAIN APP
   ================================================================ */
function App() {
  /* ── Theme ── */
  const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
  const [theme, setTheme] = useLS('los_theme', prefersDark ? 'dark' : 'light');
  useEffect(() => { document.documentElement.setAttribute('data-theme', theme); }, [theme]);

  /* ── Navigation ── */
  const [tab, setTab]           = useState('overview');
  const [sideExpanded, setSide] = useState(false);

  /* ── Toasts ── */
  const [toasts, setToasts] = useState([]);
  const toast = useCallback((message, type='success') => {
    const id = uid();
    setToasts(p => [...p, { id, message, type }]);
    setTimeout(() => setToasts(p => p.filter(t => t.id !== id)), 3000);
  }, []);
  const removeToast = id => setToasts(p => p.filter(t => t.id !== id));

  /* ── Gamification ── */
  const [xp, setXp]           = useLS('los_xp', 0);
  const [badges, setBadges]   = useLS('los_badges', []);
  const level    = Math.floor(xp / 1000) + 1;
  const levelPct = ((xp % 1000) / 1000) * 100;

  const addXp = useCallback((amt, reason) => {
    setXp(prev => {
      const next = prev + amt;
      if (Math.floor(prev/1000) < Math.floor(next/1000))
        toast(`🏆 Level Up! You're now Level ${Math.floor(next/1000)+1}!`);
      if (next >= 1000) awardBadge('centurion');
      return next;
    });
    if (reason) toast(`+${amt} XP — ${reason}`);
  }, []);

  const awardBadge = useCallback((id) => {
    setBadges(prev => {
      if (prev.includes(id)) return prev;
      const def = BADGE_DEFS.find(b => b.id === id);
      if (def) toast(`🎖 Badge Unlocked: ${def.label}!`);
      return [...prev, id];
    });
  }, []);

  /* ── All data stores ── */
  const [tasks, setTasks]       = useLS('los_tasks', []);
  const [habits, setHabits]     = useLS('los_habits', []);
  const [timeLogs, setTimeLogs] = useLS('los_timelogs', []);
  const [expenses, setExpenses] = useLS('los_expenses', []);
  const [budget, setBudget]     = useLS('los_budget', 2000);
  const [meals, setMeals]       = useLS('los_meals', []);
  const [waterLogs, setWater]   = useLS('los_water', []);
  const [notes, setNotes]       = useLS('los_notes', {});   // { date: { text, subject } }
  const [grades, setGrades]     = useLS('los_grades', []);  // { id, subject, grade, pts, date }
  const [pomoCount, setPomoCount] = useLS('los_pomo', 0);

  /* ── Export / Import ── */
  const exportData = () => {
    const data = { tasks, habits, timeLogs, expenses, budget, meals, waterLogs, notes, grades, xp, badges, pomoCount };
    const blob = new Blob([JSON.stringify(data, null, 2)], { type:'application/json' });
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.href = url; a.download = `lifeos-backup-${today()}.json`;
    a.click(); URL.revokeObjectURL(url);
    toast('Data exported successfully!');
  };

  const importData = (e) => {
    const file = e.target.files[0]; if (!file) return;
    const reader = new FileReader();
    reader.onload = ev => {
      try {
        const d = JSON.parse(ev.target.result);
        if (d.tasks)     setTasks(d.tasks);
        if (d.habits)    setHabits(d.habits);
        if (d.timeLogs)  setTimeLogs(d.timeLogs);
        if (d.expenses)  setExpenses(d.expenses);
        if (d.budget)    setBudget(d.budget);
        if (d.meals)     setMeals(d.meals);
        if (d.waterLogs) setWater(d.waterLogs);
        if (d.notes)     setNotes(d.notes);
        if (d.grades)    setGrades(d.grades);
        if (d.xp)        setXp(d.xp);
        if (d.badges)    setBadges(d.badges);
        toast('Data imported successfully!');
      } catch { toast('Import failed — invalid file', 'error'); }
    };
    reader.readAsText(file);
  };
  const fileRef = useRef();

  /* ── Sidebar tabs ── */
  const TABS = [
    { id:'overview', icon:'overview', label:'Overview' },
    { id:'tasks',    icon:'tasks',    label:'Tasks'    },
    { id:'habits',   icon:'habits',   label:'Habits'   },
    { id:'time',     icon:'time',     label:'Time'     },
    { id:'money',    icon:'money',    label:'Money'    },
    { id:'food',     icon:'food',     label:'Food'     },
    { id:'notes',    icon:'notes',    label:'Notes'    },
  ];

  const sharedProps = { toast, addXp, awardBadge, badges };

  return (
    <div id="app">
      {/* ── Header ── */}
      <header className="header">
        <button className="btn btn-secondary btn-icon btn-sm"
          style={{ border:'none', background:'transparent' }}
          onClick={() => setSide(p => !p)}>
          <Icon name="menu" size={18}/>
        </button>
        <span className="header-title">LifeOS</span>

        {/* XP ring */}
        <div className="xp-section">
          <div className="xp-ring-wrap">
            <svg width="34" height="34" viewBox="0 0 34 34">
              <circle cx="17" cy="17" r="14" fill="none" stroke="var(--bg3)" strokeWidth="3"/>
              <circle cx="17" cy="17" r="14" fill="none" stroke="var(--mint)" strokeWidth="3"
                strokeDasharray={`${levelPct * 0.88} 88`}
                strokeDashoffset="22" strokeLinecap="round"
                style={{ transition:'stroke-dasharray 0.5s ease' }}/>
            </svg>
            <div className="xp-ring-label">{level}</div>
          </div>
          <div className="xp-info">
            <div className="xp-level">Level {level}</div>
            <div className="xp-val">{xp} XP</div>
          </div>
        </div>

        {/* Theme toggle */}
        <button className="header-btn" onClick={() => setTheme(t => t==='dark'?'light':'dark')}>
          <Icon name={theme==='dark'?'sun':'moon'} size={14}/>
          {theme==='dark'?'Light':'Dark'}
        </button>

        {/* Export */}
        <button className="header-btn" onClick={exportData}>
          <Icon name="download" size={14}/>
          Export
        </button>
        <button className="header-btn" onClick={() => fileRef.current.click()}>
          <Icon name="upload" size={14}/>
          Import
        </button>
        <input ref={fileRef} type="file" accept=".json" style={{ display:'none' }} onChange={importData}/>
      </header>

      <div className="app-layout">
        {/* ── Sidebar ── */}
        <nav className={`sidebar${sideExpanded?' expanded':''}`}>
          <div className="sidebar-logo">L</div>
          {TABS.map(t => (
            <button key={t.id} className={`nav-btn${tab===t.id?' active':''}`}
              onClick={() => { setTab(t.id); setSide(false); }}
              title={t.label}>
              <Icon name={t.icon} size={18}/>
              <span className="nav-label">{t.label}</span>
            </button>
          ))}
        </nav>

        {/* ── Main ── */}
        <main className="main">
          {tab==='overview' && <OverviewPage {...sharedProps} tasks={tasks} habits={habits} timeLogs={timeLogs} expenses={expenses} budget={budget} waterLogs={waterLogs} grades={grades} xp={xp} level={level} levelPct={levelPct} pomoCount={pomoCount}/>}
          {tab==='tasks'    && <TasksPage    {...sharedProps} tasks={tasks} setTasks={setTasks}/>}
          {tab==='habits'   && <HabitsPage   {...sharedProps} habits={habits} setHabits={setHabits}/>}
          {tab==='time'     && <TimePage     {...sharedProps} timeLogs={timeLogs} setTimeLogs={setTimeLogs} pomoCount={pomoCount} setPomoCount={setPomoCount}/>}
          {tab==='money'    && <MoneyPage    {...sharedProps} expenses={expenses} setExpenses={setExpenses} budget={budget} setBudget={setBudget} grades={grades} setGrades={setGrades}/>}
          {tab==='food'     && <FoodPage     {...sharedProps} meals={meals} setMeals={setMeals} waterLogs={waterLogs} setWater={setWater}/>}
          {tab==='notes'    && <NotesPage    {...sharedProps} notes={notes} setNotes={setNotes}/>}
        </main>
      </div>

      <ToastContainer toasts={toasts} remove={removeToast}/>
    </div>
  );
}

/* ================================================================
   OVERVIEW PAGE
   ================================================================ */
function OverviewPage({ tasks, habits, timeLogs, expenses, budget, waterLogs, grades, xp, level, levelPct, pomoCount, badges, toast }) {
  const todayTasks    = tasks.filter(t => t.date === today());
  const doneTasks     = todayTasks.filter(t => t.done);
  const doneHabits    = habits.filter(h => (h.logs||[]).includes(today()));
  const todayWater    = waterLogs.filter(w => w.date === today()).length;
  const todayExp      = expenses.filter(e => e.date === today()).reduce((s,e) => s+e.amount, 0);
  const todayMins     = timeLogs.filter(l => l.date === today()).reduce((s,l) => s+l.minutes, 0);

  /* GPA calc — A=4.0, B=3.0, C=2.0, D=1.0 */
  const gradeMap = { A:4.0, B:3.0, C:2.0, D:1.0, F:0 };
  const gpa = grades.length
    ? (grades.reduce((s,g) => s + (gradeMap[g.grade]||0), 0) / grades.length).toFixed(2)
    : null;
  const gpaMax = 4.0;
  const gpaPct = gpa ? (gpa/gpaMax)*100 : 0;

  /* Today's wins = completed tasks + logged habits */
  const wins = [
    ...doneTasks.map(t => ({ icon:'tasks', text: t.title, color:'var(--mint)' })),
    ...doneHabits.map(h => ({ icon:'habits', text: h.name, color:'var(--indigo)' })),
  ];

  /* Current class */
  const nowHour = new Date().getHours();
  const currentClass = CLASS_SCHEDULE.find(s => {
    const h = parseInt(s.time); return nowHour >= h && nowHour < h+2;
  });

  const pills = [
    { label:'Tasks Done',    value:`${doneTasks.length}/${todayTasks.length}`,      icon:'tasks',   color:'var(--mint)'   },
    { label:'Habits',        value:`${doneHabits.length}/${habits.length}`,         icon:'habits',  color:'var(--indigo)' },
    { label:'Study Time',    value:`${Math.floor(todayMins/60)}h ${todayMins%60}m`, icon:'time',    color:'var(--pink)'   },
    { label:'Spent Today',   value:`₹${todayExp}`,                                  icon:'money',   color:'var(--amber)'  },
    { label:'Water',         value:`${todayWater}/8 glasses`,                       icon:'droplet', color:'var(--sky)'    },
    { label:'Pomodoros',     value:`${pomoCount} sessions`,                         icon:'coffee',  color:'var(--orange)' },
  ];

  return (
    <div className="fade-up">
      <div className="page-title">
        Good {new Date().getHours()<12?'Morning':new Date().getHours()<17?'Afternoon':'Evening'} 👋
        <div className="page-subtitle">{new Date().toLocaleDateString('en',{weekday:'long',year:'numeric',month:'long',day:'numeric'})}</div>
      </div>

      {/* XP bar */}
      <div className="card mb-4" style={{ background:'linear-gradient(135deg,rgba(110,231,183,0.08),rgba(129,140,248,0.08))' }}>
        <div style={{ display:'flex', justifyContent:'space-between', marginBottom:10, alignItems:'center' }}>
          <span style={{ fontFamily:"'Space Grotesk',sans-serif", fontWeight:600 }}>Level {level} — {['Beginner','Learner','Scholar','Expert','Master','Legend'][Math.min(level-1,5)]}</span>
          <span style={{ color:'var(--text2)', fontSize:13 }}>{xp % 1000} / 1000 XP</span>
        </div>
        <div className="progress-track">
          <div className="progress-bar" style={{ width:`${levelPct}%`, background:'linear-gradient(90deg,var(--mint),var(--indigo))' }}/>
        </div>
      </div>

      {/* Stat pills */}
      <div className="grid-auto mb-4">
        {pills.map((p,i) => (
          <div key={i} className="stat-pill" style={{ animationDelay:`${i*0.05}s` }}>
            <div className="stat-icon" style={{ background:`color-mix(in srgb, ${p.color} 15%, transparent)` }}>
              <Icon name={p.icon} size={18} color={p.color}/>
            </div>
            <div>
              <div className="stat-label">{p.label}</div>
              <div className="stat-value" style={{ fontSize:16 }}>{p.value}</div>
            </div>
          </div>
        ))}
      </div>

      <div className="grid-2 mb-4">
        {/* Class Schedule */}
        <div className="card">
          <div className="card-title">📅 Today's Schedule</div>
          {CLASS_SCHEDULE.map((s,i) => {
            const isCurrent = currentClass === s;
            return (
              <div key={i} className="schedule-slot">
                <span className="schedule-time">{s.time}</span>
                <div style={{ width:3, height:32, borderRadius:2, background:s.color, flexShrink:0 }}/>
                <span className="schedule-subject" style={{ color: isCurrent ? s.color : 'var(--text)' }}>{s.subject}</span>
                <span style={{ fontSize:11, color:'var(--text3)' }}>{s.room}</span>
                {isCurrent && <span className="schedule-now">NOW</span>}
              </div>
            );
          })}
        </div>

        {/* Today's Wins */}
        <div className="card">
          <div className="card-title">🏆 Today's Wins</div>
          {wins.length === 0
            ? <p style={{ color:'var(--text3)', fontSize:13 }}>Complete tasks or habits to see your wins here!</p>
            : wins.map((w,i) => (
              <div key={i} className="win-item">
                <Icon name={w.icon} size={14} color={w.color}/>
                <span style={{ fontSize:13 }}>{w.text}</span>
                <span className="badge badge-mint" style={{ marginLeft:'auto' }}>✓</span>
              </div>
            ))
          }
          {wins.length > 0 && (
            <div style={{ marginTop:12, padding:'10px 14px', background:'rgba(110,231,183,0.08)', borderRadius:10, fontSize:13, color:'var(--mint)', fontWeight:600 }}>
              🎉 {wins.length} win{wins.length>1?'s':''} today — keep going!
            </div>
          )}
        </div>
      </div>

      <div className="grid-2 mb-4">
        {/* GPA tracker */}
        <div className="card">
          <div className="card-title">📊 Academic Performance</div>
          {gpa ? (
            <div style={{ display:'flex', alignItems:'center', gap:20 }}>
              <div className="gpa-ring" style={{ '--pct':`${gpaPct}%` }}>
                <div className="gpa-inner">{gpa}</div>
              </div>
              <div>
                <div style={{ fontSize:13, color:'var(--text2)', marginBottom:8 }}>GPA / 4.0</div>
                {grades.slice(-4).map((g,i) => (
                  <div key={i} style={{ display:'flex', gap:8, fontSize:12, marginBottom:4 }}>
                    <span style={{ color:'var(--text2)' }}>{g.subject}</span>
                    <span className={`badge badge-${g.grade==='A'?'mint':g.grade==='B'?'indigo':g.grade==='C'?'amber':'red'}`}>{g.grade}</span>
                  </div>
                ))}
              </div>
            </div>
          ) : (
            <p style={{ color:'var(--text3)', fontSize:13 }}>Log grades in the Money tab to see your GPA here.</p>
          )}
        </div>

        {/* Badges */}
        <div className="card">
          <div className="card-title">🎖 Badges</div>
          <div style={{ display:'flex', gap:8, flexWrap:'wrap' }}>
            {BADGE_DEFS.map(b => {
              const earned = badges.includes(b.id);
              return (
                <div key={b.id} className={`badge-card${earned?' earned':' locked'}`} title={b.desc}>
                  <Icon name={b.icon} size={20} color={earned?'var(--mint)':'var(--text3)'}/>
                  <span>{b.label}</span>
                </div>
              );
            })}
          </div>
        </div>
      </div>
    </div>
  );
}

/* ================================================================
   TASKS PAGE
   ================================================================ */
function TasksPage({ tasks, setTasks, addXp, toast, awardBadge, badges }) {
  const [form, setForm] = useState({ title:'', priority:'medium', date:today(), notes:'' });
  const [filter, setFilter] = useState('today');

  const add = () => {
    if (!form.title.trim()) return;
    setTasks(p => [...p, { id:uid(), ...form, done:false, createdAt:Date.now() }]);
    setForm({ title:'', priority:'medium', date:today(), notes:'' });
    toast('Task added!');
  };

  const toggle = id => setTasks(p => p.map(t => {
    if (t.id !== id) return t;
    const done = !t.done;
    if (done) {
      addXp(25, 'Task completed');
      if (!badges.includes('first_task')) awardBadge('first_task');
    }
    return { ...t, done };
  }));

  const del = id => setTasks(p => p.filter(t => t.id !== id));

  const carryOver = () => {
    const tmr = new Date(); tmr.setDate(tmr.getDate()+1);
    const ts = tmr.toISOString().slice(0,10);
    let n = 0;
    setTasks(p => p.map(t => {
      if (t.date===today() && !t.done) { n++; return {...t,date:ts}; }
      return t;
    }));
    toast(`Carried ${n} task${n!==1?'s':''} to tomorrow`);
  };

  const filtered = useMemo(() => {
    const base = filter==='today' ? tasks.filter(t=>t.date===today())
               : filter==='all'   ? tasks
               : filter==='done'  ? tasks.filter(t=>t.done)
               : tasks.filter(t=>!t.done);
    return [...base].sort((a,b)=>({high:0,medium:1,low:2}[a.priority]-{high:0,medium:1,low:2}[b.priority]));
  }, [tasks, filter]);

  const overdue = tasks.filter(t => !t.done && isOverdue(t.date));

  return (
    <div className="fade-up">
      <div style={{ display:'flex', justifyContent:'space-between', alignItems:'flex-start', marginBottom:20, flexWrap:'wrap', gap:12 }}>
        <div className="page-title" style={{ marginBottom:0 }}>
          Tasks
          <div className="page-subtitle">{tasks.filter(t=>t.done&&t.date===today()).length}/{tasks.filter(t=>t.date===today()).length} done today</div>
        </div>
        <button className="btn btn-secondary btn-sm" onClick={carryOver}>Carry Over Unfinished</button>
      </div>

      {/* Overdue warning */}
      {overdue.length > 0 && (
        <div className="card mb-4" style={{ border:'1px solid rgba(248,113,113,0.3)', background:'rgba(248,113,113,0.06)' }}>
          <div style={{ display:'flex', gap:10, alignItems:'center' }}>
            <Icon name="alert" size={16} color="var(--red)"/>
            <span style={{ color:'var(--red)', fontSize:13, fontWeight:600 }}>{overdue.length} overdue task{overdue.length>1?'s':''}</span>
          </div>
          <div style={{ display:'flex', flexWrap:'wrap', gap:6, marginTop:8 }}>
            {overdue.map(t => <span key={t.id} className="badge badge-red">{t.title} · {fmtDate(t.date)}</span>)}
          </div>
        </div>
      )}

      {/* Add task */}
      <div className="card mb-4">
        <div className="card-title">Add Task</div>
        <div className="input-row mb-3">
          <div className="input-group" style={{ flex:2 }}>
            <label className="input-label">Task</label>
            <input value={form.title} onChange={e=>setForm(p=>({...p,title:e.target.value}))}
              onKeyDown={e=>e.key==='Enter'&&add()} placeholder="What needs to be done?"/>
          </div>
          <div className="input-group">
            <label className="input-label">Priority</label>
            <select value={form.priority} onChange={e=>setForm(p=>({...p,priority:e.target.value}))}>
              <option value="high">🔴 High</option>
              <option value="medium">🟡 Medium</option>
              <option value="low">🟢 Low</option>
            </select>
          </div>
          <div className="input-group">
            <label className="input-label">Due Date</label>
            <input type="date" value={form.date} onChange={e=>setForm(p=>({...p,date:e.target.value}))}/>
          </div>
        </div>
        <div className="input-row">
          <input value={form.notes} onChange={e=>setForm(p=>({...p,notes:e.target.value}))}
            placeholder="Notes (optional)..." style={{ flex:1 }}/>
          <button className="btn btn-primary" onClick={add}>
            <Icon name="plus" size={14} color="#0a0d14"/>Add Task
          </button>
        </div>
      </div>

      {/* Filters */}
      <div style={{ display:'flex', gap:8, marginBottom:16, flexWrap:'wrap' }}>
        {['today','all','pending','done'].map(f => (
          <button key={f} className={`tag${filter===f?' active':''}`} onClick={()=>setFilter(f)}>
            {f.charAt(0).toUpperCase()+f.slice(1)}
          </button>
        ))}
        <span style={{ marginLeft:'auto', color:'var(--text2)', fontSize:12, alignSelf:'center' }}>
          {filtered.length} task{filtered.length!==1?'s':''}
        </span>
      </div>

      {/* Task list */}
      <div className="flex-col gap-2">
        {filtered.length === 0 && (
          <div className="card" style={{ textAlign:'center', padding:40, color:'var(--text3)' }}>
            No tasks here — add one above!
          </div>
        )}
        {filtered.map((task,i) => {
          const over = !task.done && isOverdue(task.date);
          return (
            <div key={task.id} className={`task-item${task.done?' done':''}${over?' overdue':''}`} style={{ animationDelay:`${i*0.04}s` }}>
              <div className="priority-dot" style={{ background: PRIORITY_COLORS[task.priority] }}/>
              {/* Checkbox */}
              <button className={`check-btn${task.done?' checked':''}`} onClick={()=>toggle(task.id)}>
                {task.done && <Icon name="check" size={11} color="#0a0d14"/>}
              </button>
              <div style={{ flex:1, minWidth:0 }}>
                <div className="task-title" style={{ fontSize:14, fontWeight:500, textDecoration:task.done?'line-through':'none', color:task.done?'var(--text3)':'var(--text)' }}>
                  {task.title}
                </div>
                {task.notes && <div style={{ fontSize:12, color:'var(--text3)', marginTop:2 }}>{task.notes}</div>}
              </div>
              <div style={{ display:'flex', alignItems:'center', gap:8, flexShrink:0 }}>
                {over && <span className="badge badge-red">Overdue</span>}
                {task.date && <span style={{ fontSize:11, color:'var(--text3)' }}>{fmtDate(task.date)}</span>}
                <span className={`badge badge-${task.priority==='high'?'red':task.priority==='medium'?'amber':'mint'}`}>
                  {task.priority}
                </span>
                <button className="btn btn-icon btn-danger btn-sm" onClick={()=>del(task.id)} style={{ width:28, height:28 }}>
                  <Icon name="trash" size={13}/>
                </button>
              </div>
            </div>
          );
        })}
      </div>
    </div>
  );
}

/* ================================================================
   HABITS PAGE
   ================================================================ */
function HabitsPage({ habits, setHabits, addXp, toast, awardBadge, badges }) {
  const [form, setForm] = useState({ name:'', color:'#6EE7B7', type:'general', goal:7 });

  const calcStreak = logs => {
    if (!logs?.length) return 0;
    let s = 0; const d = new Date();
    for (let i=0; i<365; i++) {
      if (logs.includes(d.toISOString().slice(0,10))) { s++; d.setDate(d.getDate()-1); }
      else break;
    }
    return s;
  };

  const add = () => {
    if (!form.name.trim()) return;
    setHabits(p => [...p, { id:uid(), ...form, logs:[], pages:0 }]);
    setForm({ name:'', color:'#6EE7B7', type:'general', goal:7 });
    toast('Habit created!');
  };

  const logHabit = id => setHabits(p => p.map(h => {
    if (h.id !== id) return h;
    const logs = h.logs||[];
    if (logs.includes(today())) return { ...h, logs: logs.filter(d=>d!==today()) };
    addXp(10, 'Habit logged');
    const newLogs = [...logs, today()];
    const streak = calcStreak(newLogs);
    if (streak >= 3) awardBadge('streak_3');
    if (streak >= 7) awardBadge('streak_7');
    return { ...h, logs: newLogs };
  }));

  const addPages = (id, pages) => setHabits(p => p.map(h => {
    if (h.id !== id) return h;
    const newPages = (h.pages||0) + pages;
    if (newPages >= 100) awardBadge('bookworm');
    return { ...h, pages: newPages };
  }));

  const del = id => setHabits(p => p.filter(h => h.id !== id));

  const getLast7 = logs => Array.from({length:7}, (_,i) => {
    const d = new Date(); d.setDate(d.getDate()-6+i);
    return logs?.includes(d.toISOString().slice(0,10)) || false;
  });

  const DAYS = ['M','T','W','T','F','S','S'];

  return (
    <div className="fade-up">
      <div className="page-title">Habits
        <div className="page-subtitle">{habits.filter(h=>(h.logs||[]).includes(today())).length}/{habits.length} done today</div>
      </div>

      {/* Add habit */}
      <div className="card mb-4">
        <div className="card-title">New Habit</div>
        <div className="input-row mb-3">
          <div className="input-group" style={{ flex:2 }}>
            <label className="input-label">Name</label>
            <input value={form.name} onChange={e=>setForm(p=>({...p,name:e.target.value}))}
              onKeyDown={e=>e.key==='Enter'&&add()} placeholder="e.g. Morning Exercise, Read 20 pages..."/>
          </div>
          <div className="input-group">
            <label className="input-label">Type</label>
            <select value={form.type} onChange={e=>setForm(p=>({...p,type:e.target.value}))}>
              <option value="general">General</option>
              <option value="reading">📖 Reading (pages)</option>
              <option value="exercise">🏃 Exercise</option>
              <option value="study">📚 Study</option>
            </select>
          </div>
          <div className="input-group">
            <label className="input-label">Weekly Goal</label>
            <input type="number" value={form.goal} min="1" max="7"
              onChange={e=>setForm(p=>({...p,goal:+e.target.value}))} style={{ width:80 }}/>
          </div>
          <div className="input-group">
            <label className="input-label">Color</label>
            <input type="color" value={form.color} onChange={e=>setForm(p=>({...p,color:e.target.value}))}
              style={{ width:44, height:38, padding:4, cursor:'pointer' }}/>
          </div>
        </div>
        <button className="btn btn-primary" onClick={add}>
          <Icon name="plus" size={14} color="#0a0d14"/>Add Habit
        </button>
      </div>

      {/* Habits list */}
      <div className="flex-col gap-3">
        {habits.length===0 && (
          <div className="card" style={{ textAlign:'center', padding:40, color:'var(--text3)' }}>No habits yet. Build your first one above!</div>
        )}
        {habits.map((h,idx) => {
          const logged   = (h.logs||[]).includes(today());
          const streak   = calcStreak(h.logs);
          const last7    = getLast7(h.logs);
          const thisWeek = (h.logs||[]).filter(d=>{ const w=new Date();w.setDate(w.getDate()-6);return d>=w.toISOString().slice(0,10); }).length;
          const [pages, setPageInput] = useState('');

          return (
            <div key={h.id} className="card fade-up" style={{ animationDelay:`${idx*0.05}s` }}>
              <div style={{ display:'flex', alignItems:'center', gap:12, marginBottom:12, flexWrap:'wrap' }}>
                <div style={{ width:12, height:12, borderRadius:'50%', background:h.color, flexShrink:0 }}/>
                <span style={{ fontWeight:600, fontSize:15, flex:1 }}>{h.name}</span>
                {h.type==='reading' && (
                  <span className="badge badge-sky">📖 {h.pages||0} pages total</span>
                )}
                <span className="badge badge-amber">🔥 {streak}d streak</span>
                <span style={{ fontSize:12, background:`${h.color}22`, color:h.color, padding:'3px 10px', borderRadius:99 }}>
                  {thisWeek}/{h.goal} this week
                </span>
                <button className="btn btn-sm" onClick={()=>logHabit(h.id)}
                  style={{ background:logged?h.color:'transparent', color:logged?'#0a0d14':h.color, border:`1.5px solid ${h.color}` }}>
                  {logged ? '✓ Done' : 'Log Today'}
                </button>
                <button className="btn btn-danger btn-icon btn-sm" onClick={()=>del(h.id)} style={{width:28,height:28}}>
                  <Icon name="trash" size={12}/>
                </button>
              </div>

              {/* Reading pages input */}
              {h.type==='reading' && (
                <div className="input-row mb-3" style={{ alignItems:'center' }}>
                  <input type="number" value={pages} onChange={e=>setPageInput(e.target.value)}
                    placeholder="Pages read today..." style={{ width:180 }}/>
                  <button className="btn btn-secondary btn-sm" onClick={()=>{ if(+pages>0){addPages(h.id,+pages);setPageInput('');toast(`+${pages} pages logged!`);} }}>
                    Log Pages
                  </button>
                </div>
              )}

              {/* 7-day dots */}
              <div className="habit-dots mb-3">
                {DAYS.map((day,i) => (
                  <div key={i} style={{ flex:1, textAlign:'center' }}>
                    <div className="habit-dot" style={{ background:last7[i]?h.color:'var(--bg3)' }}/>
                    <div style={{ fontSize:9, color:'var(--text3)', marginTop:3 }}>{day}</div>
                  </div>
                ))}
              </div>

              {/* Progress bar */}
              <div className="progress-track">
                <div className="progress-bar" style={{ width:`${Math.min(100,(thisWeek/h.goal)*100)}%`, background:h.color }}/>
              </div>
            </div>
          );
        })}
      </div>
    </div>
  );
}

/* ================================================================
   TIME TRACKER PAGE (with Pomodoro)
   ================================================================ */
function TimePage({ timeLogs, setTimeLogs, addXp, toast, awardBadge, badges, pomoCount, setPomoCount }) {
  /* ── Stopwatch ── */
  const [running, setRunning]   = useState(false);
  const [elapsed, setElapsed]   = useState(0);
  const [activity, setActivity] = useState('');
  const [category, setCat]      = useState('Study');
  const iRef = useRef(null);

  /* ── Pomodoro ── */
  const POMO_WORK  = 25 * 60;
  const POMO_BREAK = 5  * 60;
  const [pomoMode, setPomoMode]       = useState(false);
  const [pomoPhase, setPomoPhase]     = useState('idle'); // idle | work | break
  const [pomoSecs, setPomoSecs]       = useState(POMO_WORK);
  const pomoRef = useRef(null);

  /* ── Manual ── */
  const [manual, setManual] = useState({ activity:'', category:'Study', minutes:30 });

  /* Stopwatch tick */
  useEffect(() => {
    if (running) iRef.current = setInterval(() => setElapsed(p=>p+1), 1000);
    else clearInterval(iRef.current);
    return () => clearInterval(iRef.current);
  }, [running]);

  /* Pomodoro tick */
  useEffect(() => {
    if (pomoPhase === 'work' || pomoPhase === 'break') {
      pomoRef.current = setInterval(() => {
        setPomoSecs(p => {
          if (p <= 1) {
            clearInterval(pomoRef.current);
            if (pomoPhase === 'work') {
              toast('🍅 Pomodoro done! Take a 5-min break.', 'success');
              const newCount = pomoCount + 1;
              setPomoCount(newCount);
              addXp(50, 'Pomodoro completed');
              if (newCount >= 5) awardBadge('pomodoro_5');
              setPomoPhase('break');
              return POMO_BREAK;
            } else {
              toast('☕ Break over! Back to work.', 'info');
              setPomoPhase('work');
              return POMO_WORK;
            }
          }
          return p - 1;
        });
      }, 1000);
    } else clearInterval(pomoRef.current);
    return () => clearInterval(pomoRef.current);
  }, [pomoPhase]);

  const startStop = () => {
    if (!running && !activity.trim()) { toast('Enter an activity name first', 'warn'); return; }
    setRunning(p => !p);
  };

  const stopSave = () => {
    if (elapsed > 5) {
      const m = Math.round(elapsed/60);
      setTimeLogs(p => [...p, { id:uid(), activity, category, minutes:m, date:today(), ts:Date.now() }]);
      addXp(Math.min(60,m), `Logged ${m}min`);
      toast(`Saved: ${activity} — ${m}min`);
    }
    setRunning(false); setElapsed(0); setActivity('');
  };

  const addManual = () => {
    if (!manual.activity.trim() || manual.minutes <= 0) return;
    setTimeLogs(p => [...p, { id:uid(), ...manual, date:today(), ts:Date.now() }]);
    addXp(Math.min(60, manual.minutes), 'Time logged');
    toast('Session logged!');
    setManual({ activity:'', category:'Study', minutes:30 });
  };

  const del = id => setTimeLogs(p => p.filter(l => l.id !== id));

  /* Weekly chart */
  const weekData = Array.from({length:7}, (_,i) => {
    const d=new Date(); d.setDate(d.getDate()-6+i);
    const ds=d.toISOString().slice(0,10);
    return { label:d.toLocaleDateString('en',{weekday:'narrow'}), value:timeLogs.filter(l=>l.date===ds).reduce((s,l)=>s+l.minutes,0) };
  });

  const todayMins = timeLogs.filter(l=>l.date===today()).reduce((s,l)=>s+l.minutes,0);
  const pomoPct   = pomoPhase==='idle' ? 0 : pomoPhase==='work' ? ((POMO_WORK-pomoSecs)/POMO_WORK)*100 : ((POMO_BREAK-pomoSecs)/POMO_BREAK)*100;

  return (
    <div className="fade-up">
      <div className="page-title">Time Tracker
        <div className="page-subtitle">Today: {Math.floor(todayMins/60)}h {todayMins%60}m logged</div>
      </div>

      <div className="grid-2 mb-4">
        {/* Stopwatch */}
        <div className="card" style={{ textAlign:'center' }}>
          <div className="card-title">⏱ Stopwatch</div>
          <div className={`pomo-display${running?' work':' idle'}`} style={{ marginBottom:16 }}>
            {fmt2(Math.floor(elapsed/3600))}:{fmt2(Math.floor((elapsed%3600)/60))}:{fmt2(elapsed%60)}
          </div>
          <div className="input-row mb-3">
            <input value={activity} onChange={e=>setActivity(e.target.value)} placeholder="Activity name..."/>
            <select value={category} onChange={e=>setCat(e.target.value)} style={{ width:'auto' }}>
              {TIME_CATS.map(c=><option key={c}>{c}</option>)}
            </select>
          </div>
          <div style={{ display:'flex', gap:10, justifyContent:'center' }}>
            <button className="btn btn-primary" onClick={startStop}>
              <Icon name={running?'pause':'play'} size={14} color="#0a0d14"/>
              {running?'Pause':'Start'}
            </button>
            {(running||elapsed>0) && (
              <button className="btn btn-danger" onClick={stopSave}>
                <Icon name="stop" size={14}/>Stop & Save
              </button>
            )}
          </div>
        </div>

        {/* Pomodoro */}
        <div className="card" style={{ textAlign:'center' }}>
          <div className="card-title">🍅 Pomodoro · {pomoCount} sessions total</div>
          <div style={{ position:'relative', width:120, height:120, margin:'0 auto 16px' }}>
            <svg width="120" height="120" style={{ transform:'rotate(-90deg)' }}>
              <circle cx="60" cy="60" r="50" fill="none" stroke="var(--bg3)" strokeWidth="8"/>
              <circle cx="60" cy="60" r="50" fill="none"
                stroke={pomoPhase==='break'?'var(--sky)':'var(--mint)'}
                strokeWidth="8"
                strokeDasharray={`${pomoPct*3.14} 314`}
                strokeLinecap="round"
                style={{ transition:'stroke-dasharray 0.5s ease' }}/>
            </svg>
            <div style={{ position:'absolute', inset:0, display:'flex', alignItems:'center', justifyContent:'center', flexDirection:'column' }}>
              <div style={{ fontSize:22, fontFamily:"'Space Grotesk',sans-serif", fontWeight:700, color:pomoPhase==='break'?'var(--sky)':'var(--mint)' }}>
                {fmt2(Math.floor(pomoSecs/60))}:{fmt2(pomoSecs%60)}
              </div>
              <div style={{ fontSize:11, color:'var(--text2)' }}>{pomoPhase==='idle'?'Ready':pomoPhase}</div>
            </div>
          </div>
          <div style={{ display:'flex', gap:8, justifyContent:'center', flexWrap:'wrap' }}>
            {pomoPhase==='idle' && (
              <button className="btn btn-primary" onClick={()=>setPomoPhase('work')}>
                <Icon name="play" size={14} color="#0a0d14"/>Start Focus
              </button>
            )}
            {(pomoPhase==='work'||pomoPhase==='break') && (
              <button className="btn btn-danger" onClick={()=>{setPomoPhase('idle');setPomoSecs(POMO_WORK);}}>
                <Icon name="stop" size={14}/>Stop
              </button>
            )}
          </div>
          <div style={{ marginTop:12, fontSize:12, color:'var(--text3)' }}>
            {pomoPhase==='work'?'25min focus session':'5min break'}
          </div>
        </div>
      </div>

      {/* Manual entry */}
      <div className="card mb-4">
        <div className="card-title">Manual Log</div>
        <div className="input-row">
          <input value={manual.activity} onChange={e=>setManual(p=>({...p,activity:e.target.value}))}
            placeholder="Activity..." style={{ flex:2 }}/>
          <select value={manual.category} onChange={e=>setManual(p=>({...p,category:e.target.value}))}>
            {TIME_CATS.map(c=><option key={c}>{c}</option>)}
          </select>
          <input type="number" value={manual.minutes} onChange={e=>setManual(p=>({...p,minutes:+e.target.value}))}
            placeholder="Minutes" style={{ width:90 }}/>
          <button className="btn btn-primary" onClick={addManual}>Log</button>
        </div>
      </div>

      {/* Weekly chart */}
      <div className="card mb-4">
        <div className="card-title">📊 Weekly Study Hours</div>
        <BarChart data={weekData.map(d=>({...d,value:Math.round(d.value/60*10)/10}))} color="var(--indigo)" height={80}/>
        <div style={{ fontSize:12, color:'var(--text3)', marginTop:8, textAlign:'right' }}>values in hours</div>
      </div>

      {/* Logs */}
      <div className="flex-col gap-2">
        {[...timeLogs].sort((a,b)=>b.ts-a.ts).slice(0,20).map(log => (
          <div key={log.id} className="task-item">
            <div style={{ width:8,height:8,borderRadius:'50%',background:CAT_COLORS[log.category]||'var(--mint)',flexShrink:0 }}/>
            <span style={{ flex:1, fontSize:13 }}>{log.activity}</span>
            <span className="badge badge-indigo">{log.category}</span>
            <span style={{ fontSize:12, fontWeight:600 }}>{log.minutes} min</span>
            <span style={{ fontSize:11, color:'var(--text3)' }}>{fmtDate(log.date)}</span>
            <button className="btn btn-danger btn-icon btn-sm" onClick={()=>del(log.id)} style={{width:28,height:28}}>
              <Icon name="trash" size={12}/>
            </button>
          </div>
        ))}
      </div>
    </div>
  );
}

/* ================================================================
   MONEY PAGE (with grades/GPA tracker)
   ================================================================ */
function MoneyPage({ expenses, setExpenses, budget, setBudget, grades, setGrades, addXp, toast, awardBadge }) {
  const [form, setForm]       = useState({ amount:'', category:'Food', note:'', date:today() });
  const [editBudget, setEdit] = useState(false);
  const [newBudget, setNB]    = useState(budget);
  const [gradeForm, setGF]    = useState({ subject:'Math', grade:'A' });

  const addExp = () => {
    if (!form.amount || isNaN(+form.amount)) return;
    const e = { id:uid(), ...form, amount:+form.amount };
    setExpenses(p => [...p, e]);
    addXp(5, 'Expense logged');
    setForm({ amount:'', category:'Food', note:'', date:today() });
    const newTotal = monthTotal + e.amount;
    if (newTotal > budget) toast(`⚠️ Over budget by ₹${newTotal-budget}!`, 'warn');
    else if (newTotal > budget*0.8) toast('🔔 80% of monthly budget used', 'warn');
    else toast('Expense added!');
    if (newTotal <= budget) awardBadge('budget_kept');
  };

  const addGrade = () => {
    setGrades(p => [...p, { id:uid(), ...gradeForm, date:today() }]);
    toast(`Grade logged: ${gradeForm.grade} in ${gradeForm.subject}`);
  };

  const del    = id => setExpenses(p => p.filter(e => e.id !== id));
  const delGrd = id => setGrades(p => p.filter(g => g.id !== id));

  const monthExp     = expenses.filter(e => e.date.startsWith(new Date().toISOString().slice(0,7)));
  const monthTotal   = monthExp.reduce((s,e) => s+e.amount, 0);
  const pct          = Math.min(100, (monthTotal/budget)*100);
  const budgetColor  = pct>90?'var(--red)':pct>75?'var(--amber)':'var(--mint)';

  const byCategory = expenses.reduce((acc,e)=>{ acc[e.category]=(acc[e.category]||0)+e.amount; return acc; }, {});
  const donutData  = Object.entries(byCategory).map(([k,v]) => ({ label:k, value:v, color:CAT_COLORS[k]||'var(--text3)' }));

  const last7 = Array.from({length:7},(_,i)=>{
    const d=new Date(); d.setDate(d.getDate()-6+i);
    const ds=d.toISOString().slice(0,10);
    return { label:d.toLocaleDateString('en',{weekday:'narrow'}), value:expenses.filter(e=>e.date===ds).reduce((s,e)=>s+e.amount,0) };
  });

  const GRADE_POINTS = { A:4.0, B:3.0, C:2.0, D:1.0, F:0 };
  const gpa = grades.length ? (grades.reduce((s,g)=>s+(GRADE_POINTS[g.grade]||0),0)/grades.length).toFixed(2) : null;

  return (
    <div className="fade-up">
      <div style={{ display:'flex', justifyContent:'space-between', alignItems:'flex-start', marginBottom:20, flexWrap:'wrap', gap:12 }}>
        <div className="page-title" style={{ marginBottom:0 }}>
          Money Tracker
          <div className="page-subtitle">₹{monthTotal} / ₹{budget} this month</div>
        </div>
        {editBudget ? (
          <div style={{ display:'flex', gap:8, alignItems:'center' }}>
            <input type="number" value={newBudget} onChange={e=>setNB(+e.target.value)} style={{ width:120 }}/>
            <button className="btn btn-primary btn-sm" onClick={()=>{setBudget(newBudget);setEdit(false);toast('Budget updated!');}}>Save</button>
            <button className="btn btn-secondary btn-sm" onClick={()=>setEdit(false)}>Cancel</button>
          </div>
        ) : (
          <button className="btn btn-secondary btn-sm" onClick={()=>setEdit(true)}>Budget: ₹{budget} ✎</button>
        )}
      </div>

      {/* Budget bar */}
      <div className="card mb-4" style={{ border:`1px solid ${pct>90?'rgba(248,113,113,0.3)':pct>75?'rgba(251,191,36,0.3)':'var(--border)'}` }}>
        <div style={{ display:'flex', justifyContent:'space-between', marginBottom:10 }}>
          <span style={{ fontWeight:600 }}>Monthly Budget</span>
          <span style={{ color:budgetColor, fontWeight:700 }}>₹{monthTotal} / ₹{budget}</span>
        </div>
        <div className="progress-track" style={{ height:10 }}>
          <div className="progress-bar" style={{ width:`${pct}%`, background:budgetColor }}/>
        </div>
        <div style={{ marginTop:8, fontSize:12, color:'var(--text2)' }}>₹{budget-monthTotal} remaining</div>
      </div>

      {/* Add expense */}
      <div className="card mb-4">
        <div className="card-title">Add Expense</div>
        <div className="input-row">
          <input type="number" value={form.amount} onChange={e=>setForm(p=>({...p,amount:e.target.value}))}
            placeholder="₹ Amount" style={{ width:110 }}/>
          <select value={form.category} onChange={e=>setForm(p=>({...p,category:e.target.value}))}>
            {EXPENSE_CATS.map(c=><option key={c}>{c}</option>)}
          </select>
          <input value={form.note} onChange={e=>setForm(p=>({...p,note:e.target.value}))}
            onKeyDown={e=>e.key==='Enter'&&addExp()} placeholder="Note..." style={{ flex:1 }}/>
          <input type="date" value={form.date} onChange={e=>setForm(p=>({...p,date:e.target.value}))} style={{ width:140 }}/>
          <button className="btn btn-primary" onClick={addExp}>Add</button>
        </div>
      </div>

      <div className="grid-2 mb-4">
        {/* Donut */}
        <div className="card">
          <div className="card-title">Spending by Category</div>
          {donutData.length>0 ? (
            <div className="donut-wrap">
              <DonutChart data={donutData}/>
              <div className="donut-legend">
                {donutData.map(d => (
                  <div key={d.label} className="donut-legend-item">
                    <div className="donut-dot" style={{ background:d.color }}/>
                    <span style={{ flex:1, color:'var(--text2)' }}>{d.label}</span>
                    <span style={{ fontWeight:600 }}>₹{d.value}</span>
                  </div>
                ))}
              </div>
            </div>
          ) : <p style={{ color:'var(--text3)', fontSize:13 }}>No expenses yet</p>}
        </div>

        {/* Weekly */}
        <div className="card">
          <div className="card-title">Last 7 Days</div>
          <BarChart data={last7} color="var(--amber)" height={80}/>
        </div>
      </div>

      {/* Grades tracker */}
      <div className="card mb-4">
        <div className="card-title">🎓 Grades Tracker {gpa && <span className="badge badge-mint" style={{marginLeft:8}}>GPA: {gpa}</span>}</div>
        <div className="input-row mb-3">
          <select value={gradeForm.subject} onChange={e=>setGF(p=>({...p,subject:e.target.value}))}>
            {NOTE_SUBJECTS.map(s=><option key={s}>{s}</option>)}
          </select>
          <select value={gradeForm.grade} onChange={e=>setGF(p=>({...p,grade:e.target.value}))} style={{ width:80 }}>
            {['A','B','C','D','F'].map(g=><option key={g}>{g}</option>)}
          </select>
          <button className="btn btn-primary" onClick={addGrade}>Log Grade</button>
        </div>
        <div style={{ display:'flex', gap:8, flexWrap:'wrap' }}>
          {grades.map(g=>(
            <div key={g.id} style={{ display:'flex', alignItems:'center', gap:6, background:'var(--bg3)', padding:'6px 12px', borderRadius:10 }}>
              <span style={{ fontSize:12, color:'var(--text2)' }}>{g.subject}</span>
              <span className={`badge badge-${g.grade==='A'?'mint':g.grade==='B'?'indigo':g.grade==='C'?'amber':'red'}`}>{g.grade}</span>
              <span style={{ fontSize:11, color:'var(--text3)' }}>{fmtDate(g.date)}</span>
              <button onClick={()=>delGrd(g.id)} style={{ background:'none', border:'none', cursor:'pointer', color:'var(--text3)', padding:2 }}>×</button>
            </div>
          ))}
        </div>
      </div>

      {/* Expense list */}
      <div className="flex-col gap-2">
        {[...expenses].sort((a,b)=>b.date.localeCompare(a.date)).slice(0,25).map(e => (
          <div key={e.id} className="task-item">
            <div style={{ width:8,height:8,borderRadius:'50%',background:CAT_COLORS[e.category]||'var(--text3)',flexShrink:0 }}/>
            <span className="badge" style={{ background:`color-mix(in srgb,${CAT_COLORS[e.category]||'var(--text3)'} 15%,transparent)`, color:CAT_COLORS[e.category]||'var(--text3)' }}>{e.category}</span>
            <span style={{ flex:1, fontSize:13, color:'var(--text2)' }}>{e.note||'—'}</span>
            <span style={{ fontWeight:700, fontSize:14 }}>₹{e.amount}</span>
            <span style={{ fontSize:11, color:'var(--text3)' }}>{fmtDate(e.date)}</span>
            <button className="btn btn-danger btn-icon btn-sm" onClick={()=>del(e.id)} style={{width:28,height:28}}>
              <Icon name="trash" size={12}/>
            </button>
          </div>
        ))}
      </div>
    </div>
  );
}

/* ================================================================
   FOOD PAGE
   ================================================================ */
function FoodPage({ meals, setMeals, waterLogs, setWater, addXp, toast, awardBadge, badges }) {
  const [form, setForm] = useState({ name:'', type:'Breakfast', calories:'', protein:'', carbs:'', fat:'' });

  const logMeal = () => {
    if (!form.name.trim()) return;
    setMeals(p => [...p, { id:uid(), ...form, calories:+form.calories||0, protein:+form.protein||0, carbs:+form.carbs||0, fat:+form.fat||0, date:today() }]);
    addXp(8, 'Meal logged');
    setForm({ name:'', type:'Breakfast', calories:'', protein:'', carbs:'', fat:'' });
    toast('Meal logged!');
  };

  const logWater = () => {
    const nl = [...waterLogs, { id:uid(), date:today() }];
    setWater(nl);
    addXp(3, 'Hydration tracked');
    const cnt = nl.filter(w=>w.date===today()).length;
    if (cnt >= 8 && !badges.includes('hydrated')) awardBadge('hydrated');
    toast(`💧 ${cnt}/8 glasses`);
  };

  const delMeal  = id => setMeals(p => p.filter(m => m.id !== id));
  const delWater = id => setWater(p => p.filter(w => w.id !== id));

  const todayMeals = meals.filter(m => m.date === today());
  const totalCals  = todayMeals.reduce((s,m) => s+m.calories, 0);
  const totalProt  = todayMeals.reduce((s,m) => s+m.protein,  0);
  const totalCarbs = todayMeals.reduce((s,m) => s+m.carbs,    0);
  const totalFat   = todayMeals.reduce((s,m) => s+m.fat,      0);
  const todayWater = waterLogs.filter(w => w.date === today()).length;

  const macroData = [
    { label:'Protein', value:totalProt,  color:'var(--mint)'   },
    { label:'Carbs',   value:totalCarbs, color:'var(--indigo)' },
    { label:'Fat',     value:totalFat,   color:'var(--amber)'  },
  ];

  const last7Cal = Array.from({length:7},(_,i)=>{
    const d=new Date(); d.setDate(d.getDate()-6+i);
    const ds=d.toISOString().slice(0,10);
    return { label:d.toLocaleDateString('en',{weekday:'narrow'}), value:meals.filter(m=>m.date===ds).reduce((s,m)=>s+m.calories,0) };
  });

  const MEAL_COLORS = { Breakfast:'var(--amber)', Lunch:'var(--mint)', Dinner:'var(--indigo)', Snack:'var(--pink)' };

  return (
    <div className="fade-up">
      <div className="page-title">Food & Hydration
        <div className="page-subtitle">{totalCals} kcal today · {todayWater}/8 glasses</div>
      </div>

      {/* Water */}
      <div className="card mb-4">
        <div style={{ display:'flex', justifyContent:'space-between', alignItems:'center', marginBottom:14 }}>
          <div className="card-title" style={{ marginBottom:0 }}>💧 Water Intake</div>
          <button className="btn btn-primary btn-sm" onClick={logWater}>
            <Icon name="droplet" size={13} color="#0a0d14"/>+1 Glass
          </button>
        </div>
        <div className="water-glasses">
          {Array.from({length:8},(_,i)=>(
            <div key={i} className={`water-glass${i<todayWater?' filled':''}`}
              onClick={()=>{ if(i>=todayWater) logWater(); }}
              title={`Glass ${i+1}`}/>
          ))}
        </div>
        <div style={{ fontSize:12, color:'var(--text2)', marginTop:10 }}>{todayWater}/8 glasses · {(todayWater*250)}ml</div>
      </div>

      {/* Log meal */}
      <div className="card mb-4">
        <div className="card-title">Log Meal</div>
        <div className="input-row mb-3">
          <div className="input-group" style={{ flex:2 }}>
            <label className="input-label">Meal</label>
            <input value={form.name} onChange={e=>setForm(p=>({...p,name:e.target.value}))} placeholder="e.g. Oats, Dal Rice..."/>
          </div>
          <div className="input-group">
            <label className="input-label">Type</label>
            <select value={form.type} onChange={e=>setForm(p=>({...p,type:e.target.value}))}>
              {['Breakfast','Lunch','Dinner','Snack'].map(t=><option key={t}>{t}</option>)}
            </select>
          </div>
        </div>
        <div className="input-row">
          <div className="input-group">
            <label className="input-label">Calories</label>
            <input type="number" value={form.calories} onChange={e=>setForm(p=>({...p,calories:e.target.value}))} placeholder="kcal" style={{ width:80 }}/>
          </div>
          <div className="input-group">
            <label className="input-label">Protein (g)</label>
            <input type="number" value={form.protein} onChange={e=>setForm(p=>({...p,protein:e.target.value}))} placeholder="g" style={{ width:80 }}/>
          </div>
          <div className="input-group">
            <label className="input-label">Carbs (g)</label>
            <input type="number" value={form.carbs} onChange={e=>setForm(p=>({...p,carbs:e.target.value}))} placeholder="g" style={{ width:80 }}/>
          </div>
          <div className="input-group">
            <label className="input-label">Fat (g)</label>
            <input type="number" value={form.fat} onChange={e=>setForm(p=>({...p,fat:e.target.value}))} placeholder="g" style={{ width:80 }}/>
          </div>
          <button className="btn btn-primary" onClick={logMeal} style={{ alignSelf:'flex-end' }}>Log Meal</button>
        </div>
      </div>

      <div className="grid-2 mb-4">
        {/* Macros */}
        <div className="card">
          <div className="card-title">Today's Macros</div>
          {macroData.some(d=>d.value>0) ? (
            <div className="donut-wrap">
              <DonutChart data={macroData.filter(d=>d.value>0)} size={100} thickness={12}/>
              <div className="donut-legend">
                {macroData.map(d=>(
                  <div key={d.label} className="donut-legend-item">
                    <div className="donut-dot" style={{ background:d.color }}/>
                    <span style={{ flex:1, color:'var(--text2)' }}>{d.label}</span>
                    <span style={{ fontWeight:600 }}>{d.value}g</span>
                  </div>
                ))}
                <div style={{ borderTop:'1px solid var(--border)', paddingTop:8, marginTop:4, display:'flex', justifyContent:'space-between' }}>
                  <span style={{ color:'var(--text2)', fontSize:12 }}>Calories</span>
                  <span style={{ fontWeight:700, color:'var(--mint)' }}>{totalCals} kcal</span>
                </div>
              </div>
            </div>
          ) : <p style={{ color:'var(--text3)', fontSize:13 }}>Log meals to see macros</p>}
        </div>

        {/* 7-day calories */}
        <div className="card">
          <div className="card-title">7-Day Calories</div>
          <BarChart data={last7Cal} color="var(--pink)" height={80}/>
        </div>
      </div>

      {/* Today's meals */}
      <div className="flex-col gap-2">
        {todayMeals.length===0 && (
          <div className="card" style={{ textAlign:'center', padding:32, color:'var(--text3)' }}>No meals logged today</div>
        )}
        {todayMeals.map(m=>(
          <div key={m.id} className="task-item">
            <div style={{ width:8,height:8,borderRadius:'50%',background:MEAL_COLORS[m.type]||'var(--mint)',flexShrink:0 }}/>
            <span className="badge" style={{ background:`color-mix(in srgb,${MEAL_COLORS[m.type]||'var(--mint)'} 15%,transparent)`, color:MEAL_COLORS[m.type]||'var(--mint)' }}>{m.type}</span>
            <span style={{ flex:1, fontSize:13 }}>{m.name}</span>
            {m.calories>0 && <span style={{ fontSize:12, fontWeight:600, color:'var(--mint)' }}>{m.calories} kcal</span>}
            {m.protein>0  && <span style={{ fontSize:11, color:'var(--mint)' }}>P:{m.protein}g</span>}
            {m.carbs>0    && <span style={{ fontSize:11, color:'var(--indigo)' }}>C:{m.carbs}g</span>}
            {m.fat>0      && <span style={{ fontSize:11, color:'var(--amber)' }}>F:{m.fat}g</span>}
            <button className="btn btn-danger btn-icon btn-sm" onClick={()=>delMeal(m.id)} style={{width:28,height:28}}>
              <Icon name="trash" size={12}/>
            </button>
          </div>
        ))}
      </div>
    </div>
  );
}

/* ================================================================
   NOTES PAGE
   ================================================================ */
function NotesPage({ notes, setNotes, toast }) {
  const [selectedDate, setSelectedDate] = useState(today());
  const [subject, setSubject]           = useState('General');
  const note = notes[selectedDate] || { text:'', subject:'General' };

  const save = (text) => {
    setNotes(p => ({ ...p, [selectedDate]: { text, subject } }));
  };

  const saveSubject = (s) => {
    setSubject(s);
    setNotes(p => ({ ...p, [selectedDate]: { ...(p[selectedDate]||{}), subject:s } }));
  };

  /* List of days with notes */
  const noteDates = Object.keys(notes).sort().reverse();

  return (
    <div className="fade-up">
      <div className="page-title">Notes
        <div className="page-subtitle">Daily study notes, organized by subject</div>
      </div>

      <div className="grid-2">
        {/* Editor */}
        <div>
          <div className="card mb-4">
            <div className="input-row mb-3" style={{ alignItems:'center' }}>
              <div className="input-group" style={{ flex:1 }}>
                <label className="input-label">Date</label>
                <input type="date" value={selectedDate} onChange={e=>{setSelectedDate(e.target.value);setSubject(notes[e.target.value]?.subject||'General');}}/>
              </div>
              <div className="input-group" style={{ flex:1 }}>
                <label className="input-label">Subject</label>
                <select value={subject} onChange={e=>saveSubject(e.target.value)}>
                  {NOTE_SUBJECTS.map(s=><option key={s}>{s}</option>)}
                </select>
              </div>
            </div>

            {/* Subject tags */}
            <div style={{ display:'flex', gap:6, flexWrap:'wrap', marginBottom:14 }}>
              {NOTE_SUBJECTS.map(s=>(
                <button key={s} className={`tag${subject===s?' active':''}`} onClick={()=>saveSubject(s)}>{s}</button>
              ))}
            </div>

            <textarea
              className="note-area"
              value={note.text}
              onChange={e=>save(e.target.value)}
              placeholder={`Start writing your ${subject} notes for ${fmtDate(selectedDate)}...\n\nTip: Use this space for class notes, summaries, key formulas, or anything you want to remember!`}
              style={{ height:320 }}
            />
            <div style={{ display:'flex', justifyContent:'space-between', marginTop:10, fontSize:12, color:'var(--text3)' }}>
              <span>{note.text.length} characters</span>
              <span style={{ color:'var(--mint)' }}>Auto-saved ✓</span>
            </div>
          </div>
        </div>

        {/* Sidebar — past notes */}
        <div>
          <div className="card">
            <div className="card-title">📓 Previous Notes ({noteDates.length})</div>
            {noteDates.length===0 && <p style={{ color:'var(--text3)', fontSize:13 }}>No notes yet. Start writing!</p>}
            <div className="flex-col gap-2" style={{ maxHeight:420, overflowY:'auto' }}>
              {noteDates.map(d => {
                const n = notes[d];
                const isSelected = d === selectedDate;
                return (
                  <div key={d}
                    onClick={()=>{ setSelectedDate(d); setSubject(n.subject||'General'); }}
                    style={{
                      padding:'12px 14px', borderRadius:12, cursor:'pointer',
                      background: isSelected ? 'rgba(110,231,183,0.1)' : 'var(--bg3)',
                      border: `1px solid ${isSelected?'var(--mint)':'var(--border)'}`,
                      transition:'all 0.2s',
                    }}>
                    <div style={{ display:'flex', justifyContent:'space-between', marginBottom:4 }}>
                      <span style={{ fontSize:12, fontWeight:600, color: isSelected?'var(--mint)':'var(--text)' }}>{fmtDate(d)}</span>
                      <span className="badge badge-indigo">{n.subject||'General'}</span>
                    </div>
                    <div style={{ fontSize:12, color:'var(--text3)', overflow:'hidden', display:'-webkit-box', WebkitLineClamp:2, WebkitBoxOrient:'vertical' }}>
                      {n.text?.slice(0,100)||'(empty)'}
                    </div>
                  </div>
                );
              })}
            </div>
          </div>
        </div>
      </div>
    </div>
  );
}

/* ── Mount ────────────────────────────────────────────────────── */
ReactDOM.createRoot(document.getElementById('app')).render(<App/>);
</script>
</body>
</html>
