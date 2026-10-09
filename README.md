<!--
    Ehasan07 / Ehasan07 — GitHub profile README
    Renders at https://github.com/Ehasan07
-->

<p align="center">
  <img src="assets/hero.png" alt="S M Ehasanul Haque — Odoo and full-stack developer, Dhaka" width="100%">
</p>

<p align="center">
  <a href="https://ehasanlive.com"><img src="https://img.shields.io/badge/Portfolio-ehasanlive.com-0B7A6F?style=for-the-badge" alt="Portfolio"></a>
  <a href="https://mycard.dupno.com/card/shiplu07/"><img src="https://img.shields.io/badge/Digital%20card-MY--Card-C8A24A?style=for-the-badge" alt="Digital card"></a>
  <a href="https://dupno.com"><img src="https://img.shields.io/badge/Building%20at-DUPNO-10201E?style=for-the-badge" alt="DUPNO"></a>
</p>

## Hi, I'm Ehasan

I'm an **Odoo and full-stack developer at DUPNO International** in Dhaka. At work I build Odoo 12 modules for the company's vehicle-tracking (VTS) operations — the fleet register, SIM recharge, voice campaigns, tracking certificates, equipment handover and the call-centre desk. Outside them I build Bangla-first SaaS: a Hajj agency platform, a personal finance app, a trading ERP and a digital business card.

A few rules I hold to in every project:

- **Bangla first**, English one tap away.
- **Money is counted in paisa**, never in floating point — totals match to the last taka.
- **Never break the system next door**: an add-on must not slow down or block the module it sits on.
- **It ships**: tested, deployed on a real server, with backups.

<br>

## Odoo modules at DUPNO

<sub>Company work, so the source is private. Screens are from the modules themselves; customer data is blurred.</sub>

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/odoo-fleet.png" alt="VTS Fleet 2.0">
      <br><b>VTS Fleet 2.0</b> — a 19,000-row Google Sheet behind a real register: every edit goes through approval, keeps an audit trail and is written back to its exact cell.
      <br><sub>Python · Odoo ORM · Google Apps Script write-back API · cron retries</sub>
    </td>
    <td width="50%" valign="top">
      <img src="assets/odoo-recharge.png" alt="Dupno Mobile Recharge">
      <br><b>Mobile Recharge</b> — bulk top-ups for the SIMs inside GPS trackers: the operator is read from the number prefix, employees spend from wallets with limits, and the ledger is checked against the live balance.
      <br><sub>SSL Wireless TopUp API · wallets · computed fields with search</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/odoo-voice.png" alt="VTS SMS Voice Clean">
      <br><b>Voice SMS in Bengali</b> — a renewal reminder as a phone call: one rendered audio file per customer, uploaded to the voice server, dialled, then matched against the carrier's call records.
      <br><sub>Google Cloud TTS · SSML · SFTP (paramiko) · queue API · CDR reconciliation</sub>
    </td>
    <td width="50%" valign="top">
      <img src="assets/odoo-certificate.png" alt="Dupno GPS Certificate">
      <br><b>GPS Certificate</b> — the BRTA / BTRC vehicle tracking certificate: type the IMEI and the rest fills itself; a Bengali PDF with a QR code that checks the live status.
      <br><sub>QWeb PDF · Bengali typeface · QR verification endpoint · onchange</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/odoo-assets.png" alt="Smart Mobility Asset">
      <br><b>Asset Handover</b> — who holds which tracker, tool or SIM pack: a handover counts only when both sides sign, open tasks block the close, and what isn't returned becomes a liability.
      <br><sub>hr · mail · state workflows · record rules</sub>
    </td>
    <td width="50%" valign="top">
      <img src="assets/odoo-desk.png" alt="VTS IPTSP Support Desk">
      <br><b>Call Support Desk</b> — an editable mirror of the PBX call records for call-centre agents, with problem tags and vehicle links, written so it can never make the PBX lose a call.
      <br><sub>Asterisk PBX · inherited create · non-blocking mirror · chatter</sub>
    </td>
  </tr>
</table>

<details>
<summary><b>What I do in Odoo</b></summary>
<br>

| Area | In these modules |
|---|---|
| Models and ORM | New models, inheritance of existing ones, computed fields with `search`, onchange, constraints |
| Views | Kanban, list, form and search views in XML; menus and actions per role |
| Reports | QWeb PDF in Bengali with seals and QR codes |
| Security | Groups, access rights, record rules, approval workflows with audit trails |
| Automation | Scheduled actions (cron) for sync, retries, balance checks and reconciliation |
| Integrations | Google Sheets / Apps Script, SSL Wireless, Google Cloud TTS, SFTP, Asterisk PBX, REST endpoints |

<p><img src="assets/odoo-fleet-collection.png" alt="VTS Fleet 2.0 collection targets, data blurred" width="100%"></p>
</details>

<br>

## Products I built

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/Ehasan07/hajj-tracking-software"><img src="assets/hajj-tracking-software.png" alt="Hajj Tracking"></a>
      <br><b>Hajj Tracking</b> — SaaS for Hajj &amp; Umrah agencies: pilgrims, QR-verified receipts, statements, payroll, hotels and four side shops.
      <br><a href="https://hajj.takatracker.com">Live</a> · <a href="https://github.com/Ehasan07/hajj-tracking-software">Code</a> · <sub>Next.js · tRPC · PostgreSQL</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/Ehasan07/takatracker"><img src="assets/takatracker.png" alt="Taka Tracker"></a>
      <br><b>Taka Tracker</b> — offline-first, double-entry personal accounting for Bangladesh, in Bangla and English.
      <br><a href="https://takatracker.com">Live</a> · <a href="https://github.com/Ehasan07/takatracker">Code</a> · <sub>Next.js · NestJS · Prisma</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/erp.png" alt="Trade ERP">
      <br><b>Trade ERP</b> — accounting, stock and VAT for rod, cement, sand, paint, aluminium and glass traders. Bangla first, double-entry, works on a phone.
      <br><sub>Next.js · Prisma · PostgreSQL · private client work, client name hidden</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://mycard.dupno.com"><img src="assets/mycard.png" alt="MY-Card"></a>
      <br><b>MY-Card</b> — digital business cards: live builder, QR and wallet passes, bKash and SSLCommerz payments, analytics.
      <br><a href="https://mycard.dupno.com">Live</a> · <sub>Django · PostgreSQL · source private</sub>
    </td>
  </tr>
</table>

<details>
<summary><b>More from Trade ERP</b></summary>
<br>
<p>
  <img src="assets/erp-stock.png" alt="Trade ERP stock summary" width="49%">
  <img src="assets/erp-trial-balance.png" alt="Trade ERP trial balance" width="49%">
</p>
</details>

<br>

## Client web work for DUPNO

<table>
  <tr>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/dupno-payment"><img src="assets/dupno-payment.png" alt="DUPNO Payment Portal"></a>
      <br><b>Payment Portal</b><br><sub>Checkout page for DUPNO services</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/Dupno-fuel-monitor"><img src="assets/Dupno-fuel-monitor.png" alt="DUPNO Fuel Monitor"></a>
      <br><b>Fuel Monitor</b><br><sub>Landing page for vehicle fuel monitoring</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/Dupno-table-filter"><img src="assets/Dupno-table-filter.png" alt="Service Comparison"></a>
      <br><b>Service Comparison</b><br><sub>Bangla package table, filtered by vehicle</sub>
    </td>
  </tr>
</table>

<br>

## Web apps, games and experiments

<table>
  <tr>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/Protfolio"><img src="assets/Protfolio.png" alt="ehasanlive.com"></a>
      <br><b>ehasanlive.com</b><br><sub>Bilingual portfolio · React, Tailwind, Framer Motion</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/V-card"><img src="assets/V-card.png" alt="Digital E-Card"></a>
      <br><b>Digital E-Card</b><br><sub>Live card builder with QR and .vcf</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/React-World-Tour"><img src="assets/React-World-Tour.png" alt="React World Tour"></a>
      <br><b>React World Tour</b><br><sub>Every country from a REST API</sub>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/Alphabate-game"><img src="assets/Alphabate-game.png" alt="Alpha Clash Pro"></a>
      <br><b>Alpha Clash Pro</b><br><sub>Keyboard typing game</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/tic-tac-toe-game"><img src="assets/tic-tac-toe-game.png" alt="Tic-Tac-Toe"></a>
      <br><b>Tic-Tac-Toe</b><br><sub>Two players, vanilla JavaScript</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/Book-management-project"><img src="assets/Book-management-project.png" alt="Book Manager"></a>
      <br><b>Book Manager</b><br><sub>Python command-line app</sub>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/Mouse-hover"><img src="assets/Mouse-hover.png" alt="Fluid Smoke Pro"></a>
      <br><b>Fluid Smoke Pro</b><br><sub>Canvas animation</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/hexagonal-grid-interaction"><img src="assets/hexagonal-grid-interaction.png" alt="Hexagon Grid"></a>
      <br><b>Hexagon Grid</b><br><sub>Honeycomb hover effect</sub>
    </td>
    <td width="33%" valign="top">
      <a href="https://github.com/Ehasan07/fluid-hover"><img src="assets/fluid-hover.png" alt="Fluid Hover"></a>
      <br><b>Fluid Hover</b> · <a href="https://github.com/Ehasan07/interesting-cursor-hover">Cursor Trails</a><br><sub>More canvas experiments</sub>
    </td>
  </tr>
</table>

<br>

## How I got here

| When | What I was building |
|---|---|
| **Jan 2024** | [First repository](https://github.com/Ehasan07/my-frist-github-repo), [first portfolio](https://github.com/Ehasan07/web-developer-portfolio), and assignment 1: a [Figma design in HTML](https://github.com/Ehasan07/My-frist-assignment) |
| **Jan – May 2024** | Assignments 2–6: [AMA Travel](https://github.com/Ehasan07/2nd-assignment-), [Hockey Club](https://github.com/Ehasan07/3rd-assignment), [JS problem solving](https://github.com/Ehasan07/4th-assignment), [P-Paribahan tickets](https://github.com/Ehasan07/5th-assignment), [Retro Forum](https://github.com/Ehasan07/6th-assignment) |
| **2024** | First games and React: [Alpha Clash Pro](https://github.com/Ehasan07/Alphabate-game), [Tic-Tac-Toe](https://github.com/Ehasan07/tic-tac-toe-game), [React World Tour](https://github.com/Ehasan07/React-World-Tour) · first client pages for DUPNO |
| **At DUPNO** | Odoo 12 modules for the VTS operations: fleet register, SIM recharge, Bengali voice campaigns, tracking certificates, asset handover, call-centre desk |
| **2025** | Python, canvas experiments, the [Digital E-Card](https://github.com/Ehasan07/V-card), then **MY-Card**, a Django SaaS with payments |
| **2026** | [ehasanlive.com](https://ehasanlive.com) rebuilt, **Taka Tracker**, **Trade ERP** and **Hajj Tracking** — full SaaS products in TypeScript, live on my own servers |

<br>

## Tools I use

<p>
  <img src="https://img.shields.io/badge/Odoo%2012-714B67?style=flat-square&logo=odoo&logoColor=white" alt="Odoo 12">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/QWeb%20%2F%20XML-875A7B?style=flat-square" alt="QWeb / XML">
  <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" alt="Django">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
</p>
<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js">
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React">
  <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" alt="NestJS">
  <img src="https://img.shields.io/badge/tRPC-2596BE?style=flat-square&logo=trpc&logoColor=white" alt="tRPC">
  <img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma">
  <img src="https://img.shields.io/badge/Drizzle-C5F74F?style=flat-square&logo=drizzle&logoColor=black" alt="Drizzle">
  <img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
</p>
<p>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white" alt="Nginx">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright">
  <img src="https://img.shields.io/badge/Hetzner-D50C2D?style=flat-square&logo=hetzner&logoColor=white" alt="Hetzner">
  <img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud">
  <img src="https://img.shields.io/badge/bKash-E2136E?style=flat-square" alt="bKash">
  <img src="https://img.shields.io/badge/SSLCommerz-1B4F8F?style=flat-square" alt="SSLCommerz">
</p>

<br>

## Get in touch

<p>
  <a href="https://ehasanlive.com"><img src="https://img.shields.io/badge/Website-ehasanlive.com-0B7A6F?style=for-the-badge" alt="Website"></a>
  <a href="https://mycard.dupno.com/card/shiplu07/"><img src="https://img.shields.io/badge/Card-mycard.dupno.com-C8A24A?style=for-the-badge" alt="Digital card"></a>
  <a href="https://dupno.com"><img src="https://img.shields.io/badge/Company-DUPNO-10201E?style=for-the-badge" alt="DUPNO"></a>
</p>

<p align="center"><sub>Ship it. Read it six months later. If it still makes sense, it's done.</sub></p>
