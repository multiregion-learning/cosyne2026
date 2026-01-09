---
title: Speakers
layout: single
permalink: /speakers/
---

<div class="speaker-filters">
  <button class="filter-btn active" data-filter="all">All</button>
  <button class="filter-btn" data-filter="experimental">Experimental</button>
  <button class="filter-btn" data-filter="computational">Computational</button>
</div>

<div class="speaker-list">

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 1">
      <p class="speaker-name">Speaker Name 1</p>
      <p class="speaker-institution">Institution 1</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 1: Placeholder Title for the First Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="computational">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 2">
      <p class="speaker-name">Speaker Name 2</p>
      <p class="speaker-institution">Institution 2</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 2: Placeholder Title for the Second Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 3">
      <p class="speaker-name">Speaker Name 3</p>
      <p class="speaker-institution">Institution 3</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 3: Placeholder Title for the Third Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="computational">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 4">
      <p class="speaker-name">Speaker Name 4</p>
      <p class="speaker-institution">Institution 4</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 4: Placeholder Title for the Fourth Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 5">
      <p class="speaker-name">Speaker Name 5</p>
      <p class="speaker-institution">Institution 5</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 5: Placeholder Title for the Fifth Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="computational">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 6">
      <p class="speaker-name">Speaker Name 6</p>
      <p class="speaker-institution">Institution 6</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 6: Placeholder Title for the Sixth Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 7">
      <p class="speaker-name">Speaker Name 7</p>
      <p class="speaker-institution">Institution 7</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 7: Placeholder Title for the Seventh Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="computational">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 8">
      <p class="speaker-name">Speaker Name 8</p>
      <p class="speaker-institution">Institution 8</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 8: Placeholder Title for the Eighth Speaker's Presentation</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/placeholder-person.jpg" alt="Speaker 9">
      <p class="speaker-name">Speaker Name 9</p>
      <p class="speaker-institution">Institution 9</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk Title 9: Placeholder Title for the Ninth Speaker's Presentation</p>
    </div>
  </div>

</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const filterBtns = document.querySelectorAll('.filter-btn');
  const speakerRows = document.querySelectorAll('.speaker-row');

  filterBtns.forEach(btn => {
    btn.addEventListener('click', function() {
      // Update active button
      filterBtns.forEach(b => b.classList.remove('active'));
      this.classList.add('active');

      // Filter speakers
      const filter = this.getAttribute('data-filter');

      speakerRows.forEach(row => {
        if (filter === 'all' || row.getAttribute('data-category') === filter) {
          row.style.display = 'flex';
        } else {
          row.style.display = 'none';
        }
      });
    });
  });
});
</script>
