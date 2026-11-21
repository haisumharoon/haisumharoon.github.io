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

  <!--
    HOW TO ADD A VIDEO: paste the full Instagram link into data-ig.
    Post links (/p/...) and reel links (/reel/...) both work.
    Delete any <figure> block you do not need.
  -->

  <!-- ========== FEATURED PIECE ========== -->
  <section class="pp-feature">
    <div class="pp-feature-text">
      <h2>[Piece title]</h2>
      <p class="pp-meta">[Composer or "Original"]. Recorded [Month Year].</p>
      <p>
        [Two or three plain sentences. Why you chose this piece, what makes it hard,
        or what it means to you. Specific is better than polished.]
      </p>
    </div>
    <div class="pp-reel" data-ig="https://www.instagram.com/p/C3fjeJINm6yqwB1eWevAm3kvDCEUvE_QV2MPKg0/" data-title="[Piece title]">
      <button type="button" class="pp-play" aria-label="Load and play: [Piece title]">
        <span class="pp-tri" aria-hidden="true"></span>
        <span class="pp-play-title">[Piece title]</span>
        <span class="pp-play-sub">Tap to load video</span>
      </button>
    </div>
  </section>

  <!-- ========== MORE RECORDINGS ========== -->
  <h2 class="pp-h2">More recordings</h2>
  <div class="pp-grid">

    <figure>
      <div class="pp-reel" data-ig="PASTE_INSTAGRAM_LINK_2" data-title="[Piece 2]">
        <button type="button" class="pp-play" aria-label="Load and play: [Piece 2]">
          <span class="pp-tri" aria-hidden="true"></span>
          <span class="pp-play-title">[Piece 2]</span>
          <span class="pp-play-sub">Tap to load video</span>
        </button>
      </div>
      <figcaption><strong>[Piece 2]</strong><br>[Composer]. One line about it.</figcaption>
    </figure>

    <figure>
      <div class="pp-reel" data-ig="PASTE_INSTAGRAM_LINK_3" data-title="[Piece 3]">
        <button type="button" class="pp-play" aria-label="Load and play: [Piece 3]">
          <span class="pp-tri" aria-hidden="true"></span>
          <span class="pp-play-title">[Piece 3]</span>
          <span class="pp-play-sub">Tap to load video</span>
        </button>
      </div>
      <figcaption><strong>[Piece 3]</strong><br>[Composer]. One line about it.</figcaption>
    </figure>

    <figure>
      <div class="pp-reel" data-ig="PASTE_INSTAGRAM_LINK_4" data-title="[Piece 4]">
        <button type="button" class="pp-play" aria-label="Load and play: [Piece 4]">
          <span class="pp-tri" aria-hidden="true"></span>
          <span class="pp-play-title">[Piece 4]</span>
          <span class="pp-play-sub">Tap to load video</span>
        </button>
      </div>
      <figcaption><strong>[Piece 4]</strong><br>[Composer]. One line about it.</figcaption>
    </figure>

  </div>

  <p class="pp-foot">
    More on Instagram: <a href="https://www.instagram.com/YOUR_HANDLE/" target="_blank" rel="noopener">@YOUR_HANDLE</a>.
    Videos load from Instagram only when you press play, so this page stays fast and does not track you on arrival.
  </p>

</div>

<style>
  .piano-page { max-width: 880px; margin: 0 auto; }

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

  /* ---- featured ---- */
  .pp-feature {
    display: grid;
    grid-template-columns: 1fr 340px;
    gap: 2.5rem;
    align-items: start;
    margin-bottom: 3.5rem;
  }
  .pp-feature h2 {
    font-family: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
    font-size: 2rem;
    margin: 0 0 0.3rem;
    border: 0;
  }
  .pp-meta { color: var(--global-text-color-light); margin-bottom: 1rem; }

  .pp-h2 {
    font-family: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
    font-size: 1.5rem;
    border: 0;
    margin-bottom: 1.2rem;
  }

  /* ---- video frame (shared) ---- */
  .pp-reel {
    position: relative;
    width: 100%;
    max-width: 340px;
    height: 600px;
    background: #1d1c21;
    border-radius: 10px;
    overflow: hidden;
  }
  .pp-reel iframe { width: 100%; height: 100%; border: 0; background: #fff; }
  .pp-play {
    all: unset;
    box-sizing: border-box;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 0.6rem;
    cursor: pointer;
    color: #f6f2e8;
    text-align: center;
    padding: 1rem;
    /* faint key stripes, so empty frames still look like piano */
    background: repeating-linear-gradient(90deg, #1d1c21 0, #1d1c21 38px, #26252b 38px, #26252b 40px);
  }
  .pp-play:hover .pp-tri { transform: scale(1.08); }
  .pp-play:focus-visible { outline: 3px solid var(--global-theme-color); outline-offset: -6px; }
  .pp-tri {
    width: 0; height: 0;
    border-left: 34px solid var(--global-theme-color);
    border-top: 21px solid transparent;
    border-bottom: 21px solid transparent;
    margin-left: 10px;
    transition: transform 120ms ease;
  }
  .pp-play-title {
    font-family: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
    font-size: 1.3rem;
  }
  .pp-play-sub { font-size: 0.85rem; opacity: 0.7; }
  .pp-open { display: block; margin-top: 0.5rem; font-size: 0.85rem; }

  /* ---- grid ---- */
  .pp-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 2rem 1.5rem;
  }
  .pp-grid figure { margin: 0; }
  .pp-grid figcaption { margin-top: 0.7rem; font-size: 0.95rem; line-height: 1.45; max-width: 340px; }
  .pp-foot { margin-top: 3rem; font-size: 0.9rem; color: var(--global-text-color-light); max-width: 38em; }

  @media (max-width: 760px) {
    .pp-feature { grid-template-columns: 1fr; gap: 1.5rem; }
    .pp-keys { height: 96px; }
    .pp-lede { font-size: 1.3rem; }
  }
  @media (prefers-reduced-motion: reduce) {
    .pp-white, .pp-black, .pp-tri { transition: none; }
  }
</style>

<script>
(function () {
  /* ---------- 1. Keyboard: C4 to B5, two octaves ---------- */
  var root = document.getElementById('ppKeys');
  if (root) {
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
  }

  /* ---------- 2. Click to load Instagram posts and reels ---------- */
  // Accepts a full link (post, reel or tv), "p/ID", "reel/ID", or a bare reel ID.
  function parseIG(s) {
    if (!s) return null;
    s = s.trim();
    var m = s.match(/instagram\.com\/(p|reels?|tv)\/([A-Za-z0-9_-]+)/i);
    if (!m) m = s.match(/^(p|reels?|tv)\/([A-Za-z0-9_-]+)$/i);
    if (m) {
      var kind = m[1].toLowerCase();
      if (kind === 'reels') kind = 'reel';
      return { kind: kind, id: m[2] };
    }
    if (/^[A-Za-z0-9_-]+$/.test(s) && s.indexOf('PASTE') !== 0) return { kind: 'reel', id: s };
    return null;
  }

  document.querySelectorAll('.pp-reel').forEach(function (box) {
    var btn = box.querySelector('.pp-play');
    var ig = parseIG(box.getAttribute('data-ig'));
    if (!btn) return;

    if (ig) {
      // small fallback link under the frame, in case an embed is blocked
      var a = document.createElement('a');
      a.className = 'pp-open';
      a.href = 'https://www.instagram.com/' + ig.kind + '/' + ig.id + '/';
      a.target = '_blank';
      a.rel = 'noopener';
      a.textContent = 'Open on Instagram';
      box.parentNode.insertBefore(a, box.nextSibling);
    }

    btn.addEventListener('click', function () {
      if (!ig) return; // placeholder link not replaced yet
      var f = document.createElement('iframe');
      f.src = 'https://www.instagram.com/' + ig.kind + '/' + ig.id + '/embed/';
      f.title = box.getAttribute('data-title') || 'Piano recording';
      f.setAttribute('allowtransparency', 'true');
      f.setAttribute('allow', 'encrypted-media; fullscreen');
      f.setAttribute('scrolling', 'no');
      box.innerHTML = '';
      box.appendChild(f);
    });
  });
})();
</script>
