
<script setup>
const sections = [
  { id: 'overview', title: 'Overview' },
  { id: 'technology', title: 'Technology' },
  { id: 'research', title: 'Research' },
  { id: 'team', title: 'Team' },
]
</script>

<template>
  <div class="page">
    <header class="header">
      <a href="#" class="logo">OrbitalRailguns</a>

      <nav>
        <a
          v-for="section in sections"
          :key="section.id"
          :href="`#${section.id}`"
        >
          {{ section.title }}
        </a>
      </nav>
    </header>

    <main>
      <section class="intro">
        <p class="eyebrow">CONRAD CHALLENGE · 2026</p>

        <h1>OrbitalRailguns</h1>

        <p class="subtitle">
          Exploring electromagnetic propulsion for the future
          of space transportation.
        </p>

        <a href="#overview" class="link">Explore the project ↓</a>
      </section>

      <section id="overview" class="section">
        <h2>Project Overview</h2>
        <p>
          Introduce the problem your project addresses, the motivation
          behind your idea, and the overall concept.
        </p>
      </section>

      <section id="technology" class="section">
        <h2>Technology</h2>
        <p>
          Explain the science and engineering behind your proposed
          electromagnetic propulsion system.
        </p>
      </section>

      <section id="research" class="section">
        <h2>Research & Development</h2>
        <p>
          Present your research, calculations, design process,
          experiments, and findings.
        </p>
      </section>

      <section id="team" class="section">
        <h2>Our Team</h2>
        <p>
          Introduce your team members and their contributions.
        </p>
      </section>
    </main>

    <footer>
      OrbitalRailguns · Conrad Challenge 2026
    </footer>
  </div>
</template>
