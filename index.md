---
layout: null
title: WEI ZIQIN · Data Science Portfolio
---
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="{{ site.description | escape }}">
  <title>{{ page.title | escape }}</title>
  <style>
    :root{--paper:#f8faf8;--ink:#17383b;--muted:#4d6566;--line:#d4dfda;--accent:#176e60;--soft:#e8f0eb}
    *{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;background:var(--paper);color:var(--ink);font-family:system-ui,-apple-system,"Segoe UI",sans-serif;font-size:17px;line-height:1.75}
    a{color:var(--accent);text-underline-offset:4px}a:hover{text-decoration-thickness:2px}a:focus-visible{outline:3px solid var(--accent);outline-offset:5px}
    .wrap{width:min(1120px,calc(100% - 80px));margin:auto}.top{display:flex;justify-content:space-between;align-items:center;gap:24px;padding:26px 0;border-bottom:1px solid var(--line)}
    .wordmark{font-size:14px;font-weight:650;letter-spacing:.09em;text-decoration:none;color:var(--ink)}nav{display:flex;gap:26px;flex-wrap:wrap}nav a{font-size:14px;text-decoration:none;color:var(--muted)}
    h1,h2,h3{font-family:Georgia,"Times New Roman",serif;font-weight:400;line-height:1.08;letter-spacing:-.035em;margin:0}h1{font-size:clamp(45px,6.9vw,82px);max-width:1000px}h2{font-size:clamp(36px,4.8vw,57px)}h3{font-size:clamp(28px,3.4vw,40px)}p{max-width:790px;margin:18px 0 0}
    .intro{padding:80px 0 76px}.eyebrow{font-size:12px;text-transform:uppercase;letter-spacing:.13em;font-weight:650;color:var(--muted);margin:0 0 22px}.lead{font-size:21px;line-height:1.65;max-width:790px;margin-top:30px}.skills{display:flex;gap:10px;flex-wrap:wrap;margin:28px 0}.skills span{font-size:13px;padding:3px 0;margin-right:15px;color:var(--muted)}.text-link{display:inline-block;margin-top:6px;text-decoration:none;font-weight:600}
    .project-intro,.result,.method,.limits,.sources{border-top:1px solid var(--line);padding:52px 0}.project-heading{display:flex;justify-content:space-between;align-items:flex-start;gap:35px}.project-status{font-size:14px;text-align:right;color:var(--muted);margin-top:8px}.question{font-size:21px;line-height:1.6;margin-top:30px}.question strong{font-size:13px;text-transform:uppercase;letter-spacing:.08em;color:var(--accent)}
    .section-heading{max-width:900px}.result p{margin-bottom:28px}figure{margin:0}figure img{display:block;width:100%;height:auto;background:white}figcaption{font-size:13px;color:var(--muted);max-width:850px;margin-top:15px}
    .method{display:grid;grid-template-columns:1fr 1.3fr;gap:65px}.method p:first-child{margin-top:0}.method .eyebrow{margin-bottom:22px}.repo-link{display:inline-block;margin-top:24px;font-weight:600}.limits{padding:48px 32px;background:var(--soft);border-top:0;margin-bottom:28px}.limits p{max-width:880px}.sources{padding:35px 0 48px}.sources h3{font-size:27px}.sources p{font-size:14px;max-width:930px}.assistance{color:var(--muted)}footer{padding:24px 0 36px;border-top:1px solid var(--line);font-size:12px;color:var(--muted)}
    @media(max-width:700px){.wrap{width:calc(100% - 36px)}body{font-size:16px}.top{align-items:flex-start;gap:18px}.top nav{gap:12px}.intro{padding:50px 0}.lead,.question{font-size:19px}.project-heading{display:block}.project-status{text-align:left;margin-top:18px}.method{grid-template-columns:1fr;gap:26px}.limits{padding:28px 20px}.project-intro,.result,.method{padding:38px 0}figure{margin-left:-4px;margin-right:-4px}nav a{font-size:13px}}
    @media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}}
  </style>
</head>
<body><div class="wrap">
  <header class="top"><a class="wordmark" href="{{ '/' | relative_url }}">WEI ZIQIN</a><nav aria-label="Main navigation"><a href="#project">Project</a><a href="#method">Method</a><a href="#limitations">Limitations</a></nav></header>
  <main><section class="intro" id="about">
  <p class="eyebrow">WEI ZIQIN · Data science coursework</p>
  <h1>From observations<br>to a clear explanation.</h1>
  <p class="lead">I am developing my skills in data exploration, reproducible Python workflows, and visual communication through CISC7204. This portfolio shows how I turn a question into documented analysis, with the limitations kept in view.</p>
  <div class="skills" aria-label="Practised technical skills"><span>Python</span><span>pandas &amp; NumPy</span><span>Matplotlib</span><span>GitHub</span><span>Reproducible analysis</span></div>
  <a class="text-link" href="#project">Explore the project <span aria-hidden="true">↓</span></a>
</section>

<section class="project-intro" id="project">
  <p class="eyebrow">01 / Featured project</p>
  <div class="project-heading"><h2>Penguin size<br>across species.</h2><p class="project-status">Analysis: completed<br>Portfolio review: in progress</p></div>
  <p class="question"><strong>Research question</strong><br>How does body mass differ across three penguin species, and does the flipper-length relationship look the same within each species?</p>
  <p>The public Palmer Penguins dataset contains 344 observations from three Antarctic islands in 2007–2009. Both analyses below use 342 observed measurement pairs; the two rows with missing required measurements are excluded, not filled with invented values.</p>
</section>

<section class="result">
  <div class="section-heading"><p class="eyebrow">Finding 01 / Compare distributions</p><h3>A higher median does not mean no overlap.</h3></div>
  <p>Gentoo penguins have a median body mass of <strong>5,000 g</strong> in this sample. Adelie and Chinstrap both have medians of <strong>3,700 g</strong>. Individual points show the variation that would be hidden by three averages alone.</p>
  <figure><img src="{{ '/body_mass_by_species.png' | relative_url }}" alt="Body-mass boxplots and individual observations. Sample sizes are 151 Adelie, 68 Chinstrap and 123 Gentoo. The Gentoo median is 5,000 grams, compared with 3,700 grams for the other two species."><figcaption>Figure 1. Each point is one observed penguin. Boxes show the middle 50% of recorded body masses; counts and medians are labelled.</figcaption></figure>
</section>

<section class="result">
  <div class="section-heading"><p class="eyebrow">Finding 02 / Check subgroups</p><h3>The overall relationship is stronger than each subgroup's.</h3></div>
  <p>Across all 342 complete measurement pairs, Pearson's correlation is <strong>0.87</strong>. Examined separately, it is <strong>0.47 for Adelie</strong>, <strong>0.64 for Chinstrap</strong> and <strong>0.70 for Gentoo</strong>. The positive association remains, but pooling species also mixes differences between groups.</p>
  <figure><img src="{{ '/flipper_mass_by_species.png' | relative_url }}" alt="Flipper length versus body mass in three species-specific scatterplots on shared axes, showing positive within-species correlations of 0.47, 0.64 and 0.70."><figcaption>Figure 2. Matching axes allow direct comparisons. Colours and marker shapes identify species without relying on colour alone.</figcaption></figure>
</section>

<section class="method" id="method">
  <div><p class="eyebrow">How the results were produced</p><h2>Small project.<br>Traceable decisions.</h2></div>
  <div><p>I used pandas and NumPy to inspect missing values and compute group summaries and correlations. Matplotlib generates both figures from the same unchanged CSV. The script has no network or API-key dependency after download.</p><p>The project repository contains the Python program, pinned requirements, raw data, two visualizations, numerical outputs and a README with reproduction instructions. Automated checks confirm that the source observations remain unchanged and that selected statistics match the results shown here.</p><a class="repo-link" href="https://github.com/crudeboywei-cyber/data-science-project">View code, data and running instructions <span aria-hidden="true">↗</span></a></div>
</section>

<section class="limits" id="limitations">
  <p class="eyebrow">What this project does not establish</p>
  <h2>A local sample, not a universal rule.</h2>
  <p>These are observations from three islands during 2007–2009, not a random sample of all penguins. Species and island are not independently balanced, and sex and other biological factors may help explain the remaining variation. The relationships are descriptive, not causal.</p>
  <p><strong>Next improvement:</strong> examine sex-specific subgroups with their sample sizes and uncertainty, then evaluate whether a prediction model is warranted. I will also refine the presentation based on a classmate's feedback.</p>
</section>

<section class="sources" id="sources">
  <h3>Source and responsible use</h3>
  <p>Data: Horst, A. M., Hill, A. P., &amp; Gorman, K. B. (2020). <em>palmerpenguins: Palmer Archipelago (Antarctica) penguin data</em>. <a href="https://doi.org/10.5281/zenodo.3960218">doi:10.5281/zenodo.3960218</a>. The documented data were collected by Dr. Kristen Gorman and the Palmer Station Long Term Ecological Research Program.</p>
  <p><a href="https://allisonhorst.github.io/palmerpenguins/articles/intro.html">Dataset documentation and CC0 permission</a> · <a href="https://github.com/allisonhorst/palmerpenguins/blob/main/inst/extdata/penguins.csv">Original CSV</a></p>
  <p class="assistance">AI assistance was used for code preparation, debugging, documentation and page design. All numerical results were computed from the cited data. No credentials, private contact details, or restricted course datasets are published.</p>
</section></main>
  <footer>WEI ZIQIN · CISC7204 Practice 09 · A reproducible data science learning project.</footer>
</div></body>
</html>
