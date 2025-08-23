---
layout: page
permalink: /teaching/
title: Teaching
description: This page provides a selected list of courses I have taught. Please refer to my CV for an exhaustive list of courses for which I have served as a TA.
nav: true
nav_order: 3
---

<head>
  <!-- Font Awesome for icons -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">
<style>
  /* Toggle icon style */
  .toggle-icon {
    font-size: 18px;
    margin-right: 10px;
    transition: transform 0.3s;
  }

  /* Badge style */
  .badge {
    display: inline-block;
    padding: 0.25em 0.5em;
    border-radius: 0.25rem;
    font-size: 0.85em;
    font-weight: 500;
    background-color: var(--global-theme-color);
    color: var(--global-theme-text);
    text-align: center;
    line-height: 1.2;
  }

  /* Toggleable course content */
  .toggle-content {
    display: none;
    margin-top: 10px;
  }

  /* Smaller, aesthetic per-card toggle button */
  .toggle-button {
    margin-top: 8px;
    padding: 3px 8px;                 /* smaller padding */
    font-size: 0.75em;                /* smaller text */
    border: 1px solid var(--global-theme-color); /* subtle border */
    border-radius: 0.25rem;
    background-color: transparent;     /* transparent background */
    color: var(--global-theme-color);  /* theme-colored text */
    cursor: pointer;
    transition: all 0.2s;
    align-self: flex-start;
  }

  .toggle-button:hover {
    background-color: var(--global-theme-color); 
    color: var(--global-theme-text);
    opacity: 0.9;
  }

  /* Ensure all cards display correctly */
  .toggle-card {
    display: block; /* visible by default */
  }
</style>
</head>

<h3 class="toggle-header" style="cursor: pointer;">
  <i class="toggle-icon fas fa-chevron-right"></i> University of Maryland
</h3>

<!-- MATH 120 (Elementary Calculus) Summer 24 -->
<div class="card mt-3 toggle-card">
  <div class="p-3">
    <div class="row">
      <div class="col-sm-10">
        <h5 class="card-title">Elementary Calculus</h5>
        <h6 class="card-subtitle font-italic">Instructor, Summer '24</h6>
      </div>
      <div class="col-sm-2 text-sm-right">
        <span class="badge">MATH 120</span>
      </div>
    </div>

    <button class="toggle-button">Show Details</button>

    <div class="row mt-2 toggle-content">
      <div class="col-sm-9">
        <p class="font-weight-light mb-0">
          MATH 120 introduces the basic ideas of differential and integral calculus to non-STEM majors. I delivered lectures and created syllabus, quizzes, exams, and homework for the course.
        </p>
      </div>
      <div class="col-sm-3 d-flex flex-column">
        <a href="/assets/pdf/MATH120-Summer24/Syllabus.pdf">Syllabus</a>
        <a href="/assets/pdf/MATH120-Summer24/Quizzes.pdf">Quizzes</a>
        <a href="/assets/pdf/MATH120-Summer24/Exams.pdf">Exams</a>
      </div>
    </div>
  </div>
</div>

<!-- MATH 740 (Diff. Geo) Spring 24 -->
<div class="card mt-3 toggle-card">
  <div class="p-3">
    <div class="row">
      <div class="col-sm-10">
        <h5 class="card-title">Differential Geometry</h5>
        <h6 class="card-subtitle font-italic">Grader and Guest Lecturer, Spring '24</h6>
      </div>
      <div class="col-sm-2 text-sm-right">
        <span class="badge">MATH 740</span>
      </div>
    </div>

    <button class="toggle-button">Show Details</button>

    <div class="row mt-2 toggle-content">
      <div class="col-sm-9">
        <p class="font-weight-light mb-0">
          MATH 740 is an introduction to differential geometry. I served as the grader for this class, led one problem session, and delivered a lecture on the Hopf-Rinow theorem.
        </p>
      </div>
      <div class="col-sm-3 d-flex flex-column">
        <a href="/assets/pdf/MATH740-Spring24/Sols.pdf">Problem Sets</a>
        <a href="/assets/pdf/MATH740-Spring24/HopfRinow.pdf">Lecture Notes</a>
      </div>
    </div>
  </div>
</div>

<!-- MATH 141 (Calc II) Summer 22 -->
<div class="card mt-3 toggle-card">
  <div class="p-3">
    <div class="row">
      <div class="col-sm-10">
        <h5 class="card-title">Calculus II</h5>
        <h6 class="card-subtitle font-italic">Instructor, Summer '22</h6>
      </div>
      <div class="col-sm-2 text-sm-right">
        <span class="badge">MATH 141</span>
      </div>
    </div>

    <button class="toggle-button">Show Details</button>

    <div class="row mt-2 toggle-content">
      <div class="col-sm-9">
        <p class="font-weight-light mb-0">
          Math 141 is a continuation of MATH 140 (Calculus I) and covers topics such as integration, exponential and logarithmic functions, sequences, and series. I delivered lectures and created syllabus, quizzes, exams, and homework for the course.
        </p>
      </div>
      <div class="col-sm-3 d-flex flex-column">
        <a href="/assets/pdf/MATH141-Summer22/Syllabus.pdf">Syllabus</a>
        <a href="/assets/pdf/MATH141-Summer22/Quizzes.pdf">Quizzes</a>
        <a href="/assets/pdf/MATH141-Summer22/Exams.pdf">Exams</a>
      </div>
    </div>
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function() {

  // Toggle visibility helper
  function toggleVisibility(el) {
    if (el.style.display === "none" || getComputedStyle(el).display === "none") {
      el.style.display = "flex";
      return true;
    } else {
      el.style.display = "none";
      return false;
    }
  }

  // Per-card toggle
  document.querySelectorAll(".toggle-card").forEach(card => {
    const button = card.querySelector(".toggle-button");
    const content = card.querySelector(".toggle-content");

    button.addEventListener("click", () => {
      const visible = toggleVisibility(content);
      button.textContent = visible ? "Hide Details" : "Show Details";
    });
  });

  // Top-level university toggle
  const toggleAllHeader = document.querySelector(".toggle-header");
  const toggleAllIcon = toggleAllHeader.querySelector(".toggle-icon");

  toggleAllHeader.addEventListener("click", e => {
    e.stopPropagation();

    const allCards = document.querySelectorAll(".toggle-card");
    const anyHidden = Array.from(allCards).some(card => getComputedStyle(card).display === "none");

    allCards.forEach(card => {
      card.style.display = anyHidden ? "block" : "none"; // Show/hide all cards
    });

    toggleAllIcon.classList.toggle("fa-chevron-down", anyHidden);
    toggleAllIcon.classList.toggle("fa-chevron-right", !anyHidden);
  });

});
</script>


