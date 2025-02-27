---
layout: default
title: Uttam Singh - Portfolio # Add this to control page title
---

<div class="header-container">
    <img src="{{ '/assets/profile.jpg' | relative_url }}" alt="Uttam Singh" class="profile-img">
    <div class="header-text">
        <h1>Uttam Singh</h1>
        <p>Master's Candidate in Computer Science @ NYU</p>
        <div class="contact-links">
            <a href="mailto:us2193@nyu.edu" class="email-link">📧 Email</a>
            <a href="https://linkedin.com/in/uttam-singh-nyu" target="_blank" class="linkedin-link">💼 LinkedIn</a>
            <a href="https://github.com/lord-fourth0107" class="github-link">👨💻 GitHub</a>
            <a href="https://scholar.google.com/citations?user=MxGGafQAAAAJ&hl=en" class="scholar-link">📚 Google Scholar</a>
        </div>
    </div>
</div>

<style>
.header-container {
    display: flex;
    align-items: center;
    margin-bottom: 2rem;
    gap: 2rem;
}

.profile-img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
}

.contact-links a {
    margin-right: 1.2rem;
    text-decoration: none;
    color: #2E86C1;
}
</style>

---