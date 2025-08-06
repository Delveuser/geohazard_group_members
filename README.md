**Delve Underground GeoHazard Team - Interactive Employee Cards**

This project is an interactive HTML component designed to showcase members of the GeoHazard and Geological Engineering Workgroup at Delve Underground. Each team member is displayed as a card containing a headshot, name, and title. Clicking on a card reveals a pop-up containing a detailed biography of the employee.

This HTML is designed to be embedded into the Delve Underground GeoHazard and Geological Engineering Workgroup marketing story map.

**Features:**
- Responsive Grid Layout – Automatically adjusts for different screen sizes.
- Interactive Cards – Click on any employee card to open a pop-up with more detailed info.
- Popup Overlay – Includes an elegant blur effect behind popups to focus user attention.
- Keyboard Accessibility – Press Escape to close the popup.

**File Structure:**
/project-root

│

├── index.html     # Main HTML file (contains all layout and logic)

└── /headshots     # Folder containing all employee headshots

**How to Add a New Team Member:**
Follow these steps to add a new employee card:
1. Upload the Headshot
Place the square format employee headshot in the /headshots/ folder of the GitHub repository.
The recommended image size is around 1800×1800 px for best results.
2. Paste the HTML Snippet
In the index.html file, scroll to the <body> section where existing .employee-card divs are listed.

Note: The vertical position of the new card in the HTML will determine where it appears in the grid. Try to maintain the existing hierarchy:
- "Principal"
- "Associate"
- "Senior Project"
- "Project"
- "Staff"

Example Snippet:
<div class="employee-card" onclick="openPopup('Paste Name Here', 'Paste Employee Bio Here')">
    <img src="https://raw.githubusercontent.com/Delveuser/geohazard_group_members/main/headshots/headshot_image_name.jpg" alt="Paste Name Here">
    <h3>Paste Name Here</h3>
    <p>Paste Position Here</p>
</div>

Replace the placeholders with the correct:
- Full Name
- Job Title
- Bio
- Headshot image name

**Notes & Limitations:**
- This is a static HTML implementation — no backend or dynamic generation.
- Image links assume your repository is public. If private, images may not load externally unless served from a CDN or authenticated repo.
- Some features like keyboard focus trapping and ARIA roles are not yet implemented; consider adding them for full accessibility compliance.
