---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 5
description:
---

<style>
/* =========================
   CV PAGE
   ========================= */

article.post > header.post-header {
  display: none;
}

.cv-page {
  max-width: 1000px;
  margin: 0 auto;
  padding-bottom: 3rem;
  color: var(--global-text-color);
}

/* Header */

.cv-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 2rem;
  padding-bottom: 1.6rem;
  margin-bottom: 2.3rem;
  border-bottom: 1px solid var(--global-divider-color);
}

.cv-name {
  font-size: 2.45rem;
  font-weight: 500;
  line-height: 1.1;
  margin: 0 0 0.55rem 0;
  letter-spacing: -0.035em;
}

.cv-subtitle {
  font-size: 1.12rem;
  line-height: 1.5;
  margin-bottom: 0.35rem;
}

.cv-affiliation {
  font-size: 1rem;
  opacity: 0.78;
  margin-bottom: 0.65rem;
}

.cv-contact {
  display: flex;
  flex-wrap: wrap;
  gap: 0.3rem 1rem;
  font-size: 0.94rem;
}

.cv-contact a {
  color: var(--global-theme-color);
  text-decoration: none;
}

.cv-contact a:hover {
  text-decoration: underline;
}

.cv-pdf-btn {
  display: inline-block;
  white-space: nowrap;
  border: 1px solid var(--global-theme-color);
  color: var(--global-theme-color) !important;
  padding: 0.48rem 0.85rem;
  border-radius: 5px;
  font-size: 0.9rem;
  text-decoration: none !important;
  transition: all 0.15s ease;
}

.cv-pdf-btn:hover {
  background: var(--global-theme-color);
  color: white !important;
}


/* Quick navigation */

.cv-nav {
  display: flex;
  flex-wrap: wrap;
  gap: 0.35rem 1.1rem;
  margin: -0.5rem 0 2.7rem 0;
  font-size: 0.9rem;
}

.cv-nav a {
  color: var(--global-text-color);
  opacity: 0.7;
  text-decoration: none;
}

.cv-nav a:hover {
  color: var(--global-theme-color);
  opacity: 1;
}


/* Sections */

.cv-section {
  margin-bottom: 3rem;
  scroll-margin-top: 90px;
}

.cv-section-title {
  font-size: 1.42rem;
  font-weight: 500;
  color: var(--global-theme-color);
  margin: 0 0 1.35rem 0;
  padding-bottom: 0.4rem;
  border-bottom: 1px solid var(--global-divider-color);
  letter-spacing: -0.015em;
}

.cv-subsection-title {
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-weight: 600;
  opacity: 0.62;
  margin: 1.7rem 0 1rem 0;
}


/* Standard entries */

.cv-entry {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 150px;
  gap: 1.5rem;
  margin-bottom: 1.5rem;
}

.cv-entry:last-child {
  margin-bottom: 0;
}

.cv-entry-title {
  font-size: 1.02rem;
  font-weight: 600;
  line-height: 1.45;
  margin-bottom: 0.12rem;
}

.cv-entry-subtitle {
  font-size: 0.96rem;
  line-height: 1.45;
  margin-bottom: 0.15rem;
}

.cv-entry-meta {
  font-size: 0.91rem;
  opacity: 0.68;
}

.cv-entry-date {
  text-align: right;
  font-size: 0.91rem;
  opacity: 0.72;
  white-space: nowrap;
  padding-top: 0.1rem;
}


/* Research */

.cv-research {
  margin-bottom: 2rem;
}

.cv-research-title {
  font-size: 1.04rem;
  line-height: 1.45;
  font-weight: 600;
  margin-bottom: 0.3rem;
}

.cv-supervisor {
  font-size: 0.92rem;
  opacity: 0.7;
  margin-bottom: 0.45rem;
}

.cv-research ul {
  margin: 0.4rem 0 0.3rem 1.1rem;
  padding-left: 0.5rem;
}

.cv-research li {
  margin-bottom: 0.25rem;
  line-height: 1.55;
}


/* Publications */

.pub-list {
  counter-reset: publication;
}

.pub-item {
  display: grid;
  grid-template-columns: 34px minmax(0, 1fr);
  gap: 0.65rem;
  margin-bottom: 1.25rem;
}

.pub-number {
  color: var(--global-theme-color);
  font-size: 0.88rem;
  font-weight: 600;
  padding-top: 0.12rem;
}

.pub-title {
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.42;
  margin-bottom: 0.15rem;
}

.pub-authors {
  font-size: 0.92rem;
  line-height: 1.48;
  opacity: 0.88;
}

.pub-authors strong {
  font-weight: 650;
  color: var(--global-text-color);
}

.pub-journal {
  font-size: 0.93rem;
  margin-top: 0.12rem;
}

.pub-journal em {
  font-weight: 500;
}

.coauthor-note {
  font-size: 0.84rem;
  opacity: 0.6;
  margin-top: -0.6rem;
  margin-bottom: 1.25rem;
}


/* Presentation */

.presentation-type {
  display: inline-block;
  font-size: 0.76rem;
  font-weight: 600;
  color: var(--global-theme-color);
  border: 1px solid var(--global-theme-color);
  border-radius: 4px;
  padding: 0.08rem 0.4rem;
  margin-right: 0.35rem;
}


/* Skills */

.skill-row {
  display: grid;
  grid-template-columns: 215px minmax(0, 1fr);
  gap: 1.2rem;
  margin-bottom: 0.85rem;
  line-height: 1.5;
}

.skill-name {
  font-weight: 600;
}

.skill-content {
  opacity: 0.88;
}


/* Mobile */

@media (max-width: 700px) {

  .cv-page {
    padding: 0 0.15rem 2rem;
  }

  .cv-header {
    display: block;
  }

  .cv-name {
    font-size: 2rem;
  }

  .cv-pdf-btn {
    margin-top: 1rem;
  }

  .cv-nav {
    line-height: 1.7;
  }

  .cv-entry {
    display: block;
    margin-bottom: 1.65rem;
  }

  .cv-entry-date {
    text-align: left;
    margin-top: 0.25rem;
  }

  .skill-row {
    display: block;
    margin-bottom: 1.1rem;
  }

  .skill-name {
    margin-bottom: 0.15rem;
  }

  .pub-item {
    grid-template-columns: 28px minmax(0, 1fr);
  }
}
</style>


<div class="cv-page">

  <!-- ================= HEADER ================= -->

  <div class="cv-header">

    <div>
      <h1 class="cv-name">Xiangping Liu</h1>

      <div class="cv-subtitle">
        Ph.D. Candidate in Biomedical Engineering
      </div>

      <div class="cv-affiliation">
        The University of Texas at Austin · Cockrell School of Engineering
      </div>

      <div class="cv-contact">
        <a href="mailto:liuxp1997@utexas.edu">liuxp1997@utexas.edu</a>

        <a href="https://scholar.google.com/citations?user=xNMmb4cAAAAJ"
           target="_blank" rel="noopener">
          Google Scholar
        </a>

        <a href="https://orcid.org/0000-0001-6554-8411"
           target="_blank" rel="noopener">
          ORCID
        </a>
      </div>
    </div>

    <div>
      <a class="cv-pdf-btn"
         href="{{ '/assets/pdf/Xiangping_Liu_CV.pdf' | relative_url }}"
         target="_blank">
        PDF ↓
      </a>
    </div>

  </div>


  <!-- ================= QUICK NAV ================= -->

  <div class="cv-nav">
    <a href="#education">Education</a>
    <a href="#research">Research</a>
    <a href="#publications">Publications</a>
    <a href="#presentations">Presentations</a>
    <a href="#teaching">Teaching & Mentoring</a>
    <a href="#awards">Awards</a>
    <a href="#service">Service</a>
    <a href="#skills">Skills</a>
  </div>


  <!-- ================= EDUCATION ================= -->

  <section class="cv-section" id="education">

    <h2 class="cv-section-title">Education</h2>

    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          The University of Texas at Austin
        </div>

        <div class="cv-entry-subtitle">
          Ph.D. Candidate in Biomedical Engineering
        </div>

        <div class="cv-entry-meta">
          Cockrell School of Engineering · Austin, TX, USA
        </div>
      </div>

      <div class="cv-entry-date">
        Aug 2022 – Present
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          Jilin University
        </div>

        <div class="cv-entry-subtitle">
          B.Sc. in Chemistry
        </div>

        <div class="cv-entry-meta">
          College of Chemistry · Changchun, China
        </div>
      </div>

      <div class="cv-entry-date">
        Sep 2015 – Jun 2019
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          Tsinghua University
        </div>

        <div class="cv-entry-subtitle">
          Summer School of Structural Biology, Chemical Biology and Medical Chemistry
        </div>

        <div class="cv-entry-meta">
          Center for Life Science · Beijing, China
        </div>
      </div>

      <div class="cv-entry-date">
        Summer 2017
      </div>
    </div>

  </section>


  <!-- ================= RESEARCH ================= -->

  <section class="cv-section" id="research">

    <h2 class="cv-section-title">Research Experience</h2>


    <div class="cv-research">

      <div class="cv-research-title">
        Ultrasound-Induced CaO<sub>2</sub>-Catalyzed Mechanoluminescent Nanoparticles
        for ChR2 Sono-Optogenetic Deep Brain Activation
      </div>

      <div class="cv-supervisor">
        Supervisor: Prof. Huiliang (Evan) Wang
      </div>

      <ul>
        <li>
          Developed Lipo@IR780/L012/CaO<sub>2</sub> liposomes with improved
          performance over first-generation organic blue mechanoluminescent
          nanoparticles by leveraging increased pH and H<sub>2</sub>O<sub>2</sub>
          generation.
        </li>

        <li>
          Demonstrated sono-optogenetic neuromodulation of the ventral tegmental
          area (VTA).
        </li>

        <li>
          Evaluated neuronal activation after VTA stimulation using c-Fos staining.
        </li>
      </ul>

    </div>


    <div class="cv-research">

      <div class="cv-research-title">
        Multicolored, Sonosensitizer-Optimized Organic Mechanoluminescent
        Nanoparticles for Functional Sono-Optogenetics
      </div>

      <div class="cv-supervisor">
        Supervisor: Prof. Huiliang (Evan) Wang
      </div>

      <ul>
        <li>
          Developed wavelength-tunable organic mechanoluminescent nanoparticles
          using FRET.
        </li>

        <li>
          Established a correlation between sonosensitizer energy gaps and ROS
          generation to guide sonosensitizer design and selection.
        </li>

        <li>
          Demonstrated bidirectional neuromodulation of genetically defined neurons
          using ChR2/ChRmine for activation and eOPN3 for inhibition.
        </li>
      </ul>

    </div>

  </section>


  <!-- ================= PUBLICATIONS ================= -->

  <section class="cv-section" id="publications">

    <h2 class="cv-section-title">Publications</h2>

    <div class="coauthor-note">
      † Co-first author. Xiangping Liu is shown in bold.
    </div>


    <div class="cv-subsection-title">
      First- and Co-first-Author Publications
    </div>


    <!-- 1 -->

    <div class="pub-item">

      <div class="pub-number">01</div>

      <div>
        <div class="pub-title">
          Multicolored, Sonosensitizer-Optimized Organic Mechanoluminescent
          Nanoparticles for Functional Sono-Optogenetics
        </div>

        <div class="pub-authors">
          <strong>Liu, X.</strong>; Wang, W.; Artman, B.; Diao, J.; Zhao, Y.;
          He, W.; Yu, S.; Tang, K. W. K.; Yao, M.; Gu, C.; Song, B.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>Journal of the American Chemical Society</em>,
          2026, <strong>148</strong>, 16809–16820.
        </div>
      </div>

    </div>


    <!-- 2 -->

    <div class="pub-item">

      <div class="pub-number">02</div>

      <div>
        <div class="pub-title">
          Organic Mechanoluminescent Nanoparticles for Biomedical Applications
        </div>

        <div class="pub-authors">
          Gu, C.; <strong>Liu, X.<sup>†</sup></strong>; Song, B.; Wang, W.;
          He, W.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>Chemical Science</em>,
          2025, <strong>16</strong> (28), 12702–12717.
        </div>
      </div>

    </div>


    <!-- 3 -->

    <div class="pub-item">

      <div class="pub-number">03</div>

      <div>
        <div class="pub-title">
          iBMEntored Buddy Program for First-Year International BME Doctoral Students
        </div>

        <div class="pub-authors">
          <strong>Liu, X.</strong>; Hsieh, J.-C.; Markey, M.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>ASEE-GSW Proceedings</em>, 2024.
        </div>
      </div>

    </div>


    <!-- 4 -->

    <div class="pub-item">

      <div class="pub-number">04</div>

      <div>
        <div class="pub-title">
          Ultrasound-Induced Cascade Amplification in a Mechanoluminescent
          Nanotransducer for Enhanced Sono-Optogenetic Deep Brain Stimulation
        </div>

        <div class="pub-authors">
          Wang, W.; Tang, K. W. K.; Pyatnitskiy, I.;
          <strong>Liu, X.<sup>†</sup></strong>; Shi, X.; Huo, D.; Jeong, J.;
          Wynn, T.; Sangani, A.; Baker, A.; Hsieh, J.-C.; Lozano, A. R.;
          Artman, B.; Fenno, L.; Buch, V. P.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>ACS Nano</em>,
          2023, <strong>17</strong> (24), 24936–24946.
        </div>
      </div>

    </div>


    <!-- 5 -->

    <div class="pub-item">

      <div class="pub-number">05</div>

      <div>
        <div class="pub-title">
          Ultra-Bright Heptamethine Dye Clusters Based on a Self-Adaptive
          Co-Assembly Strategy for NIR-IIb Biomedical Imaging
        </div>

        <div class="pub-authors">
          Dang, Z.; <strong>Liu, X.<sup>†</sup></strong>; Du, Y.; Wang, Y.;
          Zhou, D.; Zhang, Y.; Zhu, S.
        </div>

        <div class="pub-journal">
          <em>Advanced Materials</em>,
          2023, <strong>35</strong> (46), e2306773.
        </div>
      </div>

    </div>


    <div class="cv-subsection-title">
      Co-Author Publications
    </div>


    <!-- 6 -->

    <div class="pub-item">

      <div class="pub-number">06</div>

      <div>
        <div class="pub-title">
          Mechanoluminescent HOF Nanotransducers Enabled Sono-Optogenetics
          in Parkinsonian Rats
        </div>

        <div class="pub-authors">
          Wang, W.; Pyatnitskiy, I.; Shi, Y.; Tang, K. W. K.; Xie, Y.; Yu, S.;
          Wynn, T.; <strong>Liu, X.</strong>; Hsieh, J.-C.; Jeong, J.; He, W.;
          Artman, B.; Romero Lozano, A.; Shi, X.; Sangani, A.; Fenno, L. E.;
          Santacruz, S.; Chen, B.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>Advanced Functional Materials</em>, 2026, e76189.
        </div>
      </div>

    </div>


    <!-- 7 -->

    <div class="pub-item">

      <div class="pub-number">07</div>

      <div>
        <div class="pub-title">
          H-Bonded Organic Frameworks as Ultrasound-Programmable Delivery Platform
        </div>

        <div class="pub-authors">
          Wang, W.; Shi, Y.; Chai, W.; Tang, K. W. K.; Pyatnitskiy, I.; Xie, Y.;
          <strong>Liu, X.</strong>; He, W.; Jeong, J.; Hsieh, J.-C.; Lozano, A. R.;
          Artman, B.; Shi, X.; Hoefer, N.; Shrestha, B.; Stern, N. B.; Zhou, W.;
          McComb, D. W.; Porter, T.; Henkelman, G.; Chen, B.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>Nature</em>,
          2025, <strong>638</strong> (8050), 401–410.
        </div>
      </div>

    </div>


    <!-- 8 -->

    <div class="pub-item">

      <div class="pub-number">08</div>

      <div>
        <div class="pub-title">
          Bioadhesive Hydrogel-Coupled and Miniaturized Ultrasound Transducer
          System for Long-Term, Wearable Neuromodulation
        </div>

        <div class="pub-authors">
          Tang, K. W. K.; Jeong, J.; Hsieh, J.-C.; Yao, M.; Ding, H.; Wang, W.;
          <strong>Liu, X.</strong>; Pyatnitskiy, I.; He, W.; Moscoso-Barrera, W. D.;
          Lozano, A. R.; Artman, B.; Huh, H.; Wilson, P. S.; Wang, H.
        </div>

        <div class="pub-journal">
          <em>Nature Communications</em>,
          2025, <strong>16</strong> (1), 4940.
        </div>
      </div>

    </div>


    <!-- 9 -->

    <div class="pub-item">

      <div class="pub-number">09</div>

      <div>
        <div class="pub-title">
          Reversible Light-Responsive Protein Hydrogel for on-Demand Cell
          Encapsulation and Release
        </div>

        <div class="pub-authors">
          Narayan, O. P.; Dong, J.; Huang, M.; Chen, L.; Liu, L.; Nguyen, V.;
          Dozic, A. V.; <strong>Liu, X.</strong>; Wang, H.; Yin, Q.; Tang, X.;
          Guan, J.
        </div>

        <div class="pub-journal">
          <em>Acta Biomaterialia</em>, 2025, <strong>193</strong>, 202–214.
        </div>
      </div>

    </div>


    <!-- 10 -->

    <div class="pub-item">

      <div class="pub-number">10</div>

      <div>
        <div class="pub-title">
          Improved Performance of CsPbBr<sub>3</sub> Quantum-Dot Light-Emitting
          Diodes by Bottom Interface Modification
        </div>

        <div class="pub-authors">
          Zhao, Y.-Y.; Zhang, Q.-W.; Liu, Y.-F.; Lv, C.; Guo, S.;
          <strong>Liu, X.-P.</strong>; Bi, Y.-G.; Li, H.-W.; Wu, Y.-Q.
        </div>

        <div class="pub-journal">
          <em>Organic Electronics</em>, 2022, <strong>109</strong>, 106620.
        </div>
      </div>

    </div>


    <!-- 11 -->

    <div class="pub-item">

      <div class="pub-number">11</div>

      <div>
        <div class="pub-title">
          Super-Stable Cyanine@Albumin Fluorophore for Enhanced NIR-II Bioimaging
        </div>

        <div class="pub-authors">
          Bai, L.; Hu, Z.; Han, T.; Wang, Y.; Xu, J.; Jiang, G.; Feng, X.;
          Sun, B.; <strong>Liu, X.</strong>; Tian, R.; Sun, H.; Zhang, S.;
          Chen, X.; Zhu, S.
        </div>

        <div class="pub-journal">
          <em>Theranostics</em>,
          2022, <strong>12</strong> (10), 4536–4547.
        </div>
      </div>

    </div>


    <!-- 12 -->

    <div class="pub-item">

      <div class="pub-number">12</div>

      <div>
        <div class="pub-title">
          Surfactant-Chaperoned Donor-Acceptor-Donor NIR-II Dye Strategy
          Efficiently Circumvents Intermolecular Aggregation to Afford Enhanced
          Bioimaging Contrast
        </div>

        <div class="pub-authors">
          Han, T.; Wang, Y.; Xu, J.; Zhu, N.; Bai, L.; <strong>Liu, X.</strong>;
          Sun, B.; Yu, C.; Meng, Q.; Wang, J.; Su, Q.; Cai, Q.; Hettie, K. S.;
          Zhang, Y.; Zhu, S.; Yang, B.
        </div>

        <div class="pub-journal">
          <em>Chemical Science</em>,
          2022, <strong>13</strong> (44), 13201–13211.
        </div>
      </div>

    </div>


    <!-- 13 -->

    <div class="pub-item">

      <div class="pub-number">13</div>

      <div>
        <div class="pub-title">
          Near-Infrared-II Cyanine/Polymethine Dyes, Current State and Perspective
        </div>

        <div class="pub-authors">
          Du, Y.; <strong>Liu, X.</strong>; Zhu, S.
        </div>

        <div class="pub-journal">
          <em>Frontiers in Chemistry</em>, 2021, <strong>9</strong>, 718709.
        </div>
      </div>

    </div>


    <!-- 14 -->

    <div class="pub-item">

      <div class="pub-number">14</div>

      <div>
        <div class="pub-title">
          Indole Carbonized Polymer Dots Boost Full-Color Emission by Regulating
          Surface State
        </div>

        <div class="pub-authors">
          Liu, C.; Jin, Y.; Wang, R.; Han, T.; <strong>Liu, X.</strong>;
          Wang, B.; Huang, C.; Zhu, S.; Chen, J.
        </div>

        <div class="pub-journal">
          <em>iScience</em>, 2020, <strong>23</strong> (10), 101546.
        </div>
      </div>

    </div>

  </section>


  <!-- ================= PRESENTATIONS ================= -->

  <section class="cv-section" id="presentations">

    <h2 class="cv-section-title">Presentations</h2>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          Multicolored Mechanoluminescent Nanoparticles for Functional Sono-Optogenetics
        </div>

        <div class="cv-entry-subtitle">
          <span class="presentation-type">ORAL</span>
          2025 MRS Fall Meeting & Exhibit
        </div>

        <div class="cv-entry-meta">
          Boston, MA
        </div>
      </div>

      <div class="cv-entry-date">
        Dec 2025
      </div>

    </div>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          Multicolored Mechanoluminescent Nanoparticles for Functional Sono-Optogenetics
        </div>

        <div class="cv-entry-subtitle">
          <span class="presentation-type">POSTER</span>
          23rd International Nanomedicine and Drug Delivery Symposium (NanoDDS 2025)
        </div>

        <div class="cv-entry-meta">
          Houston, TX
        </div>
      </div>

      <div class="cv-entry-date">
        Oct 2025
      </div>

    </div>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          iBMEntored Buddy Program for First-Year International Doctoral Students
        </div>

        <div class="cv-entry-subtitle">
          <span class="presentation-type">POSTER</span>
          BMES 2024 Annual Meeting
        </div>

        <div class="cv-entry-meta">
          Baltimore, MD
        </div>
      </div>

      <div class="cv-entry-date">
        Oct 2024
      </div>

    </div>

  </section>


  <!-- ================= TEACHING ================= -->

  <section class="cv-section" id="teaching">

    <h2 class="cv-section-title">Teaching &amp; Mentoring</h2>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          CREATE Undergraduate Research Mentor
        </div>

        <div class="cv-entry-subtitle">
          The University of Texas at Austin
        </div>

        <div class="cv-entry-meta">
          Mentoring a CREATE Summer Research Intern in HOF nanoparticle fabrication,
          focused ultrasound-triggered mechanoluminescence experiments, and
          nanoparticle characterization.
        </div>
      </div>

      <div class="cv-entry-date">
        Summer 2026
      </div>

    </div>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          Undergraduate Research Mentor
        </div>

        <div class="cv-entry-subtitle">
          The University of Texas at Austin
        </div>

        <div class="cv-entry-meta">
          Providing training in mechanoluminescent nanoparticle and HOF fabrication
          and related equipment use.
        </div>
      </div>

      <div class="cv-entry-date">
        Fall 2025 – Present
      </div>

    </div>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          Undergraduate Research Mentor
        </div>

        <div class="cv-entry-subtitle">
          The University of Texas at Austin
        </div>

        <div class="cv-entry-meta">
          Guided an undergraduate researcher in writing a review on organic
          mechanoluminescent nanoparticles for biomedical applications, published
          in <em>Chemical Science</em>.
        </div>
      </div>

      <div class="cv-entry-date">
        Fall 2024 – Spring 2025
      </div>

    </div>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          iBMEntored Program — Mentor
        </div>

        <div class="cv-entry-subtitle">
          The University of Texas at Austin
        </div>

        <div class="cv-entry-meta">
          Mentored first-year international BME doctoral students through the
          iBMEntored buddy program.
        </div>
      </div>

      <div class="cv-entry-date">
        Fall 2023 – Spring 2025
      </div>

    </div>


    <div class="cv-entry">

      <div>
        <div class="cv-entry-title">
          BME 365R Engineering Physiology I — Teaching Assistant
        </div>

        <div class="cv-entry-subtitle">
          The University of Texas at Austin
        </div>

        <div class="cv-entry-meta">
          Led discussion sections and graded assignments. Instructors:
          Prof. Amy Brock and Prof. H. Grady Rylander III.
        </div>
      </div>

      <div class="cv-entry-date">
        Fall 2023
      </div>

    </div>

  </section>


  <!-- ================= AWARDS ================= -->

  <section class="cv-section" id="awards">

    <h2 class="cv-section-title">Honors &amp; Awards</h2>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          Gregg and Marilyn Harris Endowed Graduate Fellow
        </div>
      </div>

      <div class="cv-entry-date">2026</div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          BME Professional Development Award
        </div>

        <div class="cv-entry-meta">
          The University of Texas at Austin
        </div>
      </div>

      <div class="cv-entry-date">2026</div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          BME Professional Development Award
        </div>

        <div class="cv-entry-meta">
          The University of Texas at Austin
        </div>
      </div>

      <div class="cv-entry-date">2025</div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          UT Austin Engineering Fellowship
        </div>
      </div>

      <div class="cv-entry-date">2022</div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          First Prize Scholarship
        </div>

        <div class="cv-entry-meta">
          Jilin University
        </div>
      </div>

      <div class="cv-entry-date">2019</div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">
          Chinese National Endeavor Scholarship
        </div>
      </div>

      <div class="cv-entry-date">2016</div>
    </div>

  </section>


  <!-- ================= SERVICE ================= -->

  <section class="cv-section" id="service">

    <h2 class="cv-section-title">Academic Service</h2>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">Ad Hoc Reviewer</div>
        <div class="cv-entry-subtitle"><em>Nano Letters</em></div>
      </div>

      <div class="cv-entry-date">
        2025 – Present
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">Ad Hoc Reviewer</div>
        <div class="cv-entry-subtitle">
          <em>Biosensors and Bioelectronics</em>
        </div>
      </div>

      <div class="cv-entry-date">
        2026 – Present
      </div>
    </div>


    <div class="cv-entry">
      <div>
        <div class="cv-entry-title">Ad Hoc Reviewer</div>
        <div class="cv-entry-subtitle">
          <em>Nature Biotechnology</em>
        </div>
      </div>

      <div class="cv-entry-date">
        2026 – Present
      </div>
    </div>

  </section>


  <!-- ================= SKILLS ================= -->

  <section class="cv-section" id="skills">

    <h2 class="cv-section-title">Skills</h2>


    <div class="skill-row">

      <div class="skill-name">
        Nanomaterials &amp; Chemistry
      </div>

      <div class="skill-content">
        Organic synthesis; HOFs; polymeric nanoparticles; micelle/liposome
        formulation; drug loading; surface functionalization; bioconjugation;
        click chemistry.
      </div>

    </div>


    <div class="skill-row">

      <div class="skill-name">
        Characterization &amp; Imaging
      </div>

      <div class="skill-content">
        TEM; STEM; SEM; EDS; DLS; zeta potential; UV-Vis;
        fluorescence/chemiluminescence spectroscopy and imaging; NMR; HPLC;
        MALDI-TOF; confocal microscopy; NIR-II imaging.
      </div>

    </div>


    <div class="skill-row">

      <div class="skill-name">
        Ultrasound &amp; Neuroengineering
      </div>

      <div class="skill-content">
        Focused ultrasound (FUS); ultrasound-triggered drug delivery;
        sono-optogenetics; MEA recording; fiber photometry; laser speckle
        contrast imaging (LSCI).
      </div>

    </div>


    <div class="skill-row">

      <div class="skill-name">
        Biological Techniques
      </div>

      <div class="skill-content">
        Mammalian cell culture; primary neuron preparation; stereotactic surgery;
        IV/intracranial injection; rodent neuromodulation; photothrombotic stroke
        models.
      </div>

    </div>


    <div class="skill-row">

      <div class="skill-name">
        Software &amp; Programming
      </div>

      <div class="skill-content">
        MATLAB; Python; C; ImageJ/Fiji; Origin; ChemDraw; Gaussian; MestReNova;
        Maestro; Spartan; EndNote; Cinema 4D; 3ds Max.
      </div>

    </div>

  </section>

</div>
