---
layout: page
title: About Me
permalink: /about/
hide: true
---

<style>
.about-container {
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px;
}

.profile-section {
    display: flex;
    align-items: flex-start;
    gap: 30px;
    margin-bottom: 40px;
}

.profile-image {
    width: 500px;
    height: 500px;
    border-radius: 10px;
    object-fit: cover;
}

.profile-content {
    flex: 1;
    min-width: 0; /* Prevents text overflow issues */
}

.profile-description {
    line-height: 1.6;
    margin-bottom: 25px;
    font-size: 1.3rem;
}

.cv-button {
    display: inline-flex;
    align-items: center;
    padding: 12px 24px;
    background-color: #2196F3;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    transition: background-color 0.3s ease;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.cv-button:hover {
    background-color: #1976D2;
    transform: translateY(-1px);
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.cv-button-icon {
    margin-right: 8px;
    font-size: 1.2em;
}

/* Tablet Devices */
@media (max-width: 768px) {
    .profile-section {
        flex-direction: column;
        align-items: center;
        text-align: center;
        gap: 20px;
    }
    
    .profile-image {
        width: 270px;
        height: 270px;
    }

    .profile-content {
        width: 100%;
    }
}

/* Mobile Devices */
@media (max-width: 480px) {
    .about-container {
        padding: 15px;
    }

    .profile-image {
        width: 270px;
        height: 270px;
    }

    .cv-button {
        padding: 10px 20px;
        width: 100%;
        justify-content: center;
    }
}
</style>

<div class="about-container">
    <div class="profile-section">
        <img src="/assets/img/me.png" alt="Paweł Gągała" class="profile-image">
        <div class="profile-content">
            <div class="profile-description">
                <p>As a seasoned backend developer with over 10 years of experience,
                I thrive on crafting elegant solutions to complex challenges with awesome people. 
                My journey in software development began in 2013, 
                and I've maintained a fundamental belief: in technology, standing still means falling behind.
                This mindset drives me to continuously evolve, staying current with emerging trends and best practices in our ever-changing field.</p>

                <p>Beyond the world of code, I maintain a holistic approach to personal development.
                Exercising with my own body weight is my preferred way to maintain physical fitness, helping me achieve a healthy balance between mental and physical well-being. 
                In my downtime, you'll find me immersed in science fiction and fantasy literature. 
                I value productivity and purposeful living, making the most of every opportunity for growth and learning.</p>
            </div>

            <a href="/assets/Pawel_Gagala_CV.pdf" class="cv-button" target="_blank">
                <span class="cv-button-icon">📄</span>
                <span class="cv-button-text">Download CV</span>
            </a>
        </div>
    </div>

</div>