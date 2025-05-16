# week-7-assignment-biochemistry-web-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced Medical Biochemistry Lab</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <img src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MTIgNTEyIj48cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptLTM5LjYgMzc5LjRoLTcyLjdWMTI0LjloNzIuN3YyNjIuNXptMTUyLjEgMEgyNjguOFYxMjQuOWg3Mi43djI2Mi41eiIgZmlsbD0id2hpdGUiLz48L3N2Zz4=" alt="Microscope" class="lab-equipment microscope">
        <img src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MTIgNTEyIj48cGF0aCBkPSJNNDQ4IDI1NkMwIDI1NiAwIDI1NiAwIDI1NnMyNTYgMCAyNTYgMjU2LTI1NiAyNTYtMjU2LTI1NnptLTMyIDBjMCAxMjMuNy0xMDAuMyAyMjQtMjI0IDIyNFMzMiAzNzkuNyAzMiAyNTYgMTMyLjMgMzIgMjU2IDMyczIyNCAxMDAuMyAyMjQgMjI0eiIgZmlsbD0id2hpdGUiLz48L3N2Zz4=" alt="Flask" class="lab-equipment flask">
        <div class="header-content">
            <h1>Advanced Medical Biochemistry Lab</h1>
            <p>Precision Diagnostics for Better Healthcare</p>
        </div>
    </header>

    <nav>
        <ul class="nav-links">
            <li><a href="#services">Our Services</a></li>
            <li><a href="#tests">Diagnostic Tests</a></li>
            <li><a href="#research">Research</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <div class="container">
        <section id="services">
            <h2>Our Laboratory Services</h2>
            <div class="services">
                <div class="service-card">
                    <div class="service-img">
                        <img src="https://images.unsplash.com/photo-1581093450021-4a7360e9a6a6?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Clinical Chemistry">
                    </div>
                    <div class="service-content">
                        <h3>Clinical Chemistry</h3>
                        <p>Comprehensive metabolic panels, enzyme studies, and therapeutic drug monitoring with state-of-the-art analyzers.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-img">
                        <img src="https://images.unsplash.com/photo-1579684385127-1ef15d508118?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Molecular Diagnostics">
                    </div>
                    <div class="service-content">
                        <h3>Molecular Diagnostics</h3>
                        <p>PCR-based testing, genetic screening, and pharmacogenomics for personalized medicine approaches.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-img">
                        <img src="https://images.unsplash.com/photo-1581094271901-8022df4466f9?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Toxicology">
                    </div>
                    <div class="service-content">
                        <h3>Toxicology</h3>
                        <p>Drug screening, heavy metal testing, and comprehensive toxicology panels using GC/MS and LC/MS technology.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>

        <section class="preferences-panel">
            <h2>User Preferences</h2>
            <div class="form-group">
                <label for="theme">Select Theme:</label>
                <select id="theme">
                    <option value="light">Light Mode</option>
                    <option value="dark">Dark Mode</option>
                </select>
            </div>
            <div class="form-group">
                <label for="animation">Enable Animations:</label>
                <select id="animation">
                    <option value="enabled">Enabled</option>
                    <option value="disabled">Disabled</option>
                </select>
            </div>
            <button id="savePrefs" class="btn">Save Preferences</button>
        </section>

        <div class="test-tube">
            <div class="bubbles" id="bubbles-container"></div>
        </div>
    </div>

    <footer>
        <p>&copy; 2023 Advanced Medical Biochemistry Lab. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
#css
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    --light-color: #ecf0f1;
    --dark-color: #2c3e50;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: #f5f7fa;
    color: var(--dark-color);
    line-height: 1.6;
}

header {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: white;
    padding: 2rem 0;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    position: relative;
    overflow: hidden;
}

.lab-equipment {
    position: absolute;
    opacity: 0.1;
    z-index: 0;
}

.microscope {
    top: 20%;
    left: 10%;
    width: 100px;
    height: 100px;
    animation: float 6s ease-in-out infinite;
}

.flask {
    bottom: 15%;
    right: 10%;
    width: 80px;
    height: 80px;
    animation: float 5s ease-in-out infinite reverse;
}

@keyframes float {
    0%, 100% {
        transform: translateY(0) rotate(0deg);
    }
    50% {
        transform: translateY(-20px) rotate(5deg);
    }
}

.header-content {
    position: relative;
    z-index: 1;
}

h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    transition: all 0.3s ease;
}

h1:hover {
    transform: scale(1.05);
    text-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
}

nav {
    background-color: white;
    padding: 1rem;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.nav-links {
    display: flex;
    justify-content: center;
    list-style: none;
}

.nav-links li {
    margin: 0 1.5rem;
}

.nav-links a {
    text-decoration: none;
    color: var(--dark-color);
    font-weight: 600;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    transition: all 0.3s ease;
    position: relative;
}

.nav-links a::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 0;
    height: 2px;
    background-color: var(--accent-color);
    transition: width 0.3s ease;
}

.nav-links a:hover {
    color: var(--accent-color);
}

.nav-links a:hover::after {
    width: 100%;
}

.container {
    max-width: 1200px;
    margin: 2rem auto;
    padding: 0 2rem;
}

.services {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin: 3rem 0;
}

.service-card {
    background-color: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: all 0.3s ease;
    transform: translateY(0);
}

.service-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
}

.service-img {
    height: 200px;
    overflow: hidden;
}

.service-img img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease;
}

.service-card:hover .service-img img {
    transform: scale(1.1);
}

.service-content {
    padding: 1.5rem;
}

.service-content h3 {
    color: var(--primary-color);
    margin-bottom: 1rem;
}

.btn {
    display: inline-block;
    background-color: var(--secondary-color);
    color: white;
    padding: 0.8rem 1.5rem;
    border-radius: 4px;
    text-decoration: none;
    font-weight: 600;
    border: none;
    cursor: pointer;
    transition: all 0.3s ease;
    transform: scale(1);
}

.btn:hover {
    background-color: var(--accent-color);
    transform: scale(1.05);
}

.btn:active {
    transform: scale(0.98);
}

.preferences-panel {
    background-color: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    margin: 3rem 0;
    animation: fadeIn 0.5s ease-out;
}

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.form-group {
    margin-bottom: 1.5rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 600;
}

select, input {
    width: 100%;
    padding: 0.8rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 1rem;
    transition: border-color 0.3s ease;
}

select:focus, input:focus {
    outline: none;
    border-color: var(--secondary-color);
    box-shadow: 0 0 0 2px rgba(52, 152, 219, 0.2);
}

footer {
    background-color: var(--primary-color);
    color: white;
    text-align: center;
    padding: 2rem 0;
    margin-top: 3rem;
}

.test-tube {
    width: 50px;
    height: 100px;
    background: linear-gradient(to bottom, #3498db, #2ecc71);
    border-radius: 0 0 10px 10px;
    position: relative;
    margin: 2rem auto;
    animation: bubble 4s ease-in-out infinite;
}

@keyframes bubble {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-10px);
    }
}

.test-tube::before {
    content: '';
    position: absolute;
    top: -5px;
    left: 0;
    width: 100%;
    height: 10px;
    background-color: rgba(255, 255, 255, 0.5);
    border-radius: 50%;
}

.bubbles {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 80%;
}

.bubble {
    position: absolute;
    background-color: rgba(255, 255, 255, 0.4);
    border-radius: 50%;
    animation: rise 3s infinite;
}

@keyframes rise {
    0% {
        transform: translateY(0) scale(0.3);
        opacity: 0;
    }
    50% {
        opacity: 0.8;
    }
    100% {
        transform: translateY(-80px) scale(1);
        opacity: 0;
    }
}

/* Dark mode styles */
body.dark-mode {
    background-color: #1a1a1a;
    color: #f0f0f0;
}

body.dark-mode nav {
    background-color: #2c3e50;
}

body.dark-mode .nav-links a {
    color: #f0f0f0;
}

body.dark-mode .service-card,
body.dark-mode .preferences-panel {
    background-color: #2c3e50;
    color: #f0f0f0;
}

body.dark-mode .service-content h3 {
    color: #3498db;
}

body.dark-mode select,
body.dark-mode input {
    background-color: #34495e;
    color: #f0f0f0;
    border-color: #7f8c8d;
}

/* Add fadeOut animation dynamically */
@keyframes fadeOut {
    from { opacity: 1; transform: translateY(0); }
    to { opacity: 0; transform: translateY(20px); }
}
#jss
// DOM Elements
const themeSelect = document.getElementById('theme');
const animationSelect = document.getElementById('animation');
const savePrefsBtn = document.getElementById('savePrefs');
const bubblesContainer = document.getElementById('bubbles-container');

// Load user preferences from localStorage
function loadPreferences() {
    const preferences = JSON.parse(localStorage.getItem('labPreferences')) || {
        theme: 'light',
        animations: 'enabled'
    };

    themeSelect.value = preferences.theme;
    animationSelect.value = preferences.animations;

    applyPreferences(preferences);
}

// Apply user preferences
function applyPreferences(prefs) {
    // Apply theme
    if (prefs.theme === 'dark') {
        document.body.classList.add('dark-mode');
    } else {
        document.body.classList.remove('dark-mode');
    }

    // Apply animations
    if (prefs.animations === 'disabled') {
        document.querySelectorAll('*').forEach(el => {
            // Check if the element has an animation style
            const hasAnimation = getComputedStyle(el).animationName !== 'none';
            const hasTransition = getComputedStyle(el).transitionProperty !== 'none';

            if (hasAnimation) {
                el.style.animationPlayState = 'paused';
            }
             if (hasTransition) {
                 el.style.transition = 'none';
             }
        });
        // Also stop the bubble generation interval if running
        if (window.bubbleInterval) {
            clearInterval(window.bubbleInterval);
            window.bubbleInterval = null;
            bubblesContainer.innerHTML = ''; // Clear bubbles
        }
    } else {
        document.querySelectorAll('*').forEach(el => {
             // Check if the element had an animation style before
             const hasAnimation = getComputedStyle(el).animationName !== 'none';
             const hasTransition = getComputedStyle(el).transitionProperty !== 'none';

             if (hasAnimation) {
                 el.style.animationPlayState = 'running';
             }
              if (hasTransition && el.dataset.originalTransition !== undefined) {
                  el.style.transition = el.dataset.originalTransition; // Restore original transition
              } else if (hasTransition) {
                   el.style.transition = ''; // Clear if no original saved
              }
        });
         // Restart bubble generation if not running
         if (!window.bubbleInterval) {
            createBubbles();
            window.bubbleInterval = setInterval(createBubbles, 3000);
         }
    }
}

// Save preferences to localStorage
function savePreferences() {
    const preferences = {
        theme: themeSelect.value,
        animations: animationSelect.value
    };

    localStorage.setItem('labPreferences', JSON.stringify(preferences));
    applyPreferences(preferences);

    // Show confirmation animation
    if (preferences.animations === 'enabled') {
        const confirmation = document.createElement('div');
        confirmation.textContent = 'Preferences Saved!';
        confirmation.style.position = 'fixed';
        confirmation.style.bottom = '20px';
        confirmation.style.right = '20px';
        confirmation.style.backgroundColor = '#2ecc71';
        confirmation.style.color = 'white';
        confirmation.style.padding = '1rem 2rem';
        confirmation.style.borderRadius = '4px';
        confirmation.style.boxShadow = '0 4px 6px rgba(0, 0, 0, 0.1)';
        confirmation.style.zIndex = '1000'; // Ensure it's on top
        confirmation.style.animation = 'fadeIn 0.5s, fadeOut 0.5s 2.5s forwards';
        document.body.appendChild(confirmation);

        setTimeout(() => {
            confirmation.remove();
        }, 3000);
    }
}

// Create bubbles animation
function createBubbles() {
    // Clear existing bubbles
    bubblesContainer.innerHTML = '';

    // Check if animations are enabled
    const preferences = JSON.parse(localStorage.getItem('labPreferences')) || {
        animations: 'enabled'
    };

    if (preferences.animations === 'disabled') {
        return;
    }

    // Create bubbles
    for (let i = 0; i < 10; i++) {
        const bubble = document.createElement('div');
        bubble.classList.add('bubble');

        // Random properties
        const size = Math.random() * 10 + 5;
        const left = Math.random() * 100;
        const delay = Math.random() * 3;
        const duration = Math.random() * 2 + 2;

        bubble.style.width = `${size}px`;
        bubble.style.height = `${size}px`;
        bubble.style.left = `${left}%`;
        bubble.style.animationDelay = `${delay}s`;
        bubble.style.animationDuration = `${duration}s`;

        bubblesContainer.appendChild(bubble);
    }
}

// Event Listeners
savePrefsBtn.addEventListener('click', savePreferences);

// Initialize
document.addEventListener('DOMContentLoaded', () => {
    loadPreferences();
    // Start bubble generation only if animations are enabled on load
    const preferences = JSON.parse(localStorage.getItem('labPreferences')) || {
        animations: 'enabled'
    };
    if (preferences.animations === 'enabled') {
         createBubbles();
         window.bubbleInterval = setInterval(createBubbles, 3000);
    } else {
        window.bubbleInterval = null; // Ensure interval is null if disabled
    }
});

// Store original transitions when disabling animations
document.addEventListener('DOMContentLoaded', () => {
    const preferences = JSON.parse(localStorage.getItem('labPreferences')) || {
        animations: 'enabled'
    };
    if (preferences.animations === 'enabled') {
        document.querySelectorAll('*').forEach(el => {
            const transition = getComputedStyle(el).transition;
            if (transition !== 'all 0s ease 0s') { // Don't save default transition
                el.dataset.originalTransition = transition;
            }
        });
    }
});
