/* styles.css — design léger et réactif pour CIYOTA CLUB */
:root{
  --bg: #f7f8fb;
  --card: #ffffff;
  --accent: #0b6b63;
  --muted: #6b7280;
  --radius: 12px;
  --container: 1000px;
  --gap: 18px;
  font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  color-scheme: light;
}

*{box-sizing:border-box}
html,body{height:100%}
body{
  margin:0;
  background:var(--bg);
  color:#0f172a;
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
  line-height:1.5;
  font-size:16px;
}

/* container centré */
.container{
  width: calc(100% - 32px);
  max-width: var(--container);
  margin: 0 auto;
  padding: 28px 0;
}

/* header */
.site-header{
  background:linear-gradient(90deg, rgba(11,107,99,0.95), rgba(6,86,73,0.9));
  color:#fff;
  position:sticky;
  top:0;
  z-index:50;
  box-shadow: 0 2px 6px rgba(2,6,23,0.08);
}
.header-inner{display:flex;align-items:center;justify-content:space-between;gap:12px}
.logo{font-weight:700;letter-spacing:0.6px}
.logo .club{font-weight:400;opacity:0.9}

/* nav */
.nav a{color:#e6fffb;text-decoration:none;margin-left:14px;font-weight:600;font-size:0.95rem}
.nav a:hover{opacity:0.9;transform:translateY(-1px)}

/* hero */
.hero{
  padding:48px 0;
  background:
    radial-gradient(600px 140px at 10% 10%, rgba(11,107,99,0.06), transparent 10%),
    linear-gradient(180deg, transparent 0%, transparent 60%, rgba(11,107,99,0.02) 100%);
}
.hero h1{margin:0 0 10px;font-size:clamp(1.6rem, 3.6vw, 2.4rem)}
.hero p{margin:0 0 16px;color:var(--muted)}

/* buttons */
.btn{
  display:inline-block;
  padding:10px 16px;
  border-radius:10px;
  background:var(--accent);
  color:#fff;
  text-decoration:none;
  font-weight:600;
  border:0;
  cursor:pointer;
}
.btn.ghost{background:transparent;border:1px solid rgba(11,107,99,0.12);color:var(--accent)}
.btn:hover{transform:translateY(-3px);box-shadow:0 8px 20px rgba(11,107,99,0.08)}

/* cards & layout */
.card{background:var(--card);border-radius:var(--radius);padding:20px;box-shadow:0 6px 20px rgba(2,6,23,0.04);margin-bottom:18px}
.grid h2{margin-top:0}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;margin-top:12px}
.service{padding:16px;border-radius:10px;background:linear-gradient(180deg,#fff,#fbfcfe);border:1px solid rgba(15,23,42,0.03)}

/* form */
.contact-form{display:grid;gap:10px;max-width:640px}
.contact-form label{display:flex;flex-direction:column;font-size:0.95rem;color:var(--muted)}
.contact-form input,
.contact-form textarea{
  margin-top:8px;padding:10px;border-radius:8px;border:1px solid #e6e9ef;background:#fff;resize:vertical;
}
.form-row{margin-top:6px}

/* footer */
.site-footer{padding:16px 0;background:transparent}
.footer-inner{display:flex;align-items:center;justify-content:space-between;gap:12px;color:var(--muted);font-size:0.9rem}
.social a{margin-left:12px;text-decoration:none;color:var(--muted)}

/* responsive tweaks */
@media (max-width:720px){
  .header-inner{flex-direction:row;align-items:center}
  .nav{display:none}
  .hero{padding:36px 0}
  .footer-inner{flex-direction:column;gap:8px;text-align:center}
}
