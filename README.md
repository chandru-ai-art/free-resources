<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Responsive Design Resources</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary: #4f46e5;
            --primary-light: #818cf8;
            --secondary: #10b981;
            --dark: #1f2937;
            --light: #f9fafb;
            --gray: #9ca3af;
            --border-radius: 10px;
            --box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }
        
        body {
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            color: white;
            padding: 2rem 0;
            box-shadow: var(--box-shadow);
            margin-bottom: 2rem;
        }
        
        .header-content {
            text-align: center;
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 0.5rem;
        }
        
        .tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto 1.5rem;
        }
        
        /* Search and Filter */
        .controls {
            background: white;
            padding: 1.5rem;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            margin-bottom: 2rem;
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: space-between;
            align-items: center;
        }
        
        .search-box {
            flex: 1;
            min-width: 250px;
            position: relative;
        }
        
        .search-box input {
            width: 100%;
            padding: 0.8rem 1rem 0.8rem 2.8rem;
            border: 2px solid #e5e7eb;
            border-radius: var(--border-radius);
            font-size: 1rem;
            transition: var(--transition);
        }
        
        .search-box input:focus {
            outline: none;
            border-color: var(--primary);
        }
        
        .search-box i {
            position: absolute;
            left: 1rem;
            top: 50%;
            transform: translateY(-50%);
            color: var(--gray);
        }
        
        .filter-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }
        
        .filter-btn {
            padding: 0.6rem 1.2rem;
            background: #f3f4f6;
            border: none;
            border-radius: 50px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
        }
        
        .filter-btn:hover, .filter-btn.active {
            background: var(--primary);
            color: white;
        }
        
        /* Resources Grid */
        .resources-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        
        .resource-card {
            background: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
            height: 100%;
        }
        
        .resource-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }
        
        .resource-icon {
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            color: white;
        }
        
        .resource-icon.framework {
            background: linear-gradient(135deg, #f59e0b 0%, #d97706 100%);
        }
        
        .resource-icon.css {
            background: linear-gradient(135deg, #3b82f6 0%, #1d4ed8 100%);
        }
        
        .resource-icon.tool {
            background: linear-gradient(135deg, #10b981 0%, #059669 100%);
        }
        
        .resource-icon.image {
            background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%);
        }
        
        .resource-icon.icon {
            background: linear-gradient(135deg, #ef4444 0%, #dc2626 100%);
        }
        
        .resource-icon.font {
            background: linear-gradient(135deg, #ec4899 0%, #db2777 100%);
        }
        
        .resource-content {
            padding: 1.5rem;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }
        
        .resource-content h3 {
            font-size: 1.4rem;
            margin-bottom: 0.5rem;
            color: var(--dark);
        }
        
        .resource-content p {
            color: #6b7280;
            margin-bottom: 1.2rem;
            flex-grow: 1;
        }
        
        .resource-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1.2rem;
        }
        
        .resource-tag {
            background: #e0e7ff;
            color: var(--primary);
            padding: 0.3rem 0.8rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 600;
        }
        
        .resource-link {
            display: inline-block;
            background: var(--primary);
            color: white;
            text-decoration: none;
            padding: 0.7rem 1.2rem;
            border-radius: var(--border-radius);
            font-weight: 600;
            text-align: center;
            transition: var(--transition);
        }
        
        .resource-link:hover {
            background: #4338ca;
        }
        
        /* Tips Section */
        .tips-section {
            background: white;
            border-radius: var(--border-radius);
            padding: 2rem;
            box-shadow: var(--box-shadow);
            margin-bottom: 3rem;
        }
        
        .tips-section h2 {
            text-align: center;
            margin-bottom: 1.5rem;
            color: var(--dark);
        }
        
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        
        .tip-card {
            background: #f9fafb;
            padding: 1.5rem;
            border-radius: var(--border-radius);
            border-left: 4px solid var(--primary);
        }
        
        .tip-card h4 {
            margin-bottom: 0.5rem;
            color: var(--dark);
        }
        
        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 2.5rem 0;
            text-align: center;
        }
        
        .footer-content {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .footer-content p {
            margin-bottom: 1.5rem;
            opacity: 0.9;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-bottom: 1.5rem;
        }
        
        .social-links a {
            color: white;
            font-size: 1.3rem;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            color: var(--primary-light);
        }
        
        .copyright {
            border-top: 1px solid #374151;
            padding-top: 1.5rem;
            font-size: 0.9rem;
            opacity: 0.7;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            .controls {
                flex-direction: column;
                align-items: stretch;
            }
            
            .search-box {
                min-width: 100%;
            }
            
            .resources-container {
                grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            }
        }
        
        @media (max-width: 480px) {
            h1 {
                font-size: 1.8rem;
            }
            
            .tagline {
                font-size: 1rem;
            }
            
            .resources-container {
                grid-template-columns: 1fr;
            }
            
            .tips-grid {
                grid-template-columns: 1fr;
            }
        }
        
        /* Resource Counter */
        .resource-count {
            margin-top: 1rem;
            text-align: center;
            color: #6b7280;
            font-weight: 600;
        }
        
        /* No Results Message */
        .no-results {
            grid-column: 1 / -1;
            text-align: center;
            padding: 3rem;
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <h1>Free Responsive Design Resources</h1>
                <p class="tagline">A curated collection of free tools, frameworks, and resources to help you create beautiful, responsive websites</p>
                <div class="resource-count">
                    <span id="total-resources">0</span> free resources available
                </div>
            </div>
        </div>
    </header>
    
    <main class="container">
        <!-- Search and Filter Controls -->
        <section class="controls">
            <div class="search-box">
                <i class="fas fa-search"></i>
                <input type="text" id="search-input" placeholder="Search resources...">
            </div>
            <div class="filter-buttons">
                <button class="filter-btn active" data-filter="all">All</button>
                <button class="filter-btn" data-filter="framework">Frameworks</button>
                <button class="filter-btn" data-filter="css">CSS Libraries</button>
                <button class="filter-btn" data-filter="tool">Tools</button>
                <button class="filter-btn" data-filter="image">Images</button>
                <button class="filter-btn" data-filter="icon">Icons</button>
                <button class="filter-btn" data-filter="font">Fonts</button>
            </div>
        </section>
        
        <!-- Resources Grid -->
        <section id="resources-grid" class="resources-container">
            <!-- Resources will be loaded here dynamically -->
        </section>
        
        <!-- Tips Section -->
        <section class="tips-section">
            <h2>Responsive Design Tips</h2>
            <div class="tips-grid">
                <div class="tip-card">
                    <h4>Mobile-First Approach</h4>
                    <p>Start designing for mobile devices first, then scale up for larger screens. This ensures your site works well on all devices.</p>
                </div>
                <div class="tip-card">
                    <h4>Use Relative Units</h4>
                    <p>Use percentages, em, rem, and viewport units (vw, vh) instead of fixed pixels for flexible layouts that adapt to different screen sizes.</p>
                </div>
                <div class="tip-card">
                    <h4>Test on Real Devices</h4>
                    <p>Browser dev tools are helpful, but always test your responsive design on actual mobile devices to ensure the best user experience.</p>
                </div>
                <div class="tip-card">
                    <h4>Optimize Images</h4>
                    <p>Use responsive images with srcset attribute and compress images to reduce load times on mobile connections.</p>
                </div>
            </div>
        </section>
    </main>
    
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <p>This is a curated collection of free responsive design resources. All resources are free to use, but check individual licenses for specific usage terms.</p>
                <div class="social-links">
                    <a href="https://github.com/chandru-ai-art"><i class="fab fa-github"></i></a>
                    <a href="https://www.instagram.com/ox_lufi"><i class="fab fa-instagram"></i></a>
                    <a href="https://x.com/Chandru2421"><i class="fab fa-twitter"></i></a>
                    <a href="https://www.linkedin.com/in/chandru-m-5b5036388/"><i class="fab fa-linkedin"></i></a>
                </div>
                <div class="copyright">
                    &copy; 2026 Free Responsive Design Resources. Made with ❤️ for the web development community.
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Resources Data
        const resources = [
            {
                id: 1,
                title: "Bootstrap",
                description: "The most popular CSS framework for developing responsive, mobile-first websites.",
                category: "framework",
                tags: ["CSS", "JavaScript", "Grid System", "Components"],
                link: "https://getbootstrap.com",
                iconClass: "framework"
            },
            {
                id: 2,
                title: "Tailwind CSS",
                description: "A utility-first CSS framework packed with classes for building custom designs.",
                category: "framework",
                tags: ["Utility-First", "Customizable", "Responsive"],
                link: "https://tailwindcss.com",
                iconClass: "framework"
            },
            {
                id: 3,
                title: "Bulma",
                description: "Modern CSS framework based on Flexbox with no JavaScript dependencies.",
                category: "css",
                tags: ["Flexbox", "Modern", "Lightweight"],
                link: "https://bulma.io",
                iconClass: "css"
            },
            {
                id: 4,
                title: "Font Awesome",
                description: "The world's most popular icon set and toolkit with thousands of free icons.",
                category: "icon",
                tags: ["Icons", "Vector", "Scalable"],
                link: "https://fontawesome.com",
                iconClass: "icon"
            },
            {
                id: 5,
                title: "Google Fonts",
                description: "Free, open-source fonts optimized for the web with easy integration.",
                category: "font",
                tags: ["Typography", "Web Fonts", "Free"],
                link: "https://fonts.google.com",
                iconClass: "font"
            },
            {
                id: 6,
                title: "Unsplash",
                description: "Beautiful, free images and photos you can download and use for any project.",
                category: "image",
                tags: ["Photos", "Stock", "High-Quality"],
                link: "https://unsplash.com",
                iconClass: "image"
            },
            {
                id: 7,
                title: "Pexels",
                description: "Free stock photos and videos shared by talented creators worldwide.",
                category: "image",
                tags: ["Photos", "Videos", "Royalty-Free"],
                link: "https://pexels.com",
                iconClass: "image"
            },
            {
                id: 8,
                title: "CSS Grid Generator",
                description: "Interactive tool to visually create CSS grid layouts with real-time code output.",
                category: "tool",
                tags: ["Generator", "CSS Grid", "Interactive"],
                link: "https://cssgrid-generator.netlify.app",
                iconClass: "tool"
            },
            {
                id: 9,
                title: "Flexbox Froggy",
                description: "A fun game to learn and practice CSS Flexbox through interactive challenges.",
                category: "tool",
                tags: ["Learning", "Game", "Flexbox"],
                link: "https://flexboxfroggy.com",
                iconClass: "tool"
            },
            {
                id: 10,
                title: "FontPair",
                description: "Helps you pair Google Fonts together for beautiful, readable typography.",
                category: "tool",
                tags: ["Typography", "Font Pairing", "Design"],
                link: "https://fontpair.co",
                iconClass: "tool"
            },
            {
                id: 11,
                title: "Feather Icons",
                description: "Simply beautiful open source icons with a clean and consistent style.",
                category: "icon",
                tags: ["Minimal", "SVG", "Open Source"],
                link: "https://feathericons.com",
                iconClass: "icon"
            },
            {
                id: 12,
                title: "CSS-Tricks Guide to Flexbox",
                description: "Complete guide to CSS Flexbox with examples, diagrams, and use cases.",
                category: "css",
                tags: ["Guide", "Flexbox", "Tutorial"],
                link: "https://css-tricks.com/snippets/css/a-guide-to-flexbox",
                iconClass: "css"
            }
        ];

        // DOM Elements
        const resourcesGrid = document.getElementById('resources-grid');
        const filterButtons = document.querySelectorAll('.filter-btn');
        const searchInput = document.getElementById('search-input');
        const totalResources = document.getElementById('total-resources');

        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            // Display all resources initially
            displayResources(resources);
            
            // Set total resources count
            totalResources.textContent = resources.length;
            
            // Add event listeners to filter buttons
            filterButtons.forEach(button => {
                button.addEventListener('click', function() {
                    // Remove active class from all buttons
                    filterButtons.forEach(btn => btn.classList.remove('active'));
                    
                    // Add active class to clicked button
                    this.classList.add('active');
                    
                    // Filter resources
                    const filter = this.getAttribute('data-filter');
                    filterResources(filter, searchInput.value);
                });
            });
            
            // Add event listener to search input
            searchInput.addEventListener('input', function() {
                const activeFilter = document.querySelector('.filter-btn.active').getAttribute('data-filter');
                filterResources(activeFilter, this.value);
            });
        });

        // Function to display resources
        function displayResources(resourcesToDisplay) {
            resourcesGrid.innerHTML = '';
            
            if (resourcesToDisplay.length === 0) {
                resourcesGrid.innerHTML = `
                    <div class="no-results">
                        <h3>No resources found</h3>
                        <p>Try adjusting your search or filter criteria</p>
                    </div>
                `;
                return;
            }
            
            resourcesToDisplay.forEach(resource => {
                const resourceCard = document.createElement('div');
                resourceCard.className = 'resource-card';
                resourceCard.setAttribute('data-category', resource.category);
                
                // Create tags HTML
                let tagsHTML = '';
                resource.tags.forEach(tag => {
                    tagsHTML += `<span class="resource-tag">${tag}</span>`;
                });
                
                resourceCard.innerHTML = `
                    <div class="resource-icon ${resource.iconClass}">
                        <i class="fas fa-${getIconForCategory(resource.category)}"></i>
                    </div>
                    <div class="resource-content">
                        <h3>${resource.title}</h3>
                        <p>${resource.description}</p>
                        <div class="resource-tags">
                            ${tagsHTML}
                        </div>
                        <a href="${resource.link}" target="_blank" class="resource-link">
                            Visit Resource <i class="fas fa-external-link-alt"></i>
                        </a>
                    </div>
                `;
                
                resourcesGrid.appendChild(resourceCard);
            });
        }

        // Function to filter resources
        function filterResources(category, searchTerm) {
            let filteredResources = resources;
            
            // Filter by category
            if (category !== 'all') {
                filteredResources = filteredResources.filter(resource => resource.category === category);
            }
            
            // Filter by search term
            if (searchTerm) {
                const term = searchTerm.toLowerCase();
                filteredResources = filteredResources.filter(resource => 
                    resource.title.toLowerCase().includes(term) || 
                    resource.description.toLowerCase().includes(term) ||
                    resource.tags.some(tag => tag.toLowerCase().includes(term))
                );
            }
            
            // Display filtered resources
            displayResources(filteredResources);
            
            // Update count
            totalResources.textContent = filteredResources.length;
        }

        // Helper function to get appropriate icon for each category
        function getIconForCategory(category) {
            switch(category) {
                case 'framework': return 'layer-group';
                case 'css': return 'css3';
                case 'tool': return 'tools';
                case 'image': return 'images';
                case 'icon': return 'icons';
                case 'font': return 'font';
                default: return 'link';
            }
        }

        // Initialize with all resources
        displayResources(resources);
    </script>
</body>

</html>
