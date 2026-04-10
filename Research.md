---
layout: page
title: Research
permalink: /research/
---

<style>
  .research-shell {
    --ink: #13364a;
    --muted: #526779;
    --line: #d9e5ef;
    --card: #ffffff;
    --mist: #f4f8fb;
    --accent: #0e7082;
    --accent-soft: #dff1f4;
    --warm: #c97a2b;
    max-width: 1240px;
    margin: 0 auto;
    color: var(--ink);
    font-family: Georgia, "Times New Roman", serif;
  }

  .research-hero {
    position: relative;
    overflow: hidden;
    border-radius: 28px;
    padding: 72px 42px 44px;
    margin-bottom: 44px;
    color: #ffffff;
    background:
      linear-gradient(135deg, rgba(9, 36, 53, 0.9), rgba(13, 83, 96, 0.72)),
      url("{{ '/research/background.png' | relative_url }}") center/cover no-repeat;
    box-shadow: 0 22px 48px rgba(7, 30, 44, 0.2);
  }

  .research-hero::after {
    content: "";
    position: absolute;
    inset: auto -8% -32% auto;
    width: 340px;
    height: 340px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.22), rgba(255, 255, 255, 0));
    pointer-events: none;
  }

  .research-kicker {
    display: inline-block;
    margin-bottom: 16px;
    padding: 6px 12px;
    border-radius: 999px;
    letter-spacing: 0.08em;
    font-size: 0.78rem;
    text-transform: uppercase;
    background: rgba(255, 255, 255, 0.14);
    border: 1px solid rgba(255, 255, 255, 0.18);
  }

  .research-hero h2 {
    margin: 0 0 18px;
    font-size: clamp(2.4rem, 5vw, 4.1rem);
    line-height: 1.03;
    letter-spacing: -0.03em;
    font-weight: 700;
  }

  .research-hero p {
    max-width: 960px;
    margin: 0;
    font-size: 1.14rem;
    line-height: 1.9;
    color: rgba(255, 255, 255, 0.92);
  }

  .research-pillars {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 18px;
    margin-top: 32px;
  }

  .research-pillar {
    padding: 22px 20px;
    border-radius: 20px;
    background: rgba(255, 255, 255, 0.14);
    border: 1px solid rgba(255, 255, 255, 0.16);
    backdrop-filter: blur(10px);
  }

  .research-pillar h3 {
    margin: 0 0 8px;
    font-size: 1.2rem;
    font-family: "Segoe UI", Arial, sans-serif;
    font-weight: 700;
    color: #ffffff;
  }

  .research-pillar p {
    margin: 0;
    font-size: 0.98rem;
    line-height: 1.7;
    color: rgba(255, 255, 255, 0.9);
  }

  .research-stack {
    display: grid;
    gap: 28px;
  }

  .research-card {
    display: grid;
    grid-template-columns: minmax(0, 1.05fr) minmax(0, 1fr);
    gap: 28px;
    align-items: stretch;
    padding: 28px;
    border-radius: 26px;
    background: linear-gradient(180deg, var(--card), #fbfdff);
    border: 1px solid var(--line);
    box-shadow: 0 14px 34px rgba(19, 54, 74, 0.08);
  }

  .research-card.reverse {
    grid-template-columns: minmax(0, 1fr) minmax(0, 1.05fr);
  }

  .research-copy {
    display: flex;
    flex-direction: column;
    justify-content: center;
    min-width: 0;
  }

  .research-index {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 14px;
    font-size: 0.84rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--accent);
    font-family: "Segoe UI", Arial, sans-serif;
    font-weight: 700;
  }

  .research-index::before {
    content: "";
    width: 34px;
    height: 1px;
    background: rgba(14, 112, 130, 0.45);
  }

  .research-copy h3 {
    margin: 0 0 16px;
    font-size: clamp(1.7rem, 2.4vw, 2.4rem);
    line-height: 1.16;
    letter-spacing: -0.025em;
    color: var(--ink);
  }

  .research-copy p {
    margin: 0;
    color: var(--muted);
    font-size: 1.04rem;
    line-height: 1.9;
    text-align: left;
  }

  .research-media-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 16px;
    min-width: 0;
  }

  .research-media-card {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  .research-media-card.feature {
    grid-column: span 2;
  }

  .research-media-frame {
    position: relative;
    overflow: hidden;
    border-radius: 18px;
    aspect-ratio: 4 / 3;
    background: linear-gradient(180deg, #edf4f8, #dfeaf1);
    border: 1px solid #d7e4ee;
    box-shadow: 0 10px 24px rgba(19, 54, 74, 0.08);
  }

  .research-media-card.feature .research-media-frame {
    aspect-ratio: 16 / 9;
  }

  .research-media-frame img,
  .research-media-frame video {
    width: 100%;
    height: 100%;
    display: block;
    object-fit: cover;
  }

  .research-media-card.contain .research-media-frame img,
  .research-media-card.contain .research-media-frame video {
    object-fit: contain;
    padding: 12px;
    background: #f7fbfd;
  }

  .research-media-card.square .research-media-frame {
    aspect-ratio: 1 / 1;
  }

  .research-caption {
    margin: 0;
    padding: 0 4px;
    color: var(--muted);
    font-size: 0.95rem;
    line-height: 1.55;
    font-family: "Segoe UI", Arial, sans-serif;
  }

  .research-divider {
    margin: 36px 0 6px;
    height: 2px;
    border: 0;
    background-image: linear-gradient(to right, rgba(201, 122, 43, 0), rgba(201, 122, 43, 0.75), rgba(201, 122, 43, 0));
  }

  @media (max-width: 980px) {
    .research-hero {
      padding: 54px 24px 30px;
    }

    .research-pillars,
    .research-card,
    .research-card.reverse {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 720px) {
    .research-media-grid,
    .research-media-card.feature {
      grid-template-columns: 1fr;
      grid-column: span 1;
    }

    .research-card {
      padding: 22px;
    }

    .research-copy p,
    .research-hero p {
      font-size: 1rem;
    }
  }
</style>

<div class="research-shell">
  <section class="research-hero">
    <span class="research-kicker">Research Themes</span>
    <h2>Computational principles of natural intelligence, from behavior to brain dynamics</h2>
    <p>
      Gaining insight into the navigational algorithms of organisms and their neural network-level regulatory
      mechanisms not only deepens our understanding of biological navigational decision-making but also offers new
      perspectives for building more adaptive artificial intelligence. Our lab uses animal navigation and active
      learning as model systems to study how brains integrate sensation, memory, decision-making, and learning in
      complex environments.
    </p>
    <div class="research-pillars">
      <div class="research-pillar">
        <h3>Modeling</h3>
        <p>Quantitative experiments and machine learning models that describe and simulate biological algorithms.</p>
      </div>
      <div class="research-pillar">
        <h3>Dynamics</h3>
        <p>Whole-brain recordings and circuit-level analysis of how neural population activity supports behavior.</p>
      </div>
      <div class="research-pillar">
        <h3>Comparison</h3>
        <p>Comparative work across species and AI systems to expose the core principles of efficient intelligence.</p>
      </div>
    </div>
  </section>

  <div class="research-stack">
    <section class="research-card">
      <div class="research-copy">
        <div class="research-index">Theme 01</div>
        <h3>Quantitative experiments and ML/statistical modeling of animal navigation</h3>
        <p>
          We use <em>Caenorhabditis elegans</em> as a model system to decipher the neural computational mechanisms
          underlying navigation in complex environments. Capitalizing on its fully mapped connectome, we study how the
          worm optimizes survival through integrated processes of sensation, learning, and decision-making. Our work
          spans adaptive foraging, probabilistic associative learning in noisy settings, and olfaction-based food
          object recognition. To support these questions, we established a freely moving whole-brain imaging platform
          that enables cellular-resolution analysis of neural activity during behavior, providing direct insight into
          the circuit-level mechanisms of adaptive control.
        </p>
      </div>
      <div class="research-media-grid">
        <figure class="research-media-card feature contain">
          <div class="research-media-frame">
            <img src="{{ '/research/WBI-platform.png' | relative_url }}" alt="Whole-brain imaging platform" />
          </div>
          <figcaption class="research-caption">Whole-brain imaging platform for freely moving animals.</figcaption>
        </figure>
        <figure class="research-media-card square contain">
          <div class="research-media-frame">
            <img src="{{ '/research/C.elegans.png' | relative_url }}" alt="C. elegans model system" />
          </div>
          <figcaption class="research-caption">C. elegans as a compact model for navigation and learning.</figcaption>
        </figure>
        <figure class="research-media-card">
          <div class="research-media-frame">
            <img src="{{ '/research/WBI.gif' | relative_url }}" alt="Behavior and brain activity recording" />
          </div>
          <figcaption class="research-caption">Behavioral dynamics paired with neural activity measurements.</figcaption>
        </figure>
      </div>
    </section>

    <section class="research-card reverse">
      <div class="research-media-grid">
        <figure class="research-media-card feature">
          <div class="research-media-frame">
            <img src="{{ '/research/motor.jpg' | relative_url }}" alt="Motor interception in daily life" />
          </div>
          <figcaption class="research-caption">Everyday interception tasks motivate our sensorimotor modeling questions.</figcaption>
        </figure>
        <figure class="research-media-card">
          <div class="research-media-frame">
            <img src="{{ '/research/interception new paradigm .gif' | relative_url }}" alt="Interception behavior paradigm" />
          </div>
          <figcaption class="research-caption">A controlled behavioral paradigm for predictive motor interception.</figcaption>
        </figure>
        <figure class="research-media-card">
          <div class="research-media-frame">
            <img src="{{ '/research/interception paradigm.gif' | relative_url }}" alt="Task dynamics in interception experiments" />
          </div>
          <figcaption class="research-caption">Task dynamics used to probe anticipation and timing in neural systems.</figcaption>
        </figure>
      </div>
      <div class="research-copy">
        <div class="research-index">Theme 02</div>
        <h3>RNN analysis of motor control and predictive interception</h3>
        <p>
          Predictive motor control is a core feature of everyday behavior. We use recurrent neural networks to model
          the neural mechanisms that transform rapidly changing sensory signals into well-timed actions, using examples
          such as racket-ball interception. Our models are trained on large-scale neural population recordings from the
          common marmoset and then analyzed to identify predictive activity, dynamical primitives, and other neural
          signatures of anticipation. This work aims to uncover the computational principles that allow the brain to
          perform fast and accurate motor interception in a dynamic world.
        </p>
      </div>
    </section>

    <section class="research-card">
      <div class="research-copy">
        <div class="research-index">Theme 03</div>
        <h3>Human exploration and function learning in high-dimensional environments</h3>
        <p>
          Humans and animals must actively sample rich environments and efficiently discover the low-dimensional
          structure that matters for reward and decision-making. We study human exploratory behavior in contextual
          bandit tasks where the context resides in a genuinely high-dimensional space. Unlike classic low-dimensional
          settings, these tasks require active exploration, hypothesis formation, and dimensionality reduction rather
          than relying on explicitly instructed relevant features. Our goal is to reveal the learning strategies that
          make humans remarkably efficient in complex environments and to understand how those strategies differ from
          current AI systems.
        </p>
      </div>
      <div class="research-media-grid">
        <figure class="research-media-card square contain">
          <div class="research-media-frame">
            <img src="{{ '/research/Topic 3 .png' | relative_url }}" alt="Illustration of high-dimensional restaurant choice" />
          </div>
          <figcaption class="research-caption">An intuitive example of high-dimensional context-guided choice.</figcaption>
        </figure>
        <figure class="research-media-card feature contain">
          <div class="research-media-frame">
            <img src="{{ '/research/Topic 3-2.png' | relative_url }}" alt="Possible human behavior patterns in high dimensions" />
          </div>
          <figcaption class="research-caption">Possible exploration patterns as humans search for useful structure.</figcaption>
        </figure>
      </div>
    </section>
  </div>

  <hr class="research-divider" />
</div>
