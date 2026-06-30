<div align="center" style="display: none; visibility: hidden;">AI OS — Nikhil Rai</div>

<div style="background-color: #050505; color: #FFFFFF; font-family: -apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Inter', 'Segoe UI', Roboto, sans-serif; min-height: 100vh; padding: 0; margin: 0;">

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@300;400;500;600;700&display=swap');

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  :root {
    --bg-primary: #050505;
    --bg-secondary: #0B0B0B;
    --bg-tertiary: #111111;
    --glass: rgba(255,255,255,0.04);
    --glass-medium: rgba(255,255,255,0.06);
    --glass-heavy: rgba(255,255,255,0.10);
    --glass-border: rgba(255,255,255,0.08);
    --glass-border-hover: rgba(255,255,255,0.14);
    --text-primary: #FFFFFF;
    --text-secondary: #A1A1AA;
    --text-tertiary: #71717A;
    --text-muted: #52525B;
    --accent-blue: #4CC9F0;
    --accent-cyan: #22D3EE;
    --accent-purple: #8B5CF6;
    --accent-green: #34D399;
    --accent-amber: #FBBF24;
    --radius-sm: 6px;
    --radius-md: 10px;
    --radius-lg: 16px;
    --radius-xl: 24px;
    --radius-full: 9999px;
    --space-2: 8px;
    --space-3: 12px;
    --space-4: 16px;
    --space-5: 20px;
    --space-6: 24px;
    --space-8: 32px;
    --space-10: 40px;
    --space-12: 48px;
    --space-16: 64px;
    --space-20: 80px;
    --font-sans: -apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Inter', 'Segoe UI', Roboto, sans-serif;
    --font-display: 'Space Grotesk', -apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Inter', sans-serif;
  }

  body {
    background-color: var(--bg-primary);
    color: var(--text-primary);
    font-family: var(--font-sans);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  .os-container {
    max-width: 1100px;
    margin: 0 auto;
    padding: var(--space-8) var(--space-6);
    position: relative;
  }

  /* ===== GLASS CARD ===== */
  .glass-card {
    background: var(--glass);
    border: 1px solid var(--glass-border);
    border-radius: var(--radius-lg);
    padding: var(--space-6);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
    position: relative;
    overflow: hidden;
  }

  .glass-card:hover {
    background: var(--glass-medium);
    border-color: var(--glass-border-hover);
  }

  .glass-card-hero {
    background: linear-gradient(135deg, rgba(255,255,255,0.06) 0%, rgba(255,255,255,0.02) 100%);
    border: 1px solid rgba(255,255,255,0.10);
    border-radius: var(--radius-xl);
    padding: var(--space-10);
    backdrop-filter: blur(40px);
    -webkit-backdrop-filter: blur(40px);
    position: relative;
    overflow: hidden;
  }

  /* ===== GRID SYSTEM ===== */
  .bento-grid {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: var(--space-4);
    margin-top: var(--space-16);
  }

  .bento-grid:first-of-type {
    margin-top: 0;
  }

  .col-span-12 { grid-column: span 12; }
  .col-span-8 { grid-column: span 8; }
  .col-span-6 { grid-column: span 6; }
  .col-span-4 { grid-column: span 4; }
  .col-span-3 { grid-column: span 3; }

  /* ===== TYPOGRAPHY ===== */
  .text-hero {
    font-size: 52px;
    font-weight: 300;
    line-height: 1.1;
    letter-spacing: -0.03em;
    font-family: var(--font-display);
    color: var(--text-primary);
  }

  .text-h1 {
    font-size: 36px;
    font-weight: 300;
    line-height: 1.15;
    letter-spacing: -0.025em;
  }

  .text-h2 {
    font-size: 28px;
    font-weight: 300;
    line-height: 1.2;
    letter-spacing: -0.02em;
  }

  .text-h3 {
    font-size: 22px;
    font-weight: 400;
    line-height: 1.25;
    letter-spacing: -0.015em;
  }

  .text-h4 {
    font-size: 18px;
    font-weight: 400;
    line-height: 1.3;
    letter-spacing: -0.01em;
  }

  .text-body {
    font-size: 15px;
    font-weight: 400;
    line-height: 1.6;
    color: var(--text-secondary);
  }

  .text-small {
    font-size: 13px;
    font-weight: 400;
    line-height: 1.5;
    color: var(--text-tertiary);
  }

  .text-caption {
    font-size: 11px;
    font-weight: 500;
    line-height: 1.4;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    color: var(--text-tertiary);
  }

  .text-metric {
    font-size: 26px;
    font-weight: 300;
    line-height: 1;
    letter-spacing: -0.02em;
  }

  .accent-blue { color: var(--accent-blue); }
  .accent-cyan { color: var(--accent-cyan); }
  .accent-purple { color: var(--accent-purple); }
  .accent-green { color: var(--accent-green); }

  /* ===== SECTION HEADER ===== */
  .section-header {
    display: flex;
    align-items: center;
    gap: var(--space-3);
    margin-bottom: var(--space-5);
  }

  .section-header .icon-dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    display: inline-block;
  }

  .section-header .icon-dot.blue { background: var(--accent-blue); box-shadow: 0 0 12px rgba(76,201,240,0.3); }
  .section-header .icon-dot.cyan { background: var(--accent-cyan); box-shadow: 0 0 12px rgba(34,211,238,0.3); }
  .section-header .icon-dot.purple { background: var(--accent-purple); box-shadow: 0 0 12px rgba(139,92,246,0.3); }
  .section-header .icon-dot.green { background: var(--accent-green); box-shadow: 0 0 12px rgba(52,211,153,0.3); }

  .section-title {
    font-size: 13px;
    font-weight: 500;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    color: var(--text-tertiary);
  }

  /* ===== HERO ===== */
  .hero-layout {
    display: flex;
    align-items: center;
    gap: var(--space-10);
  }

  .hero-content {
    flex: 1;
    min-width: 0;
  }

  .hero-visual {
    flex-shrink: 0;
    width: 300px;
    height: 300px;
    position: relative;
  }

  .hero-visual img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .hero-subtitle {
    font-size: 17px;
    color: var(--text-secondary);
    margin-top: var(--space-3);
    line-height: 1.5;
    letter-spacing: -0.01em;
  }

  .hero-description {
    font-size: 15px;
    color: var(--text-tertiary);
    margin-top: var(--space-4);
    line-height: 1.7;
    max-width: 480px;
  }

  .hero-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: var(--space-3);
    margin-top: var(--space-6);
  }

  .hero-btn {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 8px 18px;
    border-radius: var(--radius-md);
    font-size: 13px;
    font-weight: 500;
    text-decoration: none;
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
    background: var(--glass);
    border: 1px solid var(--glass-border);
    color: var(--text-secondary);
  }

  .hero-btn:hover {
    background: var(--glass-medium);
    border-color: var(--glass-border-hover);
    color: var(--text-primary);
  }

  .hero-btn-primary {
    background: rgba(76,201,240,0.10);
    border-color: rgba(76,201,240,0.20);
    color: var(--accent-blue);
  }

  .hero-btn-primary:hover {
    background: rgba(76,201,240,0.15);
    border-color: rgba(76,201,240,0.30);
    color: var(--accent-blue);
  }

  /* ===== PROGRESS BARS ===== */
  .progress-item {
    margin-bottom: var(--space-4);
  }

  .progress-item:last-child {
    margin-bottom: 0;
  }

  .progress-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 6px;
  }

  .progress-label {
    font-size: 13px;
    color: var(--text-secondary);
  }

  .progress-value {
    font-size: 12px;
    color: var(--text-tertiary);
    font-weight: 500;
  }

  .progress-track {
    width: 100%;
    height: 3px;
    background: rgba(255,255,255,0.06);
    border-radius: var(--radius-full);
    overflow: hidden;
  }

  .progress-fill {
    height: 100%;
    border-radius: var(--radius-full);
    transition: width 1s cubic-bezier(0.16, 1, 0.3, 1);
    position: relative;
  }

  .progress-fill::after {
    content: '';
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
    width: 4px;
    height: 4px;
    border-radius: 50%;
  }

  .progress-fill.blue { background: linear-gradient(90deg, rgba(76,201,240,0.4), var(--accent-blue)); }
  .progress-fill.cyan { background: linear-gradient(90deg, rgba(34,211,238,0.4), var(--accent-cyan)); }
  .progress-fill.purple { background: linear-gradient(90deg, rgba(139,92,246,0.4), var(--accent-purple)); }
  .progress-fill.green { background: linear-gradient(90deg, rgba(52,211,153,0.4), var(--accent-green)); }
  .progress-fill.amber { background: linear-gradient(90deg, rgba(251,191,36,0.4), var(--accent-amber)); }

  /* ===== STAT CARDS ===== */
  .stat-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: var(--space-3);
    margin-top: var(--space-4);
  }

  .stat-item {
    text-align: center;
    padding: var(--space-3);
    background: rgba(255,255,255,0.02);
    border-radius: var(--radius-md);
    border: 1px solid rgba(255,255,255,0.04);
  }

  .stat-value {
    font-size: 24px;
    font-weight: 300;
    line-height: 1;
    letter-spacing: -0.02em;
  }

  .stat-label {
    font-size: 11px;
    color: var(--text-tertiary);
    margin-top: 4px;
    letter-spacing: 0.03em;
    text-transform: uppercase;
  }

  /* ===== TECH GRID ===== */
  .tech-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: var(--space-3);
    margin-top: var(--space-4);
  }

  .tech-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 6px;
    padding: var(--space-3) var(--space-2);
    border-radius: var(--radius-md);
    background: rgba(255,255,255,0.02);
    border: 1px solid rgba(255,255,255,0.04);
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .tech-item:hover {
    background: var(--glass);
    border-color: var(--glass-border);
  }

  .tech-item img {
    width: 24px;
    height: 24px;
    opacity: 0.7;
    transition: opacity 0.3s ease;
  }

  .tech-item:hover img {
    opacity: 1;
  }

  .tech-item span {
    font-size: 10px;
    color: var(--text-tertiary);
    text-align: center;
    line-height: 1.2;
  }

  /* ===== PROJECT CARDS ===== */
  .project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: var(--space-4);
    margin-top: var(--space-4);
  }

  .project-card {
    padding: var(--space-6);
    border-radius: var(--radius-lg);
    background: var(--glass);
    border: 1px solid var(--glass-border);
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
    position: relative;
    overflow: hidden;
  }

  .project-card:hover {
    background: var(--glass-medium);
    border-color: var(--glass-border-hover);
    transform: translateY(-2px);
  }

  .project-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, rgba(76,201,240,0.2), transparent);
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .project-card:hover::before {
    opacity: 1;
  }

  .project-card h3 {
    font-size: 17px;
    font-weight: 500;
    color: var(--text-primary);
    margin-bottom: var(--space-2);
    letter-spacing: -0.01em;
  }

  .project-card p {
    font-size: 13px;
    color: var(--text-tertiary);
    line-height: 1.6;
    margin-bottom: var(--space-4);
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    margin-bottom: var(--space-4);
  }

  .project-tag {
    padding: 3px 10px;
    border-radius: var(--radius-full);
    font-size: 10px;
    font-weight: 500;
    color: var(--text-tertiary);
    background: rgba(255,255,255,0.04);
    border: 1px solid rgba(255,255,255,0.06);
    letter-spacing: 0.02em;
  }

  .project-link {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 6px 14px;
    border-radius: var(--radius-sm);
    font-size: 12px;
    font-weight: 500;
    color: var(--accent-blue);
    background: rgba(76,201,240,0.08);
    border: 1px solid rgba(76,201,240,0.15);
    text-decoration: none;
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .project-link:hover {
    background: rgba(76,201,240,0.12);
    border-color: rgba(76,201,240,0.25);
  }

  .project-reserved {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 180px;
    text-align: center;
  }

  .project-reserved .reserved-icon {
    font-size: 32px;
    opacity: 0.15;
    margin-bottom: var(--space-3);
    line-height: 1;
  }

  .project-reserved h3 {
    opacity: 0.4;
    margin-bottom: var(--space-1);
  }

  .project-reserved p {
    opacity: 0.25;
    font-size: 12px;
  }

  /* ===== CONNECT ===== */
  .connect-grid {
    display: flex;
    flex-wrap: wrap;
    gap: var(--space-3);
    margin-top: var(--space-4);
  }

  .connect-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 10px 20px;
    border-radius: var(--radius-md);
    font-size: 14px;
    font-weight: 400;
    color: var(--text-secondary);
    background: var(--glass);
    border: 1px solid var(--glass-border);
    text-decoration: none;
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .connect-link:hover {
    background: var(--glass-medium);
    border-color: var(--glass-border-hover);
    color: var(--text-primary);
  }

  .connect-link svg {
    width: 18px;
    height: 18px;
    opacity: 0.7;
  }

  /* ===== FOOTER ===== */
  .os-footer {
    text-align: center;
    padding: var(--space-12) 0 var(--space-8);
    border-top: 1px solid rgba(255,255,255,0.04);
    margin-top: var(--space-16);
  }

  .os-footer .footer-brand {
    font-size: 13px;
    font-weight: 500;
    color: var(--text-tertiary);
    margin-bottom: var(--space-2);
  }

  .os-footer .footer-brand span {
    color: var(--accent-blue);
  }

  .os-footer .footer-sub {
    font-size: 11px;
    color: var(--text-muted);
  }

  .status-indicator {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 4px 12px;
    border-radius: var(--radius-full);
    font-size: 11px;
    font-weight: 500;
    background: rgba(52,211,153,0.08);
    border: 1px solid rgba(52,211,153,0.15);
    color: var(--accent-green);
  }

  .status-indicator .dot {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: var(--accent-green);
    animation: pulse-dot 2s ease-in-out infinite;
  }

  @keyframes pulse-dot {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.3; }
  }

  /* ===== WIDGETS CONTAINER ===== */
  .widget-container {
    width: 100%;
    overflow: hidden;
    border-radius: var(--radius-md);
    margin-top: var(--space-4);
  }

  .widget-container img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: var(--radius-md);
  }

  /* ===== STATS ROW ===== */
  .stats-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: var(--space-4);
    margin-top: var(--space-4);
  }

  .stats-row img {
    width: 100%;
    height: auto;
    border-radius: var(--radius-md);
  }

  /* ===== ABOUT CONTENT ===== */
  .about-content {
    margin-top: var(--space-3);
  }

  .about-content p {
    font-size: 14px;
    color: var(--text-secondary);
    line-height: 1.7;
  }

  .about-content p + p {
    margin-top: var(--space-3);
  }

  /* ===== MISSION CARD ===== */
  .mission-content {
    margin-top: var(--space-3);
  }

  .mission-badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 4px 12px;
    border-radius: var(--radius-full);
    font-size: 11px;
    font-weight: 500;
    background: rgba(76,201,240,0.08);
    border: 1px solid rgba(76,201,240,0.15);
    color: var(--accent-blue);
    margin-bottom: var(--space-4);
  }

  .mission-list {
    list-style: none;
    padding: 0;
  }

  .mission-list li {
    display: flex;
    align-items: flex-start;
    gap: var(--space-3);
    padding: var(--space-2) 0;
    font-size: 13px;
    color: var(--text-secondary);
    border-bottom: 1px solid rgba(255,255,255,0.04);
  }

  .mission-list li:last-child {
    border-bottom: none;
  }

  .mission-list li .mission-icon {
    flex-shrink: 0;
    width: 16px;
    height: 16px;
    margin-top: 2px;
    opacity: 0.5;
  }

  /* ===== SNAKE CONTAINER ===== */
  .snake-container {
    width: 100%;
    margin-top: var(--space-4);
    border-radius: var(--radius-md);
    overflow: hidden;
  }

  .snake-container img {
    width: 100%;
    height: auto;
    display: block;
  }

  /* ===== FOOTER STATUS ROW ===== */
  .footer-status {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: var(--space-6);
    flex-wrap: wrap;
  }

  .footer-status span {
    font-size: 12px;
    color: var(--text-muted);
  }

  .footer-status .divider {
    width: 1px;
    height: 12px;
    background: rgba(255,255,255,0.08);
  }

  /* ===== RESPONSIVE ===== */
  @media (max-width: 1024px) {
    .col-span-4, .col-span-3, .col-span-6, .col-span-8 {
      grid-column: span 6;
    }
    .hero-visual {
      width: 200px;
      height: 200px;
    }
    .text-hero {
      font-size: 40px;
    }
  }

  @media (max-width: 768px) {
    .bento-grid {
      grid-template-columns: repeat(4, 1fr);
    }
    .col-span-4, .col-span-3, .col-span-6, .col-span-8, .col-span-12 {
      grid-column: span 4;
    }
    .hero-layout {
      flex-direction: column;
      text-align: center;
    }
    .hero-description {
      max-width: 100%;
    }
    .hero-buttons {
      justify-content: center;
    }
    .hero-visual {
      width: 160px;
      height: 160px;
    }
    .text-hero {
      font-size: 32px;
    }
    .project-grid {
      grid-template-columns: 1fr;
    }
    .stats-row {
      grid-template-columns: 1fr;
    }
    .stat-grid {
      grid-template-columns: 1fr 1fr;
    }
    .os-container {
      padding: var(--space-4);
    }
    .glass-card-hero {
      padding: var(--space-6);
    }
    .hero-subtitle {
      font-size: 15px;
    }
    .tech-grid {
      grid-template-columns: repeat(3, 1fr);
    }
    .connect-grid {
      justify-content: center;
    }
  }

  @media (max-width: 480px) {
    .text-hero {
      font-size: 26px;
    }
    .hero-visual {
      width: 120px;
      height: 120px;
    }
    .glass-card-hero {
      padding: var(--space-4);
    }
    .tech-grid {
      grid-template-columns: repeat(3, 1fr);
    }
    .stat-grid {
      grid-template-columns: 1fr 1fr;
    }
    .hero-buttons {
      flex-direction: column;
      align-items: center;
    }
    .hero-btn {
      width: 100%;
      justify-content: center;
    }
    .footer-status {
      flex-direction: column;
      gap: var(--space-2);
    }
    .footer-status .divider {
      display: none;
    }
  }

  /* ===== ANIMATIONS ===== */
  @keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-6px); }
  }

  .float-anim {
    animation: float 6s ease-in-out infinite;
  }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(10px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .fade-in {
    animation: fadeIn 0.6s cubic-bezier(0.16, 1, 0.3, 1) forwards;
  }

  .fade-in-delay-1 { animation-delay: 0.1s; }
  .fade-in-delay-2 { animation-delay: 0.2s; }
  .fade-in-delay-3 { animation-delay: 0.3s; }
  .fade-in-delay-4 { animation-delay: 0.4s; }

  @keyframes glow-pulse {
    0%, 100% { opacity: 0.3; }
    50% { opacity: 0.6; }
  }

  .glow-pulse {
    animation: glow-pulse 4s ease-in-out infinite;
  }

  /* ===== TYPING CURSOR ===== */
  @keyframes blink {
    0%, 100% { opacity: 1; }
    50% { opacity: 0; }
  }

  .typing-cursor::after {
    content: '|';
    color: var(--accent-blue);
    animation: blink 1s step-end infinite;
    font-weight: 300;
    margin-left: 2px;
  }

  /* ===== SCROLLBAR ===== */
  ::-webkit-scrollbar {
    width: 6px;
    height: 6px;
  }
  ::-webkit-scrollbar-track {
    background: var(--bg-primary);
  }
  ::-webkit-scrollbar-thumb {
    background: rgba(255,255,255,0.08);
    border-radius: 3px;
  }
  ::-webkit-scrollbar-thumb:hover {
    background: rgba(255,255,255,0.12);
  }

  /* ===== UTILITY ===== */
  .mt-2 { margin-top: var(--space-2); }
  .mt-4 { margin-top: var(--space-4); }
  .mt-6 { margin-top: var(--space-6); }
  .mt-8 { margin-top: var(--space-8); }
  .mb-4 { margin-bottom: var(--space-4); }
  .mb-6 { margin-bottom: var(--space-6); }

  .bg-gradient-glow {
    position: absolute;
    top: -50%;
    left: -20%;
    width: 140%;
    height: 200%;
    background: radial-gradient(ellipse at center, rgba(76,201,240,0.03) 0%, transparent 60%);
    pointer-events: none;
  }

  /* ===== MISSION PROGRESS OVERRIDE ===== */
  .learning-item .progress-fill {
    height: 3px;
    border-radius: var(--radius-full);
  }
</style>

<!-- ===== BACKGROUND PARTICLES ===== -->
<img src="assets/svg/particles-bg.svg" alt="" style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: 0; pointer-events: none; opacity: 0.6;">

<img src="assets/svg/glow-gradient.svg" alt="" style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: 0; pointer-events: none;">

<!-- ===== OS CONTAINER ===== -->
<div class="os-container" style="position: relative; z-index: 1;">

  <!-- ============================== -->
  <!-- HERO SECTION                   -->
  <!-- ============================== -->
  <div class="glass-card-hero fade-in">
    <div class="bg-gradient-glow"></div>
    <div class="hero-layout">
      <div class="hero-content">
        <div style="display: flex; align-items: center; gap: 10px; margin-bottom: var(--space-3);">
          <span class="status-indicator">
            <span class="dot"></span>
            AI OS v1.0
          </span>
          <span class="text-caption" style="color: var(--text-muted);">· Control Center</span>
        </div>
        <h1 class="text-hero" style="margin: 0;">
          Nikhil Rai
        </h1>
        <div class="hero-subtitle">
          AI Engineer · Agentic Systems · Research Infrastructure
        </div>
        <p class="hero-description">
          Building autonomous AI systems that reason, retrieve, and accelerate scientific research. Focused on compound AI architectures and production-grade agentic frameworks.
        </p>
        <div class="hero-buttons">
          <a href="https://github.com/Nikhilrai27" class="hero-btn hero-btn-primary" target="_blank" rel="noopener">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
            GitHub
          </a>
          <a href="https://linkedin.com/in/nikhilrai27" class="hero-btn" target="_blank" rel="noopener">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
            LinkedIn
          </a>
          <a href="#" class="hero-btn" target="_blank" rel="noopener">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></svg>
            Portfolio
          </a>
          <a href="mailto:nikhilrai27@example.com" class="hero-btn">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
            Email
          </a>
        </div>
      </div>
      <div class="hero-visual float-anim">
        <img src="assets/svg/hero-neural-network.svg" alt="Neural network visualization">
      </div>
    </div>
  </div>

  <!-- ============================== -->
  <!-- BENTO GRID ROW 1               -->
  <!-- ============================== -->
  <div class="bento-grid">

    <!-- ABOUT -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-1" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot purple"></span>
          <span class="section-title">About</span>
        </div>
        <div class="about-content">
          <p>
            AI Engineer with deep expertise in building production-grade agentic systems, RAG pipelines, and research automation infrastructure.
          </p>
          <p>
            Currently architecting compound AI systems that combine retrieval, reasoning, and tool use for scientific discovery.
          </p>
        </div>
      </div>
    </div>

    <!-- AI CORE STATUS -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-1" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot blue"></span>
          <span class="section-title">AI Core Status</span>
        </div>
        <div style="margin-top: var(--space-3);">
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">ResearchOS</span>
              <span class="progress-value">92%</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill blue" style="width: 92%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">LangGraph</span>
              <span class="progress-value">85%</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill cyan" style="width: 85%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">FastAPI</span>
              <span class="progress-value">82%</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill purple" style="width: 82%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">RAG Systems</span>
              <span class="progress-value">88%</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill green" style="width: 88%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">Docker</span>
              <span class="progress-value">70%</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill amber" style="width: 70%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">MCP Protocol</span>
              <span class="progress-value">65%</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill blue" style="width: 65%;"></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- GITHUB STATS -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-2" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot cyan"></span>
          <span class="section-title">GitHub Analytics</span>
        </div>
        <div class="stats-row">
          <img src="https://github-readme-stats.vercel.app/api?username=Nikhilrai27&show_icons=true&theme=transparent&hide_border=true&bg_color=050505&text_color=A1A1AA&title_color=4CC9F0&icon_color=4CC9F0&hide=contribs&card_width=300&custom_title=" alt="GitHub Stats" loading="lazy">
          <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nikhilrai27&layout=compact&theme=transparent&hide_border=true&bg_color=050505&text_color=A1A1AA&title_color=4CC9F0&card_width=300&custom_title=" alt="Top Languages" loading="lazy">
        </div>
      </div>
    </div>

  </div>

  <!-- ============================== -->
  <!-- CONTRIBUTION GRAPH             -->
  <!-- ============================== -->
  <div class="bento-grid">
    <div class="col-span-12">
      <div class="glass-card fade-in fade-in-delay-2">
        <div class="section-header">
          <span class="icon-dot green"></span>
          <span class="section-title">Contribution Graph</span>
        </div>
        <div class="snake-container">
          <picture>
            <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nikhilrai27/Nikhilrai27/output/github-contribution-grid-snake-dark.svg" />
            <img src="https://raw.githubusercontent.com/Nikhilrai27/Nikhilrai27/output/github-contribution-grid-snake.svg" alt="GitHub contribution snake animation" loading="lazy" />
          </picture>
        </div>
      </div>
    </div>
  </div>

  <!-- ============================== -->
  <!-- BENTO GRID ROW 2               -->
  <!-- ============================== -->
  <div class="bento-grid">

    <!-- STREAK -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-2" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot amber" style="background: var(--accent-amber); box-shadow: 0 0 12px rgba(251,191,36,0.3);"></span>
          <span class="section-title">Current Streak</span>
        </div>
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Nikhilrai27&theme=transparent&hide_border=true&background=050505&stroke=71717A&ring=4CC9F0&fire=4CC9F0&currStreakNum=FFFFFF&sideNums=A1A1AA&currStreakLabel=71717A&sideLabels=71717A&dates=52525B" alt="GitHub Streak" style="width: 100%; height: auto; margin-top: var(--space-3); border-radius: var(--radius-md);" loading="lazy">
      </div>
    </div>

    <!-- ACTIVITY GRAPH -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-3" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot blue"></span>
          <span class="section-title">Activity</span>
        </div>
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=Nikhilrai27&theme=github-dark&bg_color=050505&color=A1A1AA&line=4CC9F0&point=4CC9F0&area=true&area_color=4CC9F0&hide_border=true&custom_title=" alt="GitHub Activity Graph" style="width: 100%; height: auto; margin-top: var(--space-3); border-radius: var(--radius-md);" loading="lazy">
      </div>
    </div>

    <!-- TECH STACK -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-3" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot purple"></span>
          <span class="section-title">Tech Stack</span>
        </div>
        <div class="tech-grid">
          <div class="tech-item">
            <img src="assets/svg/icons/python.svg" alt="Python" loading="lazy">
            <span>Python</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/fastapi.svg" alt="FastAPI" loading="lazy">
            <span>FastAPI</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/langchain.svg" alt="LangChain" loading="lazy">
            <span>LangChain</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/langgraph.svg" alt="LangGraph" loading="lazy">
            <span>LangGraph</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/docker.svg" alt="Docker" loading="lazy">
            <span>Docker</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/postgresql.svg" alt="PostgreSQL" loading="lazy">
            <span>PostgreSQL</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/qdrant.svg" alt="Qdrant" loading="lazy">
            <span>Qdrant</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/git.svg" alt="Git" loading="lazy">
            <span>Git</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/linux.svg" alt="Linux" loading="lazy">
            <span>Linux</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/openai.svg" alt="OpenAI" loading="lazy">
            <span>OpenAI</span>
          </div>
          <div class="tech-item">
            <img src="assets/svg/icons/gemini.svg" alt="Gemini" loading="lazy">
            <span>Gemini</span>
          </div>
          <div class="tech-item" style="border-color: rgba(255,255,255,0.02); opacity: 0.3; cursor: default;">
            <span style="font-size: 18px;">+</span>
            <span>More</span>
          </div>
        </div>
      </div>
    </div>

  </div>

  <!-- ============================== -->
  <!-- FEATURED PROJECTS              -->
  <!-- ============================== -->
  <div class="bento-grid">
    <div class="col-span-12">
      <div class="glass-card fade-in fade-in-delay-3">
        <div class="section-header">
          <span class="icon-dot cyan"></span>
          <span class="section-title">Featured Projects</span>
        </div>
        <div class="project-grid">
          <div class="project-card">
            <h3>ResearchOS</h3>
            <p>AI-powered research operating system that coordinates multiple LLM agents for autonomous literature review, hypothesis generation, and experimental design.</p>
            <div class="project-tags">
              <span class="project-tag">LangGraph</span>
              <span class="project-tag">FastAPI</span>
              <span class="project-tag">RAG</span>
              <span class="project-tag">Qdrant</span>
            </div>
            <a href="https://github.com/Nikhilrai27" class="project-link" target="_blank" rel="noopener">
              <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
              Repository
            </a>
          </div>
          <div class="project-card">
            <h3>Resume Analyzer</h3>
            <p>ATS-optimized resume analysis platform using multi-agent evaluation, semantic matching, and AI-powered recommendations for career growth.</p>
            <div class="project-tags">
              <span class="project-tag">LLM</span>
              <span class="project-tag">FastAPI</span>
              <span class="project-tag">Docker</span>
              <span class="project-tag">PostgreSQL</span>
            </div>
            <a href="https://github.com/Nikhilrai27" class="project-link" target="_blank" rel="noopener">
              <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
              Repository
            </a>
          </div>
          <div class="project-card">
            <div class="project-reserved">
              <div class="reserved-icon">◆</div>
              <h3>Future Project</h3>
              <p>Space reserved for next-generation AI research infrastructure.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- ============================== -->
  <!-- BENTO GRID ROW 3               -->
  <!-- ============================== -->
  <div class="bento-grid">

    <!-- LEARNING ROADMAP -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-4" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot green"></span>
          <span class="section-title">Learning Roadmap</span>
        </div>
        <div style="margin-top: var(--space-3);">
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">CrewAI Multi-Agent</span>
              <span class="progress-value">In Progress</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill blue" style="width: 40%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">Rust Fundamentals</span>
              <span class="progress-value">Getting Started</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill cyan" style="width: 15%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">Kubernetes</span>
              <span class="progress-value">Planning</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill amber" style="width: 10%;"></div>
            </div>
          </div>
          <div class="progress-item">
            <div class="progress-header">
              <span class="progress-label">RLHF & Alignment</span>
              <span class="progress-value">Exploring</span>
            </div>
            <div class="progress-track">
              <div class="progress-fill green" style="width: 25%;"></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- CONNECT -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-4" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot blue"></span>
          <span class="section-title">Connect</span>
        </div>
        <p style="font-size: 13px; color: var(--text-tertiary); margin-top: var(--space-3); line-height: 1.6;">
          Open to collaborations on AI research infrastructure, agentic systems, and developer tooling.
        </p>
        <div class="connect-grid">
          <a href="https://github.com/Nikhilrai27" class="connect-link" target="_blank" rel="noopener">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
            GitHub
          </a>
          <a href="https://linkedin.com/in/nikhilrai27" class="connect-link" target="_blank" rel="noopener">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
            LinkedIn
          </a>
          <a href="https://x.com/nikhilrai27" class="connect-link" target="_blank" rel="noopener">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4l11.733 16h4.267l-11.733 -16zM4 20l6.768 -6.768M19.5 4l-6.768 6.768"/></svg>
            X / Twitter
          </a>
          <a href="mailto:nikhilrai27@example.com" class="connect-link">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
            Email
          </a>
        </div>
      </div>
    </div>

    <!-- QUICK METRICS -->
    <div class="col-span-4">
      <div class="glass-card fade-in fade-in-delay-4" style="height: 100%;">
        <div class="section-header">
          <span class="icon-dot purple"></span>
          <span class="section-title">System Metrics</span>
        </div>
        <div class="stat-grid">
          <div class="stat-item">
            <div class="stat-value accent-blue">24</div>
            <div class="stat-label">Repositories</div>
          </div>
          <div class="stat-item">
            <div class="stat-value accent-cyan">847</div>
            <div class="stat-label">Contributions</div>
          </div>
          <div class="stat-item">
            <div class="stat-value accent-purple">12</div>
            <div class="stat-label">Stars Earned</div>
          </div>
          <div class="stat-item">
            <div class="stat-value accent-green">3</div>
            <div class="stat-label">Active Projects</div>
          </div>
        </div>
      </div>
    </div>

  </div>

  <!-- ============================== -->
  <!-- FOOTER                         -->
  <!-- ============================== -->
  <div class="os-footer">
    <div class="footer-status">
      <span class="status-indicator">
        <span class="dot"></span>
        System Online
      </span>
      <span class="divider"></span>
      <span>AI OS · Control Center v1.0</span>
      <span class="divider"></span>
      <span>Uptime: ∞</span>
      <span class="divider"></span>
      <span>Latency: 0ms</span>
    </div>
    <div style="margin-top: var(--space-6);">
      <div class="footer-brand">Nikhil Rai · <span>AI OS</span></div>
      <div class="footer-sub">Designed with precision · Built with purpose</div>
    </div>
  </div>

</div>

</div>
