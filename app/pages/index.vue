<script setup lang="ts">
  import { CodeXml, ExternalLink } from '@lucide/vue'
</script>

<template>
  <div >
    <!-- Hero -->
    <main class="py-25 max-[600px]:py-17.5">
      <div class="mb-5 font-mono text-sm text-accent">
        $ whoami
      </div>

      <h1
        class="m-0 dark:text-white text-[clamp(42px,8vw,72px)] font-semibold leading-none tracking-tighter"
      >
        Samuel Nandi
      </h1>

      <div class="mt-4.5 font-mono text-base text-muted">
        Software Engineer
      </div>

      <p
        class="mt-8 max-w-150 text-lg leading-[1.6] text-muted dark:text-[#a3a3a3]"
      >
        I build web applications, internal tools, and software
        that solve practical problems.
      </p>

      <div
        class="mt-7.5 flex gap-4.5 font-mono text-[13px]"
      >
        <a
          href="https://github.com/ssnnee"
          target="_blank"
          rel="noopener noreferrer"
          class="border-b border-(--border) pb-0.75 text-muted dark:text-[#a3a3a3] transition-colors hover:text-accent"
        >
          github ↗
        </a>

        <a
          href="mailto:hello@example.com"
          class="border-b border-(--border) pb-0.75 text-muted dark:text-[#a3a3a3] transition-colors hover:text-accent"
        >
          email ↗
        </a>
      </div>
    </main>
    <USeparator class="h-2" />

    <!-- About -->
    <section
      id="about"
      class="py-20"
    >
      <div
        class="relative mb-10 flex items-center gap-3 font-mono text-[14px] before:text-accent before:content-['$']"
      >
        cat about.txt
      </div>

      <div class="max-w-[650px] text-[16px] text-muted dark:text-[#a3a3a3]">
        <p class="mb-5">
          I'm Samuel, a software engineer working mostly
          with JavaScript and TypeScript.
        </p>

        <p class="mb-5">
          I like building simple interfaces, developer tools,
          and systems that remove repetitive work.
        </p>

        <p class="mb-5">
          Currently interested in web architecture, Linux,
          developer tooling, and distributed systems.
        </p>
      </div>
    </section>
    <USeparator class="h-2" />

    <!-- Projects -->
    <section
      id="projects"
      class="py-20 max-[600px]:py-15"
    >
      <div
        class="relative mb-10 flex items-center gap-3 font-mono text-[14px] before:text-accent before:content-['$']"
      >
        ls projects/
      </div>

      <!-- Project 1 -->
    <USeparator class="h-2" />
      <article
        class="py-6.25"
      >
        <div
          class="flex items-baseline justify-between gap-5 max-[600px]:block"
        >
          <div class="font-mono text-xl">
            01. IGEPSA
          </div>

          <div
            class="flex items-center justify-center gap-2 font-mono text-[12px] text-muted max-[600px]:mt-[5px] max-[600px]:block"
          >
          <ULink as="button">
            <CodeXml size=18 />
          </ULink>
          <ULink as="button">
            <ExternalLink size=18 />
          </ULink>
          </div>
        </div>

        <p
          class="my-2.5 mb-3.5 max-w-150 text-sm text-muted"
        >
          Platform for automating administrative tasks
          and managing institutional data.
        </p>

        <div class="font-mono text-[12px] text-[#525252]">
          Next.js · TypeScript · SQLite · Drizzle
        </div>
      </article>

      <!-- Project 2 -->
    <USeparator class="h-4" />
      <article
        class="py-6.25"
      >
        <div
          class="flex items-baseline justify-between gap-5 max-[600px]:block"
        >
          <div class="font-mono text-xl">
            02. Inspecteurs
          </div>

          <div
            class="font-mono text-[12px] text-muted max-[600px]:mt-[5px] max-[600px]:block"
          >
            2026
          </div>
        </div>

        <p
          class="my-2.5 mb-3.5 max-w-150 text-sm text-muted"
        >
          Web interface for exploring, filtering and
          visualizing structured Excel data.
        </p>

        <div class="font-mono text-[12px] text-[#525252]">
          React · TypeScript · XLSX
        </div>
      </article>

      <!-- Project 3 -->
    <USeparator class="h-4" />
      <article
        class="py-6.25"
      >
        <div
          class="flex items-baseline justify-between gap-5 max-[600px]:block"
        >
          <div class="font-mono text-xl">
            03. Another Project
          </div>

          <div
            class="font-mono text-[12px] text-muted max-[600px]:mt-1.25 max-[600px]:block"
          >
            2025
          </div>
        </div>

        <p
          class="my-2.5 mb-3.5 max-w-150 text-sm text-muted"
        >
          Short description of what this project does
          and why it exists.
        </p>

        <div class="font-mono text-[12px] text-[#525252]">
          Next.js · PostgreSQL · tRPC
        </div>
      </article>
    </section>

    <!-- Contact -->
    <USeparator class="h-4" />
    <section
      id="contact"
      class="py-20 max-[600px]:py-15"
    >
      <div
        class="relative mb-10 flex items-center gap-3 font-mono text-[14px] before:text-accent before:content-['$']"
      >
        echo $CONTACT
      </div>

      <div class="max-w-162.5 text-base text-muted dark:text-[#a3a3a3]">
        <p class="mb-5">
          Have a project or want to talk?
        </p>

        <p class="mb-5">
          <a
            href="mailto:hello@example.com"
            class="transition-colors hover:text-accent"
          >
            hello@example.com ↗
          </a>
        </p>
      </div>
    </section>

    <!-- Footer -->
    <USeparator class="h-4" />
    <footer
      class="flex justify-between py-7.5 font-mono text-[12px] text-muted max-[600px]:block"
    >
      <span>samuel@nandi ~</span>

      <span class="max-[600px]:mt-2 max-[600px]:block">
        © 2026
      </span>
    </footer>
  </div>
</template>
