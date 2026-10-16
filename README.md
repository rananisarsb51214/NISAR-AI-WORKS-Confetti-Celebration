# NISAR-AI-WORKS-Confetti-Celebration
A responsive, customizable confetti celebration web app built with HTML, CSS, and JavaScript. Features AI, Success, Gold, and custom color themes, smooth animations, accessibility support, reduced-motion controls, and lightweight performance optimizations. Created for NISAR AI WORKS.
🎉 NISAR AI WORKS — Confetti Celebration

A modern, responsive confetti celebration web application built with HTML, CSS, and vanilla JavaScript. Create colorful celebrations with customizable themes, animated confetti, and accessibility-friendly controls.

✨ Features

- 🎨 Multiple Themes: AI, Success, Gold, Nisar, and Rainbow.
- 🎊 Confetti Animation: Colorful particles with randomized movement, rotation, and duration.
- 📱 Responsive Design: Works across mobile devices, tablets, and desktops.
- ♿ Accessibility: Keyboard-friendly buttons, visible focus indicators, and screen-reader status announcements.
- 🧘 Reduced Motion: Respects system motion preferences and provides an animation-disable control.
- ⚡ Performance: Particle limits, cleanup of previous celebrations, and lightweight vanilla JavaScript.
- 🔒 Safer Input Handling: Validates confetti colors against an approved allowlist.
- 🌌 Modern UI: Dark navy background, cyan accents, gradient branding, and glass-inspired styling.
- 📦 Standalone Application: No external JavaScript libraries or package installation required.

🛠️ Technology Stack

- HTML5
- CSS3
- Vanilla JavaScript
- CSS animations
- Responsive design principles

🚀 Getting Started

1. Clone the repository

git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_DIRECTORY>

Replace the placeholders with your actual repository URL and directory name.

2. Run the application

Open "index.html" in a modern web browser.

Alternatively, start a local development server:

python -m http.server 8000

Visit:

http://localhost:8000

Stop the server with "Ctrl+C".

🎮 How to Use

1. Open the application in your browser.
2. Select a celebration theme: AI, Success, or Gold.
3. Click Launch Celebration to start the animation.
4. Enable the animation-disable checkbox to stop animations.
5. Enjoy the celebration and launch another whenever you are ready.

🎨 Customization

The application defines its visual theme using CSS custom properties:

:root {
  --bg: #050816;
  --confetti-1: #00d9ff;
  --confetti-2: #007bff;
  --confetti-3: #7c3aed;
  --confetti-4: #22c55e;
}

Approved confetti colors are configured in JavaScript. Add new colors to the allowlist before using them in additional themes.

The particle limit is controlled by:

const MAX_PARTICLES = 120;

Keep the limit in place to reduce excessive DOM creation.

♿ Accessibility

The application includes:

- Keyboard-accessible controls.
- Visible keyboard focus indicators.
- An accessible live status region.
- Support for the "prefers-reduced-motion" system preference.
- A user-controlled animation-disable option.

Accessibility should be verified with real keyboard and screen-reader testing before production deployment.

🔐 Security

- Uses DOM element creation rather than inserting user-controlled HTML.
- Avoids inline JavaScript event-handler attributes.
- Restricts confetti colors to an allowlist.
- Does not require external runtime dependencies.

Production note: The standalone version contains inline CSS and JavaScript. Deployments using a strict Content Security Policy should move these assets into separate files or configure an appropriate nonce/hash policy. Configure additional security headers on the hosting server.

🧪 Testing Checklist

- [ ] Application opens without JavaScript errors.
- [ ] All celebration themes work.
- [ ] Repeated launches do not accumulate particles.
- [ ] Confetti elements are removed after the animation.
- [ ] Reduced-motion preferences are respected.
- [ ] Keyboard navigation and focus indicators work.
- [ ] Layout works on mobile and desktop.
- [ ] Production Content Security Policy is tested.
- [ ] Backup and rollback procedures are verified.

📁 Project Structure

nisar-ai-works-confetti/
├── index.html
├── README.md
└── LICENSE

Create a "LICENSE" file only after selecting the license you intend to use.

🔄 Backup and Rollback

Before replacing an existing version, preserve the original:

cp -p index.html index.html.bak

Check that the backup matches:

cmp -s index.html index.html.bak

If a deployment fails, restore the verified backup:

cp -p index.html.bak index.html

For shared or Git-managed projects, use a reviewed Git commit or revert to avoid overwriting other contributors' changes.

📌 Project Status

Status: Prototype / improved standalone implementation.

Static checks alone do not establish full production readiness. Browser compatibility, accessibility, and deployed security configuration require additional testing.

👨‍💻 Created By

NISAR AI WORKS

Building practical, modern, and accessible AI-inspired web experiences.

---

One Toolbox. Infinite AI Powers. Celebrate every success.https://github.com/rananisarsb51214/NISAR-AI-WORKS-Confetti-Celebration