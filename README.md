
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="theme-color" content="#0b0b12">
    <title>VibeMatch | Find Your Vibe</title>

   <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/lucide@latest"></script>
</head>

<body>

    <aside class="sidebar">
        <a href="#" class="logo">
            <span class="logo-icon">V</span>
            VibeMatch
        </a>

        <p class="menu-label">MENU</p>

        <nav>
            <a href="#" class="nav-link active" data-page="discover">
                <i data-lucide="compass"></i> Discover
            </a>
            <a href="#" class="nav-link" data-page="matches">
                <i data-lucide="users"></i> Connections
            </a>
            <a href="#" class="nav-link" data-page="quiz">
                <i data-lucide="brain"></i> Personality Quiz
            </a>
            <a href="#" class="nav-link" data-page="messages">
                <i data-lucide="message-circle"></i> Messages
            </a>
            <a href="#" class="nav-link" data-page="profile">
                <i data-lucide="user"></i> My Profile
            </a>
        </nav>

        <div class="sidebar-bottom">
            <div class="user-mini">
                <div class="avatar">U</div>
                <div>
                    <strong>Demo User</strong>
                    <small>Free account</small>
                </div>
            </div>
        </div>
    </aside>

    <main class="main-content">

        <header class="topbar">
            <div>
                <h2 id="page-title">Discover</h2>
                <p>Explore people who share your interests.</p>
            </div>

            <div class="topbar-actions">
                <button class="icon-btn" id="theme-toggle" aria-label="Toggle theme">
                    <i data-lucide="sun"></i>
                </button>
                <div class="avatar">U</div>
            </div>
        </header>

        <section id="discover-page" class="page active">

            <div class="welcome-banner">
                <div>
                    <span class="eyebrow">YOUR COMMUNITY STARTS HERE</span>
                    <h1>Find Your <span>Vibe.</span><br>Discover Your People.</h1>
                    <p>Meet people who share your hobbies, music and interests.</p>
                </div>
                <div class="banner-decoration">✦</div>
            </div>

            <div class="section-heading">
                <div>
                    <h2>People you might connect with</h2>
                    <p>Explore these fictional demo profiles.</p>
                </div>
                <span class="online-indicator">● DEMO MODE</span>
            </div>

            <div class="filter-bar">
                <button class="filter active" data-filter="All">All</button>
                <button class="filter" data-filter="Music">Music</button>
                <button class="filter" data-filter="Technology">Technology</button>
                <button class="filter" data-filter="Travel">Travel</button>
                <button class="filter" data-filter="Gaming">Gaming</button>
            </div>

            <div class="profile-grid" id="profile-grid"></div>

        </section>

        <section id="matches-page" class="page">
            <div class="section-heading">
                <div>
                    <h2>Your connections</h2>
                    <p>People whose profiles you have liked.</p>
                </div>
            </div>
            <div class="profile-grid" id="matches-grid"></div>
        </section>

        <section id="quiz-page" class="page">
            <div class="quiz-container">
                <span class="eyebrow">GET TO KNOW YOURSELF</span>
                <h1>Discover Your <span>Personality</span></h1>
                <p>Answer a few fun questions about your interests.</p>

                <div id="quiz-content">
                    <div class="quiz-question">
                        <h2>What do you enjoy most?</h2>
                        <div class="quiz-options">
                            <button class="quiz-option">Listening to music</button>
                            <button class="quiz-option">Building technology</button>
                            <button class="quiz-option">Exploring new places</button>
                            <button class="quiz-option">Playing games</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="messages-page" class="page">
            <div class="section-heading">
                <div>
                    <h2>Messages</h2>
                    <p>Demo messaging interface.</p>
                </div>
            </div>
            <div class="empty-state">
                <i data-lucide="message-circle"></i>
                <h2>No conversations yet</h2>
                <p>This prototype does not send real messages.</p>
            </div>
        </section>

        <section id="profile-page" class="page">
            <div class="section-heading">
                <div>
                    <h2>My Profile</h2>
                    <p>Manage your demo profile.</p>
                </div>
            </div>
            <div class="profile-form">
                <label>Display name</label>
                <input type="text" id="user-name" value="Demo User">

                <label>About me</label>
                <textarea id="user-bio" rows="4">I enjoy music, technology and exploring new ideas.</textarea>

                <label>Interests</label>
                <input type="text" id="user-interests" value="Music, Technology, Gaming">

                <button class="primary-btn" id="save-profile">Save Profile</button>
                <p id="save-status"></p>
            </div>
        </section>

        <footer>
            <p>© 2026 VibeMatch. A social discovery demo.</p>
            <p>Privacy first. Respect everyone.</p>
        </footer>

    </main>

    <script src="javascript/data.js"></script>
<script src="javascript/app.js"></script>
    <script>
        lucide.createIcons();
    </script>
</body>
</html>
