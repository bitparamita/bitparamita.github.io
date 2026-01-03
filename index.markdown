---
layout: home
---
<h1>
  Hi there! 👋
  <span class="inline-notice">
    (I am <a href="https://www.linkedin.com/in/{{site.linkedin_username }}/"
      target="_blank">#OpenToWork</a> & 
    <a href="/notice-period.html">Notice Period</a>)
  </span>
</h1>

<p> 
I am dedicated and result-oriented Query Surge Certified ETL Tester and ISTQB certified software professional with a passion to reach greater heights by helping organizations achieve their business goals. With over <strong><span id="yearsOfExperience"></span></strong> years of experience in System Testing, primarily in ETL and Database Testing, and collaborating with cross-functional teams to engineer tailored data warehousing solutions. Has a proven expertise in designing, testing and debugging processes, analysing complex data scenarios, with a strong emphasis on meticulous documentation and reporting.
</p>

<style>
    .inline-notice {
        font-size: 0.6em;
        font-weight: bold;
        color: #b30000;
        margin-left: 10px;
        animation: pulse-inline 1.5s infinite;
    }

    .inline-notice a {
        color: #d32f2f;
        text-decoration: none;
        border-bottom: 1px dashed #d32f2f;
    }

    .inline-notice a:hover {
        color: #800000;
        border-bottom-style: solid;
    }

    @keyframes pulse-inline {
        0% { opacity: 0.6; }
        50% { opacity: 1; }
        100% { opacity: 0.6; }
    }

</style>

<script>
    function calculateExperience() {
    const startDate = new Date("2016-08-17");
    const now = new Date();
    const months = (now.getFullYear() - startDate.getFullYear()) * 12 + now.getMonth() - startDate.getMonth();
    const years = Math.floor(months / 12);
    const remMonths = months % 12;
    return `${years}.${remMonths.toString().padStart(2, '0')}`;
    }

    // Update the span with the calculated experience
    document.addEventListener("DOMContentLoaded", () => {
    const experience = calculateExperience();
    const experienceElement = document.getElementById("yearsOfExperience");
    if (experienceElement) {
        experienceElement.innerHTML = experience;
    }
    });
</script>