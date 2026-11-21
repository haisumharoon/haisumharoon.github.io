---
layout: page
title: Music
permalink: /music/
description: Piano, and why I keep it next to research.
nav: true
nav_order: 5
---

<div class="piano-page">

  <p class="pp-lede">
    I play piano. It is the part of my day where nothing gets submitted, reviewed, or revised by anyone but me.
  </p>

  <!-- Playable keyboard. Built by the script at the bottom of this file. -->
  <div class="pp-keys" id="ppKeys" role="group" aria-label="Small piano keyboard. Press a key to hear a note."></div>
  <p class="pp-hint">Try the keys. They are real notes.</p>

  <!-- ========== ROW 1: text | Instagram photo | your own mp4 ==========
       Upload your video to the repo as: assets/video/piano-main.mp4
       (GitHub: Add file > Upload files. Keep it under about 20 MB.)
  -->
  <section class="pp-feature">

    <div class="pp-text">
      <h2>Cornfield Chase</h2>
      <p class="pp-meta">Hans Zimmer, from Interstellar.</p>
      <p>
        My favorite piece to play. The slow build from a simple pattern into something huge is what keeps me coming back.
        Interstellar is also the film that made me want to understand how things work.
      </p>
    </div>

    <div class="pp-photo">
      <blockquote class="instagram-media" data-instgrm-permalink="https://www.instagram.com/p/DSsraZFDGTI/" data-instgrm-version="14" style="background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin:0; max-width:540px; min-width:0; padding:0; width:100%;"><a href="https://www.instagram.com/p/DSsraZFDGTI/" target="_blank" rel="noopener">View on Instagram</a></blockquote>
    </div>

    <div class="pp-video">
      <video controls playsinline preload="metadata">
        <source src="/assets/video/Interstellar.mp4#t=0.1" type="video/mp4">
        Your browser cannot play this video.
      </video>
    </div>

  </section>

  <!-- ========== ROW 2: three Instagram reels ==========
       To change one, replace the link in BOTH places inside its block. -->
  <h2 class="pp-h2">More recordings</h2>
  <div class="pp-grid">

    <div class="pp-reelbox">
      <blockquote class="instagram-media" data-instgrm-permalink="https://www.instagram.com/reel/DW60T3HjBZa/" data-instgrm-version="14" style="background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin:0; max-width:540px; min-width:0; padding:0; width:100%;"><a href="https://www.instagram.com/reel/DW60T3HjBZa/" target="_blank" rel="noopener">View on Instagram</a></blockquote>
    </div>

    <div class="pp-reelbox">
      <blockquote class="instagram-media" data-instgrm-permalink="https://www.instagram.com/reel/DKAXO6KsPJC/" data-instgrm-version="14" style="background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin:0; max-width:540px; min-width:0; padding:0; width:100%;"><a href="https://www.instagram.com/reel/DKAXO6KsPJC/" target="_blank" rel="noopener">View on Instagram</a></blockquote>
    </div>

    <div class="pp-reelbox">
      <blockquote class="instagram-media" data-instgrm-permalink="https://www.instagram.com/reel/DJym54xtU9s/" data-instgrm-version="14" style="background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin:0; max-width:540px; min-width:0; padding:0; width:100%;"><a href="https://www.instagram.com/reel/DJym54xtU9s/" target="_blank" rel="noopener">View on Instagram</a></blockquote>
    </div>

  </div>

  <p class="pp-foot">
    More on Instagram: <a href="https://www.instagram.com/haisumplays/" target="_blank" rel="noopener">@haisumplays</a>.
  </p>

</div>

<style>
  .piano-page {
    --pp-gap: 1.25rem;
    max-width: 880px;
    margin: 0 auto;
    container-type: inline-size;
  }

  .pp-lede {
    font-family: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
    font-size: 1.55rem;
    line-height: 1.45;
    max-width: 34em;
    margin: 0.5rem 0 2rem;
  }

  /* ---- keyboard ---- */
  .pp-keys {
    position: relative;
    display: flex;
    height: 120px;
    border-radius: 0 0 8px 8px;
    border-top: 6px solid var(--global-theme-color);
    user-select: none;
    touch-action: manipulation;
  }
  .pp-white {
    flex: 1;
    background: #f6f2e8;
    border: 1px solid #b9b4a6;
    border-top: 0;
    border-radius: 0 0 5px 5px;
    cursor: pointer;
    padding: 0;
    transition: transform 70ms ease, background 70ms ease;
    transform-origin: top;
  }
  .pp-white:hover { background: #ece6d6; }
  .pp-black {
    position: absolute;
    top: 0;
    width: 4.4%;
    height: 62%;
    margin-left: -2.2%;
    background: #1d1c21;
    border: 0;
    border-radius: 0 0 4px 4px;
    cursor: pointer;
    padding: 0;
    z-index: 2;
    transition: transform 70ms ease, background 70ms ease;
    transform-origin: top;
  }
  .pp-black:hover { background: #34323b; }
  .pp-white.down, .pp-black.down { transform: scaleY(0.96); background: var(--global-theme-color); }
  .pp-white:focus-visible, .pp-black:focus-visible { outline: 3px solid var(--global-theme-color); outline-offset: 2px; z-index: 3; }
  .pp-hint { font-size: 0.85rem; color: var(--global-text-color-light); margin: 0.6rem 0 3rem; }

  /* ---- row 1: three equal columns, same as the reels row below ---- */
  .pp-feature {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    grid-template-areas:
      "text  video"
      "photo video";
    column-gap: var(--pp-gap);
    row-gap: 1rem;
    align-items: start;
    margin-bottom: 3rem;
  }
  .pp-text  { grid-area: text; }
  .pp-photo { grid-area: photo; max-width: 300px; width: 100%; }
  .pp-video { grid-area: video; align-self: stretch; min-height: 420px; }

  .pp-text h2 {
    font-family: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
    font-size: 1.6rem;
    margin: 0 0 0.3rem;
    border: 0;
  }
  .pp-meta { color: var(--global-text-color-light); margin-bottom: 1rem; font-size: 0.95rem; }

  /* mp4 frame: at least 9:16, and grows to match the photo next to it */
  .pp-video {
    position: relative;
    background: #000;
    border-radius: 3px;
    overflow: hidden;
  }
  .pp-video video {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: contain;
    background: #000;
  }

  .pp-h2 {
    font-family: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
    font-size: 1.5rem;
    border: 0;
    margin-bottom: 1.2rem;
  }

  /* ---- row 2: three reels in one row ---- */
  .pp-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: var(--pp-gap);
    align-items: start;
  }
  .pp-foot { margin-top: 3rem; font-size: 0.9rem; color: var(--global-text-color-light); }

  /* Let Instagram's embed shrink to the column width */
  .piano-page iframe.instagram-media,
  .piano-page blockquote.instagram-media {
    min-width: 0 !important;
    max-width: 100% !important;
    width: 100% !important;
    margin: 0 !important;
  }

  /* ---- narrow layouts: everything stacks in one column ---- */
  @container (max-width: 700px) {
    .pp-feature {
      grid-template-columns: minmax(0, 1fr);
      grid-template-areas:
        "text"
        "video"
        "photo";
      max-width: 400px;
    }
    .pp-grid { grid-template-columns: minmax(0, 1fr); max-width: 400px; }
    .pp-video { aspect-ratio: 9 / 16; min-height: 0; }
    .pp-keys { height: 96px; }
    .pp-lede { font-size: 1.3rem; }
  }
  @media (prefers-reduced-motion: reduce) {
    .pp-white, .pp-black { transition: none; }
  }
</style>

<script>
(function () {
  /* ---------- Keyboard: C4 to B5, two octaves ---------- */
  var root = document.getElementById('ppKeys');
  if (!root) return;

  var whiteSteps = [0, 2, 4, 5, 7, 9, 11];
  var blackAfter = { 0: 1, 1: 3, 3: 6, 4: 8, 5: 10 };
  var whiteCount = 14, startMidi = 60;
  var ctx = null;

  function freq(m) { return 440 * Math.pow(2, (m - 69) / 12); }

  function play(m) {
    try {
      ctx = ctx || new (window.AudioContext || window.webkitAudioContext)();
      if (ctx.state === 'suspended') ctx.resume();
      var t = ctx.currentTime;
      var out = ctx.createGain();
      out.gain.setValueAtTime(0.0001, t);
      out.gain.exponentialRampToValueAtTime(0.35, t + 0.01);
      out.gain.exponentialRampToValueAtTime(0.0001, t + 1.6);
      out.connect(ctx.destination);
      [[1, 1], [2, 0.35], [3, 0.12]].forEach(function (p) {
        var o = ctx.createOscillator(), g = ctx.createGain();
        o.type = 'sine';
        o.frequency.value = freq(m) * p[0];
        g.gain.value = p[1];
        o.connect(g); g.connect(out);
        o.start(t); o.stop(t + 1.7);
      });
    } catch (e) { /* audio blocked: keys still animate */ }
  }

  function press(el, m) {
    el.classList.add('down');
    setTimeout(function () { el.classList.remove('down'); }, 140);
    play(m);
  }

  var names = ['C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#', 'A', 'A#', 'B'];
  function label(m) { return names[m % 12] + (Math.floor(m / 12) - 1); }

  for (var i = 0; i < whiteCount; i++) {
    (function (i) {
      var m = startMidi + Math.floor(i / 7) * 12 + whiteSteps[i % 7];
      var w = document.createElement('button');
      w.type = 'button';
      w.className = 'pp-white';
      w.setAttribute('aria-label', label(m));
      w.addEventListener('pointerdown', function () { press(w, m); });
      w.addEventListener('keydown', function (e) {
        if (e.key === 'Enter' || e.key === ' ') { e.preventDefault(); press(w, m); }
      });
      root.appendChild(w);

      if (blackAfter.hasOwnProperty(i % 7) && i < whiteCount - 1) {
        var bm = startMidi + Math.floor(i / 7) * 12 + blackAfter[i % 7];
        var b = document.createElement('button');
        b.type = 'button';
        b.className = 'pp-black';
        b.style.left = ((i + 1) * 100 / whiteCount) + '%';
        b.setAttribute('aria-label', label(bm));
        b.addEventListener('pointerdown', function (e) { e.stopPropagation(); press(b, bm); });
        b.addEventListener('keydown', function (e) {
          if (e.key === 'Enter' || e.key === ' ') { e.preventDefault(); press(b, bm); }
        });
        root.appendChild(b);
      }
    })(i);
  }
})();
</script>

<!-- Instagram's own script turns each blockquote above into a live embed. -->
<script async src="https://www.instagram.com/embed.js"></script>
