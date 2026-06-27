---
theme: default
title: From Author to Orchestrator
info: |
  ## How AI redefined the software engineer
  A 25-minute lecture for year 1–3 CS students. Evidence over hype.
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
colorSchema: dark
fonts:
  sans: IBM Plex Sans
  serif: Space Grotesk
  mono: JetBrains Mono
  weights: '400,500,600,700'
---

<div class="h-full flex flex-col justify-center">

<div class="eyebrow"><span class="i">//</span>&nbsp; the role is being rewritten</div>

<h1 style="margin-top:1.1rem; font-size:3.6rem;">From <span class="h-acc">Author</span><br>to <span class="a-acc">Orchestrator</span></h1>

<div style="font-size:1.3rem; color:var(--muted); margin-top:1rem; max-width:42ch;">
How AI redefined what a software engineer is <b style="color:var(--ink)">for</b>.
</div>

<div class="src" style="margin-top:2.6rem;">a 25-minute field guide &nbsp;·&nbsp; evidence over hype</div>

</div>

<!--
**What this talk is:** not hype — a careful read of the evidence. The core idea: in about three years the job shifted from writing code yourself to directing and checking AI that writes it. As code gets cheap, your value moves to intent, judgment, verification, and being accountable for the result (Alenezi, 2026).

**How to frame it:** tell them you'll deliberately show *contradicting* studies — one says AI makes you much faster, another says it makes you slower. Holding both is the whole point.

**Live prompt:** "Hands up — who used an AI tool to write code this week? Keep your hand up if you read every line it produced." (Most hands drop on the second half — that's your trust/verification theme.)
-->

---
title: "Your speaker"
---

<div class="h-full flex items-center" style="gap:3.4rem;">
  <img src="/profile-photo.jpg" alt="Abdellah Iraamane" style="flex-shrink:0; width:232px; height:232px; border-radius:50%; object-fit:cover; border:1px solid var(--line); box-shadow:0 0 0 6px var(--bg), 0 0 0 7px var(--line);" />
  <div>
    <div class="eyebrow"><span class="i">//</span>&nbsp; your speaker</div>
    <h1 style="margin-top:1rem; font-size:3rem;">Abdellah <span class="h-acc">Iraamane</span></h1>
    <div style="font-size:1.25rem; color:var(--ink); margin-top:.9rem; font-family:'Space Grotesk'; font-weight:500;">Senior Software Engineer <span style="color:var(--faint);">·</span> <span style="color:var(--muted);">Microsoft</span></div>
    <div style="font-size:.98rem; color:var(--muted); margin-top:.6rem;">Master IADO FSR <span style="color:var(--faint);">·</span> Promo 2015</div>
    <div style="font-size:.98rem; color:var(--muted); margin-top:.2rem;">MSc Software Project Management <span style="color:var(--faint);">·</span> University of Sussex</div>
    <div style="display:flex; gap:.7rem; margin-top:1.4rem;"><span class="chip" style="border-color:var(--agent); color:var(--agent);">Agentic AI</span><span class="chip" style="border-color:var(--agent); color:var(--agent);">Applied AI</span></div>
  </div>
</div>

<!--
**Who's talking:** Abdellah Iraamane — Senior Software Engineer at Microsoft, working on Agentic and Applied AI. A quick 30-second intro: what you build day-to-day, and why the shift from writing code to orchestrating it is something you live, not just study. Then bridge in: "I work on the systems this talk is about — so let's look at what the evidence actually says."
-->

---
title: "The timeline"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 02</span> &nbsp; the timeline</div>
<h2 style="margin-top:.6rem;">Three paradigms. Three years.</h2>
</div>

<div class="body items-center">
<div style="display:grid; grid-template-columns:repeat(3,1fr); gap:1.6rem; width:100%; position:relative;">

  <div style="position:absolute; top:7px; left:10%; right:10%; height:2px; background:linear-gradient(90deg,var(--human),var(--line) 55%,var(--agent)); opacity:.6;"></div>

  <div style="position:relative;">
    <div style="width:15px;height:15px;border-radius:50%;background:var(--human);box-shadow:0 0 0 5px var(--bg),0 0 0 6px var(--line);margin-bottom:1.4rem;"></div>
    <div class="src h-acc">2022 · assisted</div>
    <div style="font-family:'Space Grotesk';font-size:1.35rem;font-weight:600;margin:.25rem 0;">AI autocompletes</div>
    <div style="color:var(--muted);font-size:.95rem;">You are the author.</div>
    <div class="chip" style="margin-top:.8rem;">unit: lines</div>
  </div>

  <div style="position:relative;">
    <div style="width:15px;height:15px;border-radius:50%;background:#8a93b0;box-shadow:0 0 0 5px var(--bg),0 0 0 6px var(--line);margin-bottom:1.4rem;"></div>
    <div class="src" style="color:#8a93b0;">~2023 · generative</div>
    <div style="font-family:'Space Grotesk';font-size:1.35rem;font-weight:600;margin:.25rem 0;">AI drafts on request</div>
    <div style="color:var(--muted);font-size:.95rem;">Functions, tests, docs.</div>
    <div class="chip" style="margin-top:.8rem;">unit: blocks</div>
  </div>

  <div style="position:relative;">
    <div style="width:15px;height:15px;border-radius:50%;background:var(--agent);box-shadow:0 0 0 5px var(--bg),0 0 0 6px var(--agent);margin-bottom:1.4rem;"></div>
    <div class="src a-acc">now · agentic</div>
    <div style="font-family:'Space Grotesk';font-size:1.35rem;font-weight:600;margin:.25rem 0;">AI ships end-to-end</div>
    <div style="color:var(--muted);font-size:.95rem;">Reads issues, edits, opens PRs.</div>
    <div class="chip" style="margin-top:.8rem; border-color:var(--agent); color:var(--agent);">unit: pull requests</div>
  </div>

</div>
</div>

<div class="foot">
  <div class="takeaway"><b class="a-acc">932,791</b> pull requests authored by agents, across 116,211 real repos. This is production, not a demo.</div>
  <div class="src">src: AIDev 2026 · Alenezi 2026</div>
</div>
</div>

<!--
**Reading the timeline** (three dots, left → right) — three eras in ~3 years:

- **2022 · assisted** — Copilot autocompletes; you write the code, AI finishes your lines. Unit of work = *lines*. You're the author.
- **~2023 · generative** — you ask in plain language; the AI drafts whole functions, tests, docs. Unit of work = *blocks* on request.
- **now · agentic** — the AI reads an issue, edits files, runs tests, opens a pull request itself. Unit of work = *whole PRs*.

**The big number (bottom):** 932,791 pull requests were authored by AI agents across 116,211 real repositories (AIDev, 2026). Say it plainly: nearly a million PRs written by software, not people, in real production projects — proof this is happening now, not a demo.

**Prompt:** "If the unit of work is now a PR an agent wrote, what is the human actually contributing to that PR?"
-->

---
title: "The capability leap"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 03</span> &nbsp; the capability leap</div>
<h2 style="margin-top:.6rem;">In one year, AI went from <span class="a-acc">4%</span> to <span class="a-acc">72%</span>.</h2>
</div>

<div class="body items-end justify-center" style="gap:4.5rem; padding-bottom:.5rem;">
  <div style="text-align:center;">
    <div class="stat" style="font-size:1.7rem; color:var(--muted); margin-bottom:.6rem;">4.4%</div>
    <div style="width:96px; height:13px; background:var(--line); border-radius:6px 6px 0 0;"></div>
    <div class="src" style="margin-top:.7rem;">2023</div>
  </div>

  <div style="align-self:center; font-size:2.4rem; color:var(--agent); transform:translateY(-30px);">↗</div>

  <div style="text-align:center;">
    <div class="stat" style="font-size:2.8rem; color:var(--agent); margin-bottom:.6rem;">71.7%</div>
    <div style="width:96px; height:198px; background:linear-gradient(180deg,var(--agent),#2c7e74); border-radius:6px 6px 0 0;"></div>
    <div class="src" style="margin-top:.7rem;">2024</div>
  </div>
</div>

<div class="foot">
  <div class="takeaway">Share of real GitHub issues solved on <b>SWE-bench</b>. The improvement is genuine — and steep.</div>
  <div class="src">src: Stanford 2025 · SWE-agent 2024</div>
</div>
</div>

<!--
**Reading the chart:** two bars — short one (2023) = 4.4%, tall one (2024) = 71.7%. This is **SWE-bench**: the AI is handed REAL bug reports from real GitHub projects and must produce a fix that passes the project's own tests. So the % = "share of genuine issues it solved end-to-end."

**Say it plainly:** in one year AI went from solving about 1 in 20 real issues to roughly 7 in 10 (Stanford, 2025). Frontier agents in late 2025/26 sit around 75–80%. The jump is real and steep.

**Why it jumped:** AI gained the ability to "use the computer" — open files, search the repo, run tests (SWE-agent, 2024) — and splitting work across specialized sub-agents pushed it further (MASAI, 2024).

**Cliffhanger (sets up next slide):** "These numbers make it look like the job is almost solved. Hold that thought."

**Prompt:** "A benchmark says an AI solves 80% of issues. What would you need to know before you trust that number?"
-->

---
title: "The benchmark caveat"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 04</span> &nbsp; the caveat</div>
<h2 style="margin-top:.6rem;">…80% doesn't mean 80%.</h2>
</div>

<div class="body flex-col justify-center" style="gap:1.8rem; max-width:660px;">
  <div>
    <div style="display:flex; justify-content:space-between; align-items:baseline; margin-bottom:.45rem;">
      <span class="src">popular benchmark</span>
      <span class="stat a-acc" style="font-size:1.5rem;">~80%</span>
    </div>
    <div style="height:20px; background:var(--line); border-radius:10px;">
      <div style="width:80%; height:100%; background:var(--agent); border-radius:10px;"></div>
    </div>
  </div>

  <div>
    <div style="display:flex; justify-content:space-between; align-items:baseline; margin-bottom:.45rem;">
      <span class="src">contamination-resistant test</span>
      <span class="stat w-acc" style="font-size:1.5rem;">~23%</span>
    </div>
    <div style="height:20px; background:var(--line); border-radius:10px;">
      <div style="width:23%; height:100%; background:var(--warn); border-radius:10px;"></div>
    </div>
  </div>
</div>

<div class="foot">
  <div class="takeaway"><b>Same models.</b> Harder, decontaminated test. Headline capability numbers are marketing-adjacent — interrogate the methodology.</div>
  <div class="src">src: Scale AI / SWE-bench Pro · Ganhotra 2025</div>
</div>
</div>

<!--
**Reading the two bars:** same AI models, two different tests. Top (~80%) = the popular benchmark everyone quotes. Bottom (~23%) = a harder, contamination-resistant version (SWE-bench Pro / Scale AI).

**The two problems, in plain English:**

- **Data contamination** — the test questions (or near-identical ones) leaked into the AI's training data, so it has effectively "seen the exam." Give it fresh problems and the score drops.
- **Saturation** — the easy problems are already solved by everyone, so the headline benchmark can't tell good models from great ones anymore (Ganhotra, 2025).

**The point:** capability is real and rising, but the ~80% in marketing can become ~23% on a clean test. Headline numbers are marketing-adjacent — engineers interrogate the methodology before believing them.

**Prompt:** "Who benefits from the higher number being the one that gets quoted in the press?"
-->

---
title: "Productivity — the optimistic case"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 05</span> &nbsp; productivity · the optimistic case</div>
<h2 style="margin-top:.6rem;">The case that AI makes us faster.</h2>
</div>

<div class="body flex-col justify-center">
  <div class="stat h-acc" style="font-size:7rem;">55.8%<span style="font-size:2rem; color:var(--muted); font-weight:500;"> faster</span></div>
  <div style="color:var(--muted); margin-top:.5rem; font-size:1.05rem;">on a well-defined, brand-new task &nbsp;·&nbsp; 95% CI 21–89%</div>
  <div class="chip" style="margin-top:1.5rem;">biggest gains&nbsp;→&nbsp;<b style="color:var(--ink)">less experienced</b>&nbsp;developers</div>
</div>

<div class="foot">
  <div class="takeaway">A rigorous, randomized, statistically significant trial. AI lowers the barrier for newcomers.</div>
  <div class="src">src: Peng et al. 2023 · GitHub–Accenture</div>
</div>
</div>

<!--
**The big stat:** 55.8% faster. In a randomized controlled trial (split people into "with Copilot" vs "without," same task), the Copilot group finished ~56% faster (Peng et al., 2023).

**Explain "95% CI 21–89%":** the confidence interval — the honest range the true effect likely sits in. It's wide, but stays well above zero, so the speed-up is real, not noise. Present this study sincerely — it's rigorous and statistically significant.

**The chip ("biggest gains → less experienced devs"):** the people who sped up most were newcomers — AI lowers the barrier for beginners. A separate enterprise trial at Accenture saw +84% more successful builds.

**Set the trap for next slide:** note WHAT the task was — a brand-new, well-defined HTTP server. Greenfield, clear spec. Remember that when the next study contradicts this one.

**Prompt:** "What's different about writing a brand-new HTTP server vs fixing a bug in a 1-million-line codebase you've maintained for years?"
-->

---
title: "Productivity — the surprise"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 06</span> &nbsp; productivity · the surprise</div>
<h2 style="margin-top:.6rem;">The study that surprised everyone.</h2>
</div>

<div class="body items-center justify-center">
<svg viewBox="0 0 640 230" style="width:100%; max-width:640px;">
  <!-- bracket -->
  <path d="M196 64 L196 54 L430 54 L430 64" fill="none" stroke="var(--faint)" stroke-width="1.5"/>
  <text x="313" y="44" text-anchor="middle" font-family="JetBrains Mono" font-size="14" fill="var(--ink)">≈ 39-point gap</text>
  <text x="313" y="30" text-anchor="middle" font-family="JetBrains Mono" font-size="10.5" fill="var(--faint)" letter-spacing="1.5">FEELING vs FACT</text>

  <!-- zero line -->
  <line x1="313" y1="78" x2="313" y2="190" stroke="var(--faint)" stroke-width="1" stroke-dasharray="3 4"/>
  <text x="313" y="206" text-anchor="middle" font-family="JetBrains Mono" font-size="10" fill="var(--faint)">0%</text>

  <!-- reality bar (left, slower) -->
  <rect x="199" y="92" width="114" height="48" rx="3" fill="var(--warn)"/>
  <text x="190" y="112" text-anchor="end" font-family="Space Grotesk" font-weight="700" font-size="22" fill="var(--warn)">−19%</text>
  <text x="190" y="130" text-anchor="end" font-family="IBM Plex Sans" font-size="12" fill="var(--muted)">actually slower</text>

  <!-- perception bar (right, felt faster) -->
  <rect x="313" y="92" width="120" height="48" rx="3" fill="var(--human)"/>
  <text x="442" y="112" text-anchor="start" font-family="Space Grotesk" font-weight="700" font-size="22" fill="var(--human)">+20%</text>
  <text x="442" y="130" text-anchor="start" font-family="IBM Plex Sans" font-size="12" fill="var(--muted)">they felt faster</text>
</svg>
</div>

<div class="foot">
  <div class="takeaway">Experienced devs in mature repos were <b class="w-acc">slower</b> with AI — and couldn't perceive it. Developers are unreliable narrators of their own speed.</div>
  <div class="src">src: METR 2025</div>
</div>
</div>

<!--
**Reading the chart:** a zero line down the middle. **Red bar points left = −19%** (reality). **Amber bar points right = +20%** (what they *felt*). The bracket on top labels the distance: a ~39-point gap between feeling and fact.

**What happened:** METR ran the same kind of rigorous randomized trial as the last slide — but on EXPERIENCED developers in big, mature codebases they already knew. With AI they were actually ~19% **slower**, yet afterward estimated they'd been ~20% **faster** (METR, 2025).

**The key lesson (say it slowly):** developers are unreliable narrators of their own speed. They felt faster and were slower — and couldn't tell. That perception gap is the most important takeaway in the deck.

**Why slower:** time lost writing prompts, waiting on the model, and reviewing/fixing its output; they accepted fewer than 44% of suggestions.

**Reconcile with slide 5 — both are good science.** The difference is context: slide 5 was a new, simple task with juniors; this is a complex, familiar codebase with seniors. Same tool, opposite result.

**Live prompt (~2 min):** "Two rigorous trials reached opposite conclusions the same year. Before you call one wrong — what would have to differ for BOTH to be right?" Steer to: task novelty, codebase maturity, experience level.
-->

---
title: "Adoption vs trust"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 07</span> &nbsp; adoption vs trust</div>
<h2 style="margin-top:.6rem;">Everyone uses it. Fewer trust it.</h2>
</div>

<div class="body items-center justify-center">
<svg viewBox="0 0 500 250" style="width:100%; max-width:540px;">
  <!-- legend -->
  <circle cx="64" cy="20" r="5" fill="var(--agent)"/>
  <text x="76" y="24" font-family="JetBrains Mono" font-size="12" fill="var(--muted)">adoption</text>
  <circle cx="180" cy="20" r="5" fill="var(--warn)"/>
  <text x="192" y="24" font-family="JetBrains Mono" font-size="12" fill="var(--muted)">trust in accuracy</text>

  <!-- baseline -->
  <line x1="60" y1="222" x2="440" y2="222" stroke="var(--line)" stroke-width="1"/>
  <text x="60" y="240" font-family="JetBrains Mono" font-size="11" fill="var(--faint)">2024</text>
  <text x="440" y="240" text-anchor="end" font-family="JetBrains Mono" font-size="11" fill="var(--faint)">2025</text>

  <!-- adoption line: 76% -> 84% -->
  <line x1="60" y1="86" x2="420" y2="71" stroke="var(--agent)" stroke-width="3" stroke-linecap="round"/>
  <circle cx="60" cy="86" r="4.5" fill="var(--agent)"/>
  <circle cx="420" cy="71" r="5.5" fill="var(--agent)"/>
  <text x="52" y="78" text-anchor="end" font-family="JetBrains Mono" font-size="12" fill="var(--muted)">76%</text>
  <text x="430" y="66" font-family="Space Grotesk" font-weight="700" font-size="20" fill="var(--agent)">84%</text>

  <!-- trust line: 40% -> 29% -->
  <line x1="60" y1="147" x2="420" y2="166" stroke="var(--warn)" stroke-width="3" stroke-linecap="round"/>
  <circle cx="60" cy="147" r="4.5" fill="var(--warn)"/>
  <circle cx="420" cy="166" r="5.5" fill="var(--warn)"/>
  <text x="52" y="151" text-anchor="end" font-family="JetBrains Mono" font-size="12" fill="var(--muted)">40%</text>
  <text x="430" y="171" font-family="Space Grotesk" font-weight="700" font-size="20" fill="var(--warn)">29%</text>
</svg>
</div>

<div class="foot">
  <div class="takeaway">Adoption and trust moving in opposite directions. <b>"Almost right"</b> is the expensive failure mode — and verifying it is now a paid skill.</div>
  <div class="src">src: Stack Overflow Developer Survey 2025</div>
</div>
</div>

<!--
**Reading the two lines (2024 → 2025):** the **teal** line is **adoption**, rising 76% → 84% (more developers using AI). The **red** line is **trust** in the AI's accuracy, falling 40% → 29%. They move in opposite directions — that's the whole point: usage up, trust down at the same time (Stack Overflow, 2025).

**The "almost right" problem (plain English):** 66% of devs are frustrated by output that's *almost* correct, and 45% say debugging AI code takes LONGER than writing it themselves. Why it's expensive: code that's 90% right can cost more to fix than starting fresh, because first you have to find the hidden 10% that's wrong. That's why verifying AI output is becoming a paid skill.

**Prompt:** "Why would a tool people distrust MORE still get adopted MORE? What does that tell you about workplace incentives?"
-->

---
title: "The quality paradox"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 08</span> &nbsp; the quality paradox</div>
<h2 style="margin-top:.6rem;">Individual speed <span style="color:var(--faint)">≠</span> team stability.</h2>
</div>

<div class="body flex-col justify-center" style="gap:1.1rem;">
  <div style="display:grid; grid-template-columns:repeat(4,1fr); gap:.9rem;">
    <div class="panel" style="padding:.9rem 1rem;">
      <div class="stat a-acc" style="font-size:1.7rem;">▲ 3.4%</div>
      <div class="src" style="margin-top:.35rem;">code quality</div>
    </div>
    <div class="panel" style="padding:.9rem 1rem;">
      <div class="stat a-acc" style="font-size:1.7rem;">▲ 7.5%</div>
      <div class="src" style="margin-top:.35rem;">documentation</div>
    </div>
    <div class="panel" style="padding:.9rem 1rem;">
      <div class="stat w-acc" style="font-size:1.7rem;">▼ 1.5%</div>
      <div class="src" style="margin-top:.35rem;">throughput</div>
    </div>
    <div class="panel" style="padding:.9rem 1rem;">
      <div class="stat w-acc" style="font-size:1.7rem;">▼ 7.2%</div>
      <div class="src" style="margin-top:.35rem;">delivery stability</div>
    </div>
  </div>
  <div style="display:flex; gap:.8rem; flex-wrap:wrap; margin-top:.4rem;">
    <span class="chip"><b style="color:var(--warn)">27.67%</b> of agent PRs → merge conflicts</span>
    <span class="chip">the <b style="color:var(--ink)">Confidence Trap</b>: confident PRs still break</span>
  </div>
</div>

<div class="foot">
  <div class="takeaway">Per +25% AI adoption (DORA). Faster individuals ≠ more reliable shipping. An agent's confidence is <b>not</b> a safety signal.</div>
  <div class="src">src: DORA 2024 · Ferdous et al. 2026</div>
</div>
</div>

<!--
**Reading the four cards** (per +25% more AI adoption — Google's DORA study, 2024):

- **code quality ▲ 3.4%** — the individual code looks a bit better.
- **documentation ▲ 7.5%** — also up.
- **throughput ▼ 1.5%** — the team ships slightly *less*.
- **delivery stability ▼ 7.2%** — and what ships breaks / needs fixing *more* often.

**The paradox (say it plainly):** making individuals write code faster and cleaner does NOT automatically make the team ship more reliably. Speed at the keyboard ≠ stability of the system — two arrows up, two arrows down, together.

**The two chips:**

- **27.67% of agent PRs hit merge conflicts** (Ogenrwot & Businge, 2026) — they collide with other changes.
- **The Confidence Trap** — agents sound confident even when their PRs are wrong; confidence is NOT a safety signal, especially in refactoring/maintenance (Ferdous et al., 2026). This is where technical debt quietly piles up.

**Live prompt (~2 min):** "If AI improves individual code quality but reduces system-level stability, where is the harm actually created — and who's accountable for it?" (Bridges into the next slide on ownership.)
-->

---
title: "The redefinition"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 09</span> &nbsp; the redefinition</div>
<h2 style="margin-top:.6rem;">From authorship to orchestration.</h2>
</div>

<div class="body items-center" style="gap:1.5rem;">
  <div class="panel" style="flex:1; padding:1.4rem 1.5rem; opacity:.75;">
    <div class="src" style="margin-bottom:.9rem;">yesterday</div>
    <div style="font-family:'Space Grotesk'; font-size:1.15rem; line-height:1.9; color:var(--muted);">
      Write the code<br>Ship lines<br>You are the <b style="color:var(--muted)">author</b>
    </div>
  </div>

  <div style="font-size:2rem; color:var(--human);">→</div>

  <div class="panel" style="flex:1; padding:1.4rem 1.5rem; border-color:var(--human);">
    <div class="src h-acc" style="margin-bottom:.9rem;">today</div>
    <div style="font-family:'Space Grotesk'; font-size:1.15rem; line-height:1.9; color:var(--ink);">
      Direct &amp; verify systems<br>Configs are the new specs<br>You own the <b class="h-acc">liability</b>
    </div>
  </div>
</div>

<div class="foot">
  <div class="takeaway">The role is changing, not vanishing. A good config file <b>is</b> engineering — and you're accountable for code you didn't type.</div>
  <div class="src">src: Alenezi 2026 · Santos 2025 · Treude 2026</div>
</div>
</div>

<!--
**Reading the two panels:** left (faded) = **yesterday** — write the code, ship lines, you're the author. Right (highlighted) = **today** — direct and verify systems, write the configs that tell agents what to do, own the liability. The arrow between them is the whole talk in one image: authorship → orchestration.

**The two new things, in plain English:**

- **Configs are the new specs** — telling an agent precisely how to behave (its architecture, rules, guardrails) is now real engineering. Researchers studied 328 of these config files and found genuine engineering decisions inside (Santos et al., 2025).
- **You own the liability** — the fine print (Terms of Service) of these tools pushes responsibility onto YOU. If the agent's code causes harm, that's on you, even if you didn't type it (Treude, 2026).

**Reframe the anxiety:** the role is changing, not disappearing. The skill set broadens into five areas — technical, cognitive, socio-technical, governance, organizational (Alenezi, 2026).

**Prompt:** "If you're legally and professionally responsible for an agent's code, how much should you trust it before you ship?"
-->

---
title: "The hard part — labor market"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 10</span> &nbsp; the hard part · labor market</div>
<h2 style="margin-top:.6rem;">Canaries in the coal mine.</h2>
</div>

<div class="body items-center justify-center" style="gap:5rem;">
  <!-- juniors: -16% -->
  <div style="text-align:center;">
    <div style="height:120px; display:flex; align-items:flex-start; justify-content:center;">
      <div style="width:80px; height:96px; background:linear-gradient(180deg,var(--warn),#7d3640); border-radius:0 0 6px 6px;"></div>
    </div>
    <div class="stat w-acc" style="font-size:2.2rem; margin-top:.4rem;">−16%</div>
    <div class="src" style="margin-top:.5rem; max-width:140px;">workers aged 22–25, AI-exposed jobs</div>
  </div>

  <!-- baseline divider -->
  <div style="width:1px; height:150px; background:var(--line);"></div>

  <!-- experienced: stable -->
  <div style="text-align:center;">
    <div style="height:120px; display:flex; align-items:flex-end; justify-content:center;">
      <div style="width:80px; height:8px; background:var(--human); border-radius:6px;"></div>
    </div>
    <div class="stat h-acc" style="font-size:2.2rem; margin-top:.4rem;">~0%</div>
    <div class="src" style="margin-top:.5rem; max-width:140px;">experienced workers, same jobs</div>
  </div>
</div>

<div class="foot">
  <div class="takeaway">AI helps juniors do the work — yet erodes the junior roles where people <b>learn the craft</b>. (Caveat: rates &amp; over-hiring also bit; pay still rose for most roles.)</div>
  <div class="src">src: Stanford / ADP payroll 2025</div>
</div>
</div>

<!--
**Reading the two bars:** left (red, tall, dropping) = young workers aged **22–25** in AI-exposed jobs saw a **16% relative drop** in employment. Right (amber, flat) = **experienced** workers in the SAME jobs stayed basically flat (~0%). This is real payroll data (ADP via Stanford, 2025), not a survey.

**"Relative decline," plain English:** compared with similar workers in jobs AI can't do, young workers in exposed jobs fell behind by ~16%. The damage clusters where AI *automates* the work (replaces the person) rather than *augments* it (helps the person).

**The structural trap (the hard part — be honest, this matters most to them):** AI is best at exactly the entry-level tasks juniors used to learn on. If those vanish, the on-ramp to becoming senior narrows.

**Don't doom-spiral — the caveats:** high interest rates and post-pandemic over-hiring also shrank tech jobs, and pay actually ROSE for most developer roles, so demand for skilled engineers continues. Someone still has to direct the AI.

**Capstone prompt (~2–3 min, pairs):** "If AI removes the tasks juniors learned on, how does anyone become a senior? Design one concrete fix — for a university, a company, or yourself." Then share-outs. Protect time for this one.
-->

---
title: "What this means for you"
---

<div class="scaffold">
<div class="head">
<div class="eyebrow"><span class="i">// 11</span> &nbsp; what this means for you</div>
<h2 style="margin-top:.6rem;">Be the engineer the field still needs.</h2>
</div>

<div class="body items-center">
<div style="display:grid; grid-template-columns:1fr 1fr; gap:1rem; width:100%;">
  <div class="panel" style="padding:1.05rem 1.2rem;">
    <div class="src h-acc">01 · verify</div>
    <div style="font-family:'Space Grotesk'; font-size:1.15rem; font-weight:600; margin:.3rem 0 .15rem;">Review like it's yours</div>
    <div style="color:var(--muted); font-size:.92rem;">The "almost right" bug is yours to catch.</div>
  </div>
  <div class="panel" style="padding:1.05rem 1.2rem;">
    <div class="src h-acc">02 · fundamentals</div>
    <div style="font-family:'Space Grotesk'; font-size:1.15rem; font-weight:600; margin:.3rem 0 .15rem;">Don't skip the basics</div>
    <div style="color:var(--muted); font-size:.92rem;">Depth is how you spot the Confidence Trap.</div>
  </div>
  <div class="panel" style="padding:1.05rem 1.2rem;">
    <div class="src a-acc">03 · specify</div>
    <div style="font-family:'Space Grotesk'; font-size:1.15rem; font-weight:600; margin:.3rem 0 .15rem;">Say intent precisely</div>
    <div style="color:var(--muted); font-size:.92rem;">Configs, constraints, requirements.</div>
  </div>
  <div class="panel" style="padding:1.05rem 1.2rem;">
    <div class="src a-acc">04 · trust slowly</div>
    <div style="font-family:'Space Grotesk'; font-size:1.15rem; font-weight:600; margin:.3rem 0 .15rem;">Start low-stakes</div>
    <div style="color:var(--muted); font-size:.92rem;">Progressive trust; mind shadow-AI data risk.</div>
  </div>
</div>
</div>

<div class="foot">
  <div class="takeaway">The meta-skill is <b>judgment</b>: knowing when the AI is wrong means knowing the domain better than the AI.</div>
  <div class="src">src: Stack Overflow AI 2025 · Santos 2025</div>
</div>
</div>

<!--
**Reading the four cards — your action list:**

- **1 · verify** — review AI code like you wrote it; the "almost right" bug is yours to catch.
- **2 · fundamentals** — don't skip the basics; depth is the only way you spot the Confidence Trap from slide 8.
- **3 · specify** — say intent precisely (configs, constraints, requirements) — the orchestration skill from slide 9.
- **4 · trust slowly** — "progressive trust": start on low-stakes tasks, and watch for shadow-AI risk (pasting private code/data into tools that may store it).

**The takeaway:** the meta-skill is **judgment** — knowing when the AI is wrong requires knowing the domain BETTER than the AI does. Fundamentals aren't nostalgia; they're the prerequisite for oversight. Keep this slide practical and energizing.

**Prompt:** "Name one fundamental you were tempted to let AI handle for you — and why that might be a trap."
-->

---
layout: center
class: text-center
title: "The throughline"
---

<div class="eyebrow"><span class="i">// 12</span> &nbsp; the throughline</div>

<h1 style="margin:1.2rem 0 1.6rem; font-size:3.2rem;">Redefinition,<br>not replacement.</h1>

<div style="display:flex; gap:2.5rem; justify-content:center; align-items:center; margin-bottom:1.8rem;">
  <div><span class="stat h-acc" style="font-size:1.9rem;">55% faster</span><div class="src" style="margin-top:.3rem;">new task, new dev</div></div>
  <div style="color:var(--faint); font-size:1.3rem;">vs</div>
  <div><span class="stat w-acc" style="font-size:1.9rem;">19% slower</span><div class="src" style="margin-top:.3rem;">mature repo, senior dev</div></div>
</div>

<div style="font-size:1.25rem; color:var(--muted); max-width:54ch; margin:0 auto;">
As code gets cheap, value moves to <b style="color:var(--ink)">intent · judgment · verification · accountability</b>. The field still needs you — a different version than five years ago.
</div>

<!--
**The two numbers (callback to the whole talk):** 55% faster vs 19% slower — same tool, opposite outcomes. 55% faster was a NEW task with a NEW developer (Peng, 2023); 19% slower was a MATURE repo with a SENIOR developer (METR, 2025). The productivity story is genuinely contested — that contradiction was the lesson.

**Land the throughline:** as code becomes cheap and abundant, the durable value of an engineer is what AI still can't do reliably — specifying intent, exercising judgment, verifying correctness, owning complex systems (Alenezi, 2026).

**Tone:** end on agency, not fear. The field still needs them — just a different version of the engineer than five years ago.
-->

---
layout: center
class: text-center
title: "Before you go"
---

<div class="eyebrow"><span class="i">//</span> &nbsp; before you go</div>

<div style="font-family:'Space Grotesk'; font-weight:600; font-size:2.4rem; line-height:1.25; margin-top:1.4rem; max-width:20ch; margin-left:auto; margin-right:auto;">
In one sentence — what will you do <span class="h-acc">differently</span> in how you learn to code?
</div>

<div class="src" style="margin-top:2.6rem;">thank you</div>

<!--
Closing audience prompt. Let a few volunteers answer aloud, or do a 10-second think-pair. Keep it warm and forward-looking — this is the note they leave on.
-->
