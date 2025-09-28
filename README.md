<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Voice Echoes | The Professional Voice of Alex Rivers</title>
    <!-- Basic SEO -->
    <meta name="description" content="Professional voice-over artist specializing in commercials, narration, and character work. Hear my demos and request a quote.">
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure Tailwind to use Inter font -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Custom scrollbar styling for a darker aesthetic */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0f172a; /* Darker blue-gray */
        }
        ::-webkit-scrollbar-thumb {
            background: #14b8a6; /* Teal */
            border-radius: 4px;
        }
    </style>
    <!-- Font Awesome for Icons (Socials, Play button) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-gray-900 text-white min-h-screen">

    <!-- Sticky Header/Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900/90 backdrop-blur-sm shadow-xl">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <a href="#hero" class="text-2xl font-extrabold tracking-widest text-teal-400">VOICE ECHOES</a>
            <nav class="space-x-4">
                <a href="#demos" class="text-gray-300 hover:text-teal-400 transition duration-300 font-medium">Demos</a>
                <a href="#services" class="text-gray-300 hover:text-teal-400 transition duration-300 font-medium hidden sm:inline">Services</a>
                <a href="#about" class="text-gray-300 hover:text-teal-400 transition duration-300 font-medium hidden md:inline">About</a>
                <a href="#contact" class="text-gray-300 hover:text-teal-400 transition duration-300 font-medium">Contact</a>
            </nav>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section id="hero" class="relative h-screen flex items-center justify-center text-center overflow-hidden py-16">
            <!-- Background Visual/Gradient -->
            <div class="absolute inset-0 bg-gradient-to-br from-gray-900 via-gray-800 to-gray-900 opacity-90"></div>
            
            <div class="relative z-10 p-6 max-w-4xl mx-auto">
                <h1 class="text-5xl sm:text-7xl font-black mb-4 tracking-tight">
                    The Voice <span class="text-teal-400">That Connects</span>
                </h1>
                <p class="text-xl sm:text-2xl text-gray-300 mb-8 max-w-xl mx-auto leading-relaxed">
                    Hello, I'm Alex Rivers. Whether you need an authoritative corporate narration or a friendly, conversational commercial, I bring your script to life with professional clarity.
                </p>
                <a href="#demos" class="inline-block px-10 py-4 text-xl font-semibold bg-teal-600 text-white rounded-full shadow-lg hover:bg-teal-500 transition duration-300 transform hover:scale-105">
                    Listen to My Demos
                </a>
            </div>
        </section>

        <!-- Demos/Samples Section -->
        <section id="demos" class="py-16 md:py-24 bg-gray-800">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-4xl font-bold text-center mb-12 text-teal-400">Voice-Over Samples</h2>
                
                <!-- Category Tabs -->
                <div class="flex justify-center space-x-4 mb-8">
                    <button data-category="commercial" class="category-btn px-4 py-2 rounded-full text-sm font-medium bg-teal-600 text-white shadow-md hover:bg-teal-500 transition duration-300">Commercial</button>
                    <button data-category="narration" class="category-btn px-4 py-2 rounded-full text-sm font-medium bg-gray-700 text-gray-300 shadow-md hover:bg-gray-600 transition duration-300">Narration</button>
                    <button data-category="character" class="category-btn px-4 py-2 rounded-full text-sm font-medium bg-gray-700 text-gray-300 shadow-md hover:bg-gray-600 transition duration-300">Character</button>
                </div>

                <!-- Custom Audio Player UI -->
                <div class="max-w-xl mx-auto bg-gray-900 p-6 rounded-xl shadow-2xl border-2 border-teal-500/50 mb-10">
                    <p id="current-track-title" class="text-center text-lg font-semibold mb-3 text-teal-300">Select a demo to play...</p>
                    <div class="flex items-center justify-center space-x-6">
                        <button id="play-pause-btn" class="text-3xl text-teal-400 hover:text-teal-300 transition duration-200" disabled>
                            <i class="fas fa-play"></i>
                        </button>
                        <!-- Basic progress bar placeholder -->
                        <div class="w-2/3 h-2 bg-gray-700 rounded-full overflow-hidden">
                            <div id="progress-bar" class="h-full bg-teal-600" style="width: 0%;"></div>
                        </div>
                    </div>
                    <!-- Hidden native audio element -->
                    <audio id="audio-player" src="" preload="auto"></audio>
                </div>

                <!-- Demos List -->
                <div id="demos-list" class="space-y-4 max-w-3xl mx-auto">
                    <!-- Audio samples will be rendered here by JavaScript -->
                </div>

            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="py-16 md:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-4xl font-bold text-center mb-12 text-teal-400">Services Offered</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                    
                    <!-- Service 1: Commercials -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-xl hover:shadow-teal-500/30 transition duration-300 border-t-4 border-teal-600">
                        <i class="fas fa-bullhorn text-3xl text-teal-400 mb-3"></i>
                        <h3 class="text-xl font-bold mb-2">Commercials</h3>
                        <p class="text-gray-400 text-sm">Radio, TV, and web ads. Delivering energetic, persuasive, or relaxed tones to match your brand identity perfectly.</p>
                    </div>

                    <!-- Service 2: E-Learning & Corporate -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-xl hover:shadow-teal-500/30 transition duration-300 border-t-4 border-teal-600">
                        <i class="fas fa-graduation-cap text-3xl text-teal-400 mb-3"></i>
                        <h3 class="text-xl font-bold mb-2">E-Learning & Corporate</h3>
                        <p class="text-gray-400 text-sm">Clear, trustworthy, and engaging narration for training modules, explainer videos, and corporate presentations.</p>
                    </div>

                    <!-- Service 3: Audiobooks & Narration -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-xl hover:shadow-teal-500/30 transition duration-300 border-t-4 border-teal-600">
                        <i class="fas fa-book-reader text-3xl text-teal-400 mb-3"></i>
                        <h3 class="text-xl font-bold mb-2">Audiobooks & Narration</h3>
                        <p class="text-gray-400 text-sm">Narrating long-form content, documentary voice-over, and full audiobook production with emotional depth.</p>
                    </div>

                    <!-- Service 4: Dubbing & IVR -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-xl hover:shadow-teal-500/30 transition duration-300 border-t-4 border-teal-600">
                        <i class="fas fa-phone-volume text-3xl text-teal-400 mb-3"></i>
                        <h3 class="text-xl font-bold mb-2">Dubbing & IVR</h3>
                        <p class="text-gray-400 text-sm">Accurate lip-sync dubbing for media and professional, clear voicing for phone systems and hold messages.</p>
                    </div>

                </div>
            </div>
        </section>

        <!-- About Me Section -->
        <section id="about" class="py-16 bg-gray-900">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-4xl">
                <h2 class="text-4xl font-bold text-center mb-12 text-teal-400">About Alex Rivers</h2>
                
                <div class="flex flex-col md:flex-row items-start md:space-x-12 bg-gray-800 p-8 rounded-xl shadow-2xl border border-gray-700">
                    <div class="w-full md:w-1/3 mb-6 md:mb-0 flex flex-col items-center">
                        <img src="https://placehold.co/300x300/1f2937/ffffff?text=Alex+Rivers" 
                             alt="Portrait of the voice-over artist"
                             class="rounded-full w-48 h-48 object-cover border-4 border-teal-500 shadow-2xl">
                        <div class="mt-4 text-center">
                            <h3 class="text-xl font-semibold">The Voice Style</h3>
                            <ul class="text-gray-400 text-sm mt-1 list-none p-0 space-y-1">
                                <li>Tone: Warm, Clear, Authoritative</li>
                                <li>Age Range: 30s-40s</li>
                                <li>Specialty: Empathetic & Corporate</li>
                            </ul>
                        </div>
                    </div>
                    <div class="w-full md:w-2/3 text-gray-300 text-center md:text-left">
                        <p class="mb-4 text-lg font-medium text-teal-300">
                            "A decade of experience turning words into immersive auditory experiences."
                        </p>
                        <p class="mb-4">
                            With a professional studio setup (Neumann TLM 103 and Pro Tools) and a background in broadcast journalism, my voice is reliable, consistent, and easy to direct. I pride myself on providing clean, edited files and a quick turnaround time, typically within 24 hours.
                        </p>
                        <p>
                            I believe the success of a project lies in capturing the *right* tone—the one that truly connects with the listener. From high-energy retail spots to complex medical narrations, I ensure every read is executed with precision and care. Let's make some noise together.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonials Section -->
        <section id="testimonials" class="py-16 bg-gray-800">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-4xl font-bold text-center mb-12 text-teal-400">Rave Reviews</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                    
                    <!-- Testimonial 1 -->
                    <div class="bg-gray-900 p-6 rounded-xl shadow-lg border border-gray-700">
                        <i class="fas fa-quote-left text-2xl text-teal-500 mb-3"></i>
                        <p class="text-gray-300 italic mb-4 text-sm">"Alex's voice instantly elevated our corporate video. Professional, fast, and required zero revisions. Highly recommend for any business project."</p>
                        <p class="font-semibold text-teal-400">Sarah K.</p>
                        <p class="text-xs text-gray-500">Marketing Director, Tech Solutions Inc.</p>
                    </div>

                    <!-- Testimonial 2 -->
                    <div class="bg-gray-900 p-6 rounded-xl shadow-lg border border-gray-700">
                        <i class="fas fa-quote-left text-2xl text-teal-500 mb-3"></i>
                        <p class="text-gray-300 italic mb-4 text-sm">"The emotional range he brought to the audiobook was incredible. He made every character distinct and the story truly came alive."</p>
                        <p class="font-semibold text-teal-400">James P.</p>
                        <p class="text-xs text-gray-500">Indie Author</p>
                    </div>

                    <!-- Testimonial 3 -->
                    <div class="bg-gray-900 p-6 rounded-xl shadow-lg border border-gray-700">
                        <i class="fas fa-quote-left text-2xl text-teal-500 mb-3"></i>
                        <p class="text-gray-300 italic mb-4 text-sm">"We needed a quick turnaround for a radio spot, and Alex delivered a broadcast-ready file in under 4 hours. Exceptional quality and service."</p>
                        <p class="font-semibold text-teal-400">Media Agency Team</p>
                        <p class="text-xs text-gray-500">Apex Advertising</p>
                    </div>

                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-16 md:py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-2xl">
                <h2 class="text-4xl font-bold text-center mb-12 text-teal-400">Request a Quote</h2>
                <div class="bg-gray-800 p-8 rounded-xl shadow-2xl border border-gray-700">
                    <p class="text-center text-gray-300 mb-6">Tell me about your project, budget, and timeline. I'll respond with a custom quote immediately.</p>
                    
                    <form id="contact-form" action="#" method="POST" class="space-y-4">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-300 mb-1">Your Name</label>
                            <input type="text" id="name" name="name" placeholder="Contact Name"
                                   class="w-full px-4 py-3 rounded-lg bg-gray-900 border border-gray-600 focus:border-teal-500 focus:ring-teal-500 text-white transition duration-200" required>
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-300 mb-1">Project Email</label>
                            <input type="email" id="email" name="email" placeholder="project@company.com"
                                   class="w-full px-4 py-3 rounded-lg bg-gray-900 border border-gray-600 focus:border-teal-500 focus:ring-teal-500 text-white transition duration-200" required>
                        </div>
                        <div>
                            <label for="details" class="block text-sm font-medium text-gray-300 mb-1">Project Details & Usage</label>
                            <textarea id="details" name="details" rows="5" placeholder="Type of project (commercial, e-learning), word count, usage (internet only, broadcast), and deadline."
                                      class="w-full px-4 py-3 rounded-lg bg-gray-900 border border-gray-600 focus:border-teal-500 focus:ring-teal-500 text-white transition duration-200" required></textarea>
                        </div>
                        <button type="submit" 
                                class="w-full py-3 bg-teal-600 text-white font-semibold rounded-lg shadow-md hover:bg-teal-500 transition duration-300 transform hover:scale-[1.01] focus:outline-none focus:ring-2 focus:ring-teal-500 focus:ring-offset-2 focus:ring-offset-gray-900">
                            Get a Free Quote
                        </button>
                    </form>

                    <div id="contact-message" class="mt-4 hidden text-center p-3 rounded-lg bg-green-900/50 text-green-300">
                        <!-- Message box for form submission feedback -->
                    </div>

                    <p class="text-center text-gray-400 mt-6">
                        Or email directly: 
                        <a href="mailto:alex@voiceechoes.com" class="text-teal-400 hover:text-teal-300 font-medium">alex@voiceechoes.com</a>
                    </p>
                </div>
                
                <!-- Social Media Links -->
                <div class="flex justify-center space-x-6 mt-8">
                    <a href="#" target="_blank" class="text-2xl text-gray-400 hover:text-teal-400 transition duration-300"><i class="fab fa-twitter"></i></a>
                    <a href="#" target="_blank" class="text-2xl text-gray-400 hover:text-teal-400 transition duration-300"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" target="_blank" class="text-2xl text-gray-400 hover:text-teal-400 transition duration-300"><i class="fab fa-soundcloud"></i></a>
                    <a href="#" target="_blank" class="text-2xl text-gray-400 hover:text-teal-400 transition duration-300"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 py-8">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 text-center text-gray-400 text-sm">
            <p>&copy; 2024 Voice Echoes by Alex Rivers. All rights reserved.</p>
        </div>
    </footer>

    <!-- JavaScript for Player and Interactivity -->
    <script>
        // --- DATA: VOICE SAMPLES ---
        const samples = [
            { id: 1, title: "High-Energy Retail Ad", category: "commercial", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" },
            { id: 2, title: "Warm, Conversational PSA", category: "commercial", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3" },
            { id: 3, title: "Corporate Explainer Video", category: "narration", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-3.mp3" },
            { id: 4, title: "Documentary Voice-Over (Serious)", category: "narration", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-4.mp3" },
            { id: 5, title: "Wacky Cartoon Character", category: "character", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-5.mp3" },
            { id: 6, title: "Fantasy Game NPC (Deep)", category: "character", src: "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-6.mp3" }
        ];

        // --- DOM Elements ---
        const audioPlayer = document.getElementById('audio-player');
        const playPauseBtn = document.getElementById('play-pause-btn');
        const progressBar = document.getElementById('progress-bar');
        const currentTrackTitle = document.getElementById('current-track-title');
        const demosList = document.getElementById('demos-list');
        const categoryBtns = document.querySelectorAll('.category-btn');
        const contactForm = document.getElementById('contact-form');
        const contactMessage = document.getElementById('contact-message');

        let currentTrack = null;
        let isPlaying = false;

        // --- FUNCTIONS ---

        // Renders the list of samples for the currently selected category
        const renderSamples = (category) => {
            demosList.innerHTML = '';
            const filteredSamples = samples.filter(sample => sample.category === category);

            filteredSamples.forEach(sample => {
                const button = document.createElement('button');
                button.className = 'w-full flex items-center justify-between p-4 bg-gray-900 rounded-lg border border-gray-700 hover:bg-gray-700 transition duration-200 shadow-md';
                button.innerHTML = `
                    <span class="text-left font-medium text-gray-200">${sample.title}</span>
                    <i class="fas fa-play text-teal-400 track-icon" data-id="${sample.id}"></i>
                `;
                button.setAttribute('data-id', sample.id);
                button.addEventListener('click', () => loadAndPlayTrack(sample));
                demosList.appendChild(button);
            });
            updateTrackIcons();
        };

        // Loads a track into the audio player and starts playback
        const loadAndPlayTrack = (sample) => {
            // Pause any currently playing track
            if (currentTrack && currentTrack.id !== sample.id && !audioPlayer.paused) {
                audioPlayer.pause();
            }
            
            // If the same track is clicked and it's playing, pause it
            if (currentTrack && currentTrack.id === sample.id) {
                if (isPlaying) {
                    audioPlayer.pause();
                } else {
                    audioPlayer.play();
                }
                return;
            }

            // Load new track
            currentTrack = sample;
            audioPlayer.src = sample.src;
            currentTrackTitle.textContent = sample.title;
            
            audioPlayer.load(); // Ensure the new source is loaded
            audioPlayer.play().then(() => {
                isPlaying = true;
                playPauseBtn.disabled = false;
            }).catch(error => {
                console.error("Playback failed: ", error);
                // Fallback for failed play attempts (e.g., due to user interaction policy)
                isPlaying = false;
                playPauseBtn.disabled = true;
                currentTrackTitle.textContent = `Error playing "${sample.title}"`;
            });
            updatePlayerUI();
            updateTrackIcons();
        };

        // Updates the play/pause button icon
        const updatePlayerUI = () => {
            playPauseBtn.innerHTML = isPlaying ? '<i class="fas fa-pause"></i>' : '<i class="fas fa-play"></i>';
        };
        
        // Updates the icon next to the track in the list
        const updateTrackIcons = () => {
            document.querySelectorAll('.track-icon').forEach(icon => {
                const trackId = parseInt(icon.getAttribute('data-id'));
                if (currentTrack && trackId === currentTrack.id) {
                    icon.className = `text-teal-400 track-icon fas ${isPlaying ? 'fa-pause' : 'fa-play'}`;
                } else {
                    icon.className = 'text-teal-400 track-icon fas fa-play';
                }
            });
        };

        // --- EVENT LISTENERS ---

        // Category button click handler
        categoryBtns.forEach(button => {
            button.addEventListener('click', function() {
                const category = this.getAttribute('data-category');
                
                // Update active button styles
                categoryBtns.forEach(btn => {
                    btn.classList.remove('bg-teal-600', 'text-white');
                    btn.classList.add('bg-gray-700', 'text-gray-300');
                });
                this.classList.remove('bg-gray-700', 'text-gray-300');
                this.classList.add('bg-teal-600', 'text-white');

                renderSamples(category);
            });
        });
        
        // Main player play/pause button handler
        playPauseBtn.addEventListener('click', () => {
            if (audioPlayer.paused || audioPlayer.ended) {
                audioPlayer.play();
                isPlaying = true;
            } else {
                audioPlayer.pause();
                isPlaying = false;
            }
            updatePlayerUI();
            updateTrackIcons();
        });

        // Audio events for UI updates
        audioPlayer.addEventListener('play', () => {
            isPlaying = true;
            updatePlayerUI();
            updateTrackIcons();
        });

        audioPlayer.addEventListener('pause', () => {
            isPlaying = false;
            updatePlayerUI();
            updateTrackIcons();
        });
        
        audioPlayer.addEventListener('ended', () => {
            isPlaying = false;
            progressBar.style.width = '0%';
            updatePlayerUI();
            updateTrackIcons();
        });

        // Update progress bar
        audioPlayer.addEventListener('timeupdate', () => {
            const percentage = (audioPlayer.currentTime / audioPlayer.duration) * 100;
            progressBar.style.width = `${percentage}%`;
        });
        
        // Smooth scrolling for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Contact Form Submission (Simulated)
        contactForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Simple validation check
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            
            if (name && email) {
                // Simulate form success
                contactMessage.classList.remove('hidden', 'bg-red-900/50', 'text-red-300');
                contactMessage.classList.add('bg-green-900/50', 'text-green-300');
                contactMessage.textContent = "Thank you for your inquiry! Alex will get back to you within 24 hours.";
                
                // Reset form fields
                contactForm.reset();
                
                // Hide message after a few seconds
                setTimeout(() => {
                    contactMessage.classList.add('hidden');
                }, 5000);
            } else {
                // Show error message
                contactMessage.classList.remove('hidden', 'bg-green-900/50', 'text-green-300');
                contactMessage.classList.add('bg-red-900/50', 'text-red-300');
                contactMessage.textContent = "Please fill out all required fields.";
            }
        });

        // --- INITIALIZATION ---
        // Render the default category (Commercial) on load
        window.onload = () => {
            document.querySelector('.category-btn[data-category="commercial"]').click();
        };
    </script>

</body>
</html>

