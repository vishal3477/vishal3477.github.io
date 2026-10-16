---
permalink: /
title: ""
excerpt: "Research Scientist at Adobe working on trustworthy AI, watermarking, and media provenance."
author_profile: true
selected_work:
  - name: FlowMark
    permalink: /publication/flowmark
    problem: "How can we add provenance signals to video, not just individual images?"
    contribution: "Explore mask-guided watermarking for video."
    significance: "Extends the study of content provenance to moving imagery."
    related:
      - name: Signpost
        permalink: /publication/signpost
        venue_label: ECCV LifegenIP Workshop
      - name: NRGMark
        permalink: /publication/nrgmark
        venue_label: WACV
  - name: TokenTrace
    permalink: /publication/tokentrace
    venue_label: CVPR
    problem: "A generated image can combine several concepts. Which ones influenced it?"
    contribution: "Recover watermarked tokens to attribute generated images to multiple concepts."
    significance: "Makes the mix of influences in generated content more traceable."
    related:
      - name: CustomMark
        permalink: /publication/custommark
        venue_label: ICCV APAI Workshop
      - name: ProMark
        permalink: /publication/paper6
        venue_label: CVPR
  - name: MaLP
    permalink: /publication/paper4
    venue_label: CVPR
    problem: "Knowing an image was manipulated is not enough. Where was it changed?"
    contribution: "Use a proactive template and local-global features to localize image manipulation."
    significance: "Moves beyond a real-or-fake label to identifying manipulated regions."
    related:
      - name: Proactive detection
        permalink: /publication/paper3
        venue_label: CVPR
      - name: "PrObeD: Proactive object detection"
        permalink: /publication/paper5
        venue_label: NeurIPS
  - name: Reverse engineering
    permalink: /publication/paper2
    venue_label: TPAMI
    problem: "What can generated images reveal about the model that created them?"
    contribution: "Infer generative-model architecture and loss-function attributes from generated images."
    significance: "Investigates the origins of synthetic media beyond detecting that it is generated."
    related:
      - name: Hyperparameter dependencies for model parsing
        permalink: /publication/model-parsing-graph
        venue_label: NeurIPS
      - name: Reverse engineering of deceptions survey
        permalink: /publication/paper7
        venue_label: Foundations and Trends in Privacy and Security
redirect_from:
  - /about/
  - /about.html
---

<div class="research-intro">
  <p class="research-intro__label">Vishal Asnani / Research Scientist</p>
  <h1 class="research-intro__headline">Building trust<br>in this <span>AI-generated era.</span></h1>
</div>

I'm a **Research Scientist at Adobe Research** in San Jose. I work on **video and audio watermarking**, image provenance, and generative AI attribution: methods that help answer where content came from, what influenced its creation, and whether it has been manipulated. My research connects content authenticity and responsible AI with practical safeguards for digital media, including durable Content Credentials for video.

I earned my **Ph.D. in Computer Science and Engineering at Michigan State University in December 2024**, advised by [Prof. Xiaoming Liu](https://www.cse.msu.edu/~liuxm/index2.html). Before joining Adobe full-time in January 2025, I interned at Adobe in 2023 and 2024, collaborating with [John Collomosse](https://research.adobe.com/person/john-collomosse/) and [Shruti Agarwal](https://agarwalshruti15.github.io/).

[Publications]({{ '/publications/' | relative_url }}) · [CV]({{ '/cv/' | relative_url }}) · [Talks & tutorials]({{ '/talks/' | relative_url }}) · [Get in touch](mailto:vishal.8.asnani@gmail.com)

## Recent news

<ol id="research-news" class="news-timeline" aria-label="Research news and milestones">
  <li>
    <time datetime="2026-10">Oct 2026</time>
    <p><a href="{{ '/publication/signpost' | relative_url }}">Signpost Watermarking</a>, our work on joint optimization for visual watermark coexistence, was <strong>accepted to the ECCV 2026 LifegenIP Workshop.</strong></p>
  </li>
  <li>
    <time datetime="2026-07">Jul 2026</time>
    <p><a href="{{ '/publication/flowmark' | relative_url }}">FlowMark</a>, our work on mask-guided video watermarking, is available as a preprint.</p>
  </li>
  <li>
    <time datetime="2026-06">Jun 2026</time>
    <div>
      <p>Co-organized <a href="https://vishal3477.github.io/watermarking-cvpr2026/">Foundations and Frontiers of Watermarking</a> at <strong>CVPR 2026</strong>, covering methods, multimodal extensions, robustness, and authenticity frameworks.</p>
      <p>Our <a href="{{ '/publication/deepfake-benchmark-audit' | relative_url }}">deepfake benchmark audit</a> is available as a preprint.</p>
      <p><a href="{{ '/publication/tokentrace' | relative_url }}">TokenTrace</a> and our <a href="{{ '/publication/edit-friendly-prompts' | relative_url }}">edit-friendly hard prompt inversion</a> work appeared at <strong>CVPR</strong>; <a href="{{ '/publication/pivot' | relative_url }}">PiVoT</a> appeared at <strong>CVPR Workshops</strong>.</p>
    </div>
  </li>
  <li>
    <time datetime="2026-04">Apr 2026</time>
    <p>Our <a href="{{ '/publication/paper8' | relative_url }}">survey of proactive schemes</a> appeared in the April issue of <strong>IJCV</strong>.</p>
  </li>
  <li>
    <time datetime="2026-03">Mar 2026</time>
    <p><a href="{{ '/publication/nrgmark' | relative_url }}">NRGMark</a> appeared at <strong>WACV 2026</strong>, exploring localized watermarking for energy transparency in images.</p>
  </li>
  <li>
    <time datetime="2025-10">Oct 2025</time>
    <p><a href="{{ '/publication/object-level-watermarking' | relative_url }}">Your Text Encoder Can Be An Object-Level Watermarking Controller</a> appeared at <strong>ICCV</strong>, and <a href="{{ '/publication/custommark' | relative_url }}">CustomMark</a> appeared at the <strong>ICCV APAI Workshop</strong>.</p>
  </li>
  <li>
    <time datetime="2025-01">Jan 2025</time>
    <p>Joined <strong>Adobe Research</strong> as a Research Scientist.</p>
  </li>
  <li>
    <time datetime="2024-12">Dec 2024</time>
    <div>
      <p>Completed my <strong>Ph.D. at Michigan State University</strong>.</p>
      <p>Our work on <a href="{{ '/publication/model-parsing-graph' | relative_url }}">hyperparameter dependencies for model parsing</a> appeared at <strong>NeurIPS 2024</strong>.</p>
    </div>
  </li>
  <li>
    <time datetime="2024-09">Sep 2024</time>
    <p>Shared the first version of our <a href="{{ '/publication/paper8' | relative_url }}">survey of proactive schemes</a>, bringing together applications of purposeful signals in computer vision. The survey is now published in <strong>IJCV</strong>.</p>
  </li>
  <li>
    <time datetime="2024-06">Jun 2024</time>
    <p><a href="{{ '/publication/paper6' | relative_url }}">ProMark</a> appeared at <strong>CVPR 2024</strong>, introducing proactive diffusion watermarking for causal attribution.</p>
  </li>
  <li>
    <time datetime="2024-05">May 2024</time>
    <p>Returned to <strong>Adobe Research</strong> as a Research Scientist Intern, continuing research on generative AI attribution.</p>
  </li>
  <li>
    <time datetime="2024-03">Mar 2024</time>
    <p>Shared the news that <a href="{{ '/publication/paper6' | relative_url }}">ProMark</a> was <strong>accepted to CVPR 2024</strong>, following research during my 2023 Adobe internship.</p>
  </li>
  <li>
    <time datetime="2024-01">Jan 2024</time>
    <p>Our <a href="{{ '/publication/paper7' | relative_url }}">Reverse Engineering of Deceptions survey</a> was published in <strong>Foundations and Trends in Privacy and Security</strong>.</p>
  </li>
  <li>
    <time datetime="2023-12">Dec 2023</time>
    <p>Our <a href="{{ '/publication/paper2' | relative_url }}">reverse engineering of generative models</a> paper appeared in the December issue of <strong>TPAMI</strong>, exploring how generated images reveal model hyperparameters.</p>
  </li>
  <li>
    <time datetime="2023-09">Sep 2023</time>
    <p><a href="{{ '/publication/paper5' | relative_url }}">PrObeD</a>, our proactive wrapper for object detection, was <strong>accepted to NeurIPS 2023</strong>.</p>
  </li>
  <li>
    <time datetime="2023-07">Jul 2023</time>
    <p>Our work on <a href="{{ '/publication/paper2' | relative_url }}">reverse engineering generative models and inferring their hyperparameters</a> was <strong>accepted to TPAMI</strong>.</p>
  </li>
  <li>
    <time datetime="2023-06">Jun 2023</time>
    <div>
      <p><a href="{{ '/publication/paper4' | relative_url }}">MaLP</a>, our proactive approach to manipulation localization, appeared at <strong>CVPR 2023</strong>.</p>
      <p>Co-organized the <a href="{{ '/talks/reverse-engineering-deceptions-cvpr2023' | relative_url }}">Reverse Engineering of Deceptions tutorial</a> at <strong>CVPR 2023</strong>.</p>
    </div>
  </li>
  <li>
    <time datetime="2023-05">May 2023</time>
    <p>Joined <strong>Adobe Research</strong> as a Research Scientist Intern, collaborating with John Collomosse and Shruti Agarwal on proactive attribution for generative AI.</p>
  </li>
  <li>
    <time datetime="2023-03">Mar 2023</time>
    <p>Shared the news that <a href="{{ '/publication/paper4' | relative_url }}">MaLP: Manipulation Localization Using a Proactive Scheme</a> was <strong>accepted to CVPR 2023</strong>.</p>
  </li>
  <li>
    <time datetime="2023-01">Jan 2023</time>
    <p>Gave an <a href="{{ '/talks/talk_2' | relative_url }}">in-person talk at Scale AI</a> on reverse engineering generative models.</p>
  </li>
  <li>
    <time datetime="2022-08">Aug 2022</time>
    <p>Gave a <a href="{{ '/talks/2012-03-01-talk-1' | relative_url }}">virtual talk at Scale AI</a> on proactive image manipulation detection.</p>
  </li>
  <li>
    <time datetime="2022-06">Jun 2022</time>
    <p><a href="{{ '/publication/paper3' | relative_url }}">Proactive Image Manipulation Detection</a> appeared at <strong>CVPR 2022</strong>, exploring learnable templates for detecting manipulated images.</p>
  </li>
  <li>
    <time datetime="2022-03">Mar 2022</time>
    <p><a href="{{ '/publication/paper3' | relative_url }}">Proactive Image Manipulation Detection</a> was <strong>accepted to CVPR 2022</strong>.</p>
  </li>
</ol>

<div class="news-controls">
  <button id="news-show-more" class="btn btn--inverse news-more" type="button" aria-controls="research-news" hidden>Show more</button>
  <span id="news-status" role="status" aria-live="polite"></span>
</div>

## Research areas

<div class="research-cards">
  <article class="research-card" aria-labelledby="watermarking-title">
    <p class="research-card__label">Content authenticity</p>
    <h3 id="watermarking-title">Signals that help media tell its story.</h3>
    <img class="research-card__visual" src="{{ '/images/research-watermarking.svg' | relative_url }}" alt="Watermarking overview: digital media, an embedded signal, and provenance verification." width="720" height="240" loading="lazy">
    <p><strong>Video and audio watermarking</strong>, localized image metadata, and visual watermark coexistence for traceable media.</p>
    <ul class="research-card__links" aria-label="Watermarking papers">
      <li><a href="{{ '/publication/flowmark' | relative_url }}">FlowMark <span>Preprint</span></a></li>
      <li><a href="{{ '/publication/nrgmark' | relative_url }}">NRGMark <span>WACV 2026</span></a></li>
      <li><a href="{{ '/publication/signpost' | relative_url }}">Signpost <span>ECCV 2026 LifegenIP Workshop · Accepted</span></a></li>
    </ul>
  </article>
  <article class="research-card" aria-labelledby="attribution-title">
    <p class="research-card__label">Generative AI attribution</p>
    <h3 id="attribution-title">Tracing the ideas behind the image.</h3>
    <img class="research-card__visual" src="{{ '/images/research-attribution.svg' | relative_url }}" alt="Attribution overview: source concepts influence generated content, followed by tracing those influences." width="720" height="240" loading="lazy">
    <p>Tracing creative influences through watermarked training data, diffusion-model customization, and token recovery.</p>
    <ul class="research-card__links" aria-label="Attribution papers">
      <li><a href="{{ '/publication/paper6' | relative_url }}">ProMark <span>CVPR 2024</span></a></li>
      <li><a href="{{ '/publication/custommark' | relative_url }}">CustomMark <span>ICCV 2025 APAI Workshop</span></a></li>
      <li><a href="{{ '/publication/tokentrace' | relative_url }}">TokenTrace <span>CVPR 2026</span></a></li>
    </ul>
  </article>
  <article class="research-card" aria-labelledby="forensics-title">
    <p class="research-card__label">Media forensics &amp; evaluation</p>
    <h3 id="forensics-title">Looking beyond what meets the eye.</h3>
    <img class="research-card__visual" src="{{ '/images/research-forensics.svg' | relative_url }}" alt="Forensics overview: media inputs, forensic analysis, and evaluation." width="720" height="240" loading="lazy">
    <p>Localizing manipulation, inferring model properties, and testing what deepfake benchmarks really measure.</p>
    <ul class="research-card__links" aria-label="Media forensics papers">
      <li><a href="{{ '/publication/paper3' | relative_url }}">Proactive detection <span>CVPR 2022</span></a></li>
      <li><a href="{{ '/publication/paper4' | relative_url }}">MaLP <span>CVPR 2023</span></a></li>
      <li><a href="{{ '/publication/paper2' | relative_url }}">Model parsing <span>TPAMI 2023</span></a></li>
      <li><a href="{{ '/publication/deepfake-benchmark-audit' | relative_url }}">Benchmark audit <span>Preprint</span></a></li>
    </ul>
  </article>
</div>

<p class="research-visual-note">Illustrative research-area overviews, not experimental results.</p>

<span id="selected-work"></span>

## Selected publications

Four perspectives on trustworthy media: watermarking video, tracing creative influences, localizing manipulation, and reverse engineering generative models.

<div class="selected-work" aria-label="Selected research papers">
  {% for work in page.selected_work %}
    {% assign publication = site.publications | where: 'permalink', work.permalink | first %}
    <article class="selected-work__card" aria-labelledby="selected-{{ work.name | slugify }}">
      <p class="selected-work__meta">{% if publication.status == 'preprint' %}Preprint{% else %}{{ work.venue_label }}{% endif %} · {{ publication.date | date: "%b %Y" }}</p>
      <h3 id="selected-{{ work.name | slugify }}"><a href="{{ publication.url | relative_url }}">{{ work.name }}</a></h3>
      <p class="selected-work__title">{{ publication.title }}</p>
      <dl class="selected-work__facts">
        <dt>The problem</dt>
        <dd>{{ work.problem }}</dd>
        <dt>Our approach</dt>
        <dd>{{ work.contribution }}</dd>
        <dt>Why it matters</dt>
        <dd>{{ work.significance }}</dd>
      </dl>
      <div class="selected-work__footer">
        <div class="selected-work__links">
          <a href="{{ publication.url | relative_url }}" aria-label="Explore {{ work.name }}">Explore work</a>
          {% if publication.paperurl contains '://' %}{% assign paper_url = publication.paperurl %}{% else %}{% assign paper_url = publication.paperurl | relative_url %}{% endif %}
          <a href="{{ paper_url }}" aria-label="Read the {{ work.name }} paper">{% if publication.status == 'preprint' %}Read preprint{% else %}Read paper{% endif %}</a>
        </div>
        <div class="selected-work__related">
          <h4>Related work</h4>
          <ul aria-label="Related work for {{ work.name }}">
            {% for related in work.related %}
              {% assign related_publication = site.publications | where: 'permalink', related.permalink | first %}
              <li>
                <a href="{{ related_publication.url | relative_url }}">{{ related.name }}</a>
                <span>{% if related_publication.status == 'preprint' %}Preprint{% else %}{% if related_publication.status == 'accepted' %}Accepted · {% endif %}{{ related.venue_label }}{% endif %} · {{ related_publication.date | date: "%Y" }}</span>
              </li>
            {% endfor %}
          </ul>
        </div>
      </div>
    </article>
  {% endfor %}
</div>

[Browse all publications]({{ '/publications/' | relative_url }})

## Community and collaboration

I mentor research interns, co-organize tutorials, and review for venues including CVPR, ICCV, ECCV, TPAMI, IJCV, ICLR, AAAI, ACM Multimedia, and WACV. I also co-organized the CVPR 2023 tutorial *Reverse Engineering of Deceptions* and presented my research at Scale AI.

I welcome collaborations on watermarking, content authenticity, responsible AI, media provenance, and deepfake detection. Reach me at [vishal.8.asnani@gmail.com](mailto:vishal.8.asnani@gmail.com).

My collaborators have included Xiaoming Liu, Tal Hassner, John Collomosse, Shruti Agarwal, Xi Yin, and Sijia Liu.

## Selected media coverage

Our research on reverse engineering generative models was covered by [CNBC](https://www.cnbc.com/2021/06/16/facebook-scientists-say-they-can-tell-where-deepfakes-come-from.html), [The Verge](https://www.theverge.com/2021/6/16/22534690/facebook-deepfake-detection-reverse-engineer-ai-model-hyperparameters), [VentureBeat](https://venturebeat.com/business/facebooks-ai-reverse-engineers-models-used-to-generate-deepfakes/), [The Wall Street Journal](https://www.wsj.com/articles/facebook-michigan-state-develop-deepfake-detection-technique-11623859200), and [MSU Today](https://msutoday.msu.edu/news/2021/deepfake-detection).

## Outside research

I enjoy long drives, jigsaw puzzles, reading, football, badminton, and table tennis.
