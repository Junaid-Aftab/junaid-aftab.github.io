---
layout: page
permalink: /teaching/
title: Teaching
description: This page provides a selected list of courses I have taught. For a comprehensive list, including courses for which I served as a graduate TA, please refer to my CV.
nav: true
nav_order: 3
---

<head>
  <!-- Include Font Awesome for nice icons -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">
  <style>
    /* Decrease icon size and align it properly *
    #toggle-icon {
      font-size: 18px; /* Decrease the icon size */
      margin-right: 10px; /* Add some space between icon and text */
    }
  </style>
</head>

<style>
  /* Use the global theme variables instead of new ones */
  .badge {
    display: inline-block;
    padding: 0.25em 0.5em;
    border-radius: 0.25rem;
    font-size: 0.85em;
    font-weight: 500;
    background-color: var(--global-theme-color);   /* pick up your theme color */
    color: var(--global-theme-text);               /* pick up your theme text color */
    text-align: center;
    line-height: 1.2;
  }
</style>

<!-- University of Maryland with toggle icon on the left -->
<h3 id="umd" onclick="toggleCourses()" style="cursor: pointer;">
  <i id="toggle-icon" class="fas fa-chevron-down"></i> University of Maryland
</h3>

<div class="card mt-3">
  <div class="p-3">
    <div class="row">
      <div class="col-sm-10">
        <h5 id="Math120" class="card-title">Elementary Calculus</h5>
        <h6 class="card-subtitle font-italic">Instructor, Summer '24</h6>
      </div>
      <div class="col-sm-2 text-sm-right">
      
      <span class="badge">MATH 120</span>
      
      
      
      </div>
    </div>
    <div class="row mt-2">
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
<div class="card mt-3">
  <div class="p-3">
    <div class="row">
      <div class="col-sm-10">
        <h5 id="math740" class="card-title">Differential Geometry</h5>
        <h6 class="card-subtitle font-italic">Grader and Guest Lecturer, Spring '24</h6>
      </div>
      <div class="col-sm-2 text-sm-right">
        <!--
<span class="badge" style="background-color: #4682b4; color: white;">
  MATH 740
</span>
-->
      </div>
    </div>
    <div class="row mt-2">
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
<div class="card mt-3">
  <div class="p-3">
    <div class="row">
      <div class="col-sm-10">
        <h5 id="math141" class="card-title">Calculus II</h5>
        <h6 class="card-subtitle font-italic">Instructor, Summer '22</h6>
      </div>
      <div class="col-sm-2 text-sm-right">
        <!--
<span class="badge" style="background-color: #4682b4; color: white;">
  MATH 141
</span>
-->
      </div>
    </div>
    <div class="row mt-2">
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
  // Function to toggle courses and change icon direction
  function toggleCourses() {
    var courses = document.getElementById("courses");
    var icon = document.getElementById("toggle-icon");

    if (courses.style.display === "none") {
      courses.style.display = "block"; // Show courses
      icon.classList.remove("fa-chevron-right");
      icon.classList.add("fa-chevron-down"); // Change to downward arrow
    } else {
      courses.style.display = "none"; // Hide courses
      icon.classList.remove("fa-chevron-down");
      icon.classList.add("fa-chevron-right"); // Change to right arrow
    }
  }
</script>

