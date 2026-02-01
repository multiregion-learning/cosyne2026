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
      <img src="/assets/images/aaron-batista.jpg" alt="Aaron Batista">
      <p class="speaker-name"><a href="https://www.cnup.pitt.edu/people/aaron-batista-phd" target="_blank">Aaron Batista</a></p>
      <p class="speaker-institution">University of Pittsburgh</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/kayvon-daie.jpg" alt="Kayvon Daie">
      <p class="speaker-name"><a href="https://www.allenneuraldynamics.org/people/kayvon-daie" target="_blank">Kayvon Daie</a></p>
      <p class="speaker-institution">Allen Institute</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
    </div>
  </div>

  <div class="speaker-row" data-category="computational">
    <div class="speaker-photo">
      <img src="/assets/images/lea-duncker.jpg" alt="Lea Duncker">
      <p class="speaker-name"><a href="https://zuckermaninstitute.columbia.edu/lea-duncker-phd" target="_blank">Lea Duncker</a></p>
      <p class="speaker-institution">Columbia University</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/hidehiko-inagaki.jpg" alt="Hidehiko Inagaki">
      <p class="speaker-name"><a href="https://mpfi.org/science/our-labs/inagaki-lab/" target="_blank">Hidehiko Inagaki</a></p>
      <p class="speaker-institution">Max Planck Florida Institute for Neuroscience</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/jeff-magee.jpg" alt="Jeff Magee">
      <p class="speaker-name"><a href="https://themageelab.org/" target="_blank">Jeff Magee</a></p>
      <p class="speaker-institution">Baylor College of Medicine, HHMI</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
    </div>
  </div>

  <div class="speaker-row" data-category="computational">
    <div class="speaker-photo">
      <img src="/assets/images/cengiz-pehlevan.jpg" alt="Cengiz Pehlevan">
      <p class="speaker-name"><a href="https://pehlevan.seas.harvard.edu/people/cengiz-pehlevan" target="_blank">Cengiz Pehlevan</a></p>
      <p class="speaker-institution">Harvard University</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
    </div>
  </div>

  <div class="speaker-row" data-category="experimental">
    <div class="speaker-photo">
      <img src="/assets/images/xulu-sun.jpg" alt="Xulu Sun">
      <p class="speaker-name">Xulu Sun</p>
      <p class="speaker-institution">UCSF</p>
    </div>
    <div class="speaker-talk">
      <p class="talk-title">Talk title coming soon</p>
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
