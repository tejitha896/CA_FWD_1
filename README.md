📄 HTML (index.html)
Description:
This file structures a personal portfolio website that showcases:

✅ A navigation bar with anchor links to different sections (Home, About, Projects, Contact).

✅ A hero section with a brief intro and social icons.

✅ An About Me section describing skills and technologies.

✅ A Projects section highlighting completed work and internships.

✅ A Contact form to allow users to reach out.

✅ A footer with name, social links, and copyright.

The HTML also prepares the structure for:

*A responsive image gallery (via .item class and data-category attributes).

*Button controls (data-filter) for JavaScript to apply dynamic filtering.

*Compatibility with external CSS (style.css) and JavaScript (script.js) files.



📜 JavaScript (script.js)
Description:
This file adds interactivity and logic to the portfolio, focusing on two main functionalities:

1. 🔍 Filterable Gallery
-->Dynamically filters .item elements based on the data-filter value.
-->Updates button UI to show the active filter.
-->Shows or hides images based on their data-category attribute.

2. 🖼️ Image Viewer (Lightbox)
Opens a full-screen viewer when an image is clicked.

Supports:
-->Next/Prev navigation (buttons + arrow keys).
-->Close viewer (button or Escape key).
-->Only includes currently visible images based on the active filter.
-->Dynamically updates the viewer content and navigation with currentIndex.



🎨 CSS (style.css)
Description:
This file styles a filterable image gallery with a lightbox viewer and ensures a clean, modern, and responsive user interface.

🧱 General Styles:
-->Sets a soft background color (#ff9997c4) for the entire page.
-->Applies zero margin and padding to reset browser defaults.
-->Uses Algerian font for the header to give it a stylized look.

🧭 Header Section:
Centers and colors the .header text in a green shade.
-->Adds vertical spacing with padding.

🔘 Filter Buttons:
-->Flex container centers buttons horizontally.
-->button style includes rounded corners, padding, and hover-ready cursors.
-->active-button highlights the currently selected category with a teal background and white text.

🖼️ Gallery Grid:
-->The gallery class uses CSS Grid for a responsive layout, adjusting automatically with auto-fit and minmax.
-->Gap and padding make the layout clean and breathable.
Images inside .item:
    -->Are sized uniformly (250x250 px).
    -->Have hover effects (zoom and rotation).
    -->Include smooth transitions for a polished effect.

🔍 Image Viewer / Lightbox:
#image-viewer is a fixed full-screen overlay with a dark semi-transparent background.
#full-image scales to fit within 90% width and 80% height.
Close (#close-btn) and navigation buttons (#nav-buttons) are clearly positioned and styled:
    -->Big, clickable, and user-friendly.
    -->Styled white to contrast against the dark overlay.
    -->Rounded and padded for visual clarity.
