# reMarkable Templates Repository

This repository is a collection of LaTeX-based PDF templates designed for reMarkable devices (reMarkable Paper Pro, 1, and 2), aimed at enhancing productivity, organization, and note-taking. Each template is crafted to fit the reMarkable Paper Pro screen (1404x1872 pixels, ~4.97x6.63 inches at 226 PPI) and is organized into subfolders based on use case (e.g., meetings, planning, journaling). The templates are professional, customizable, and optimized for handwritten notes.

## Repository Structure

The templates are organized into the following subfolders, each containing specific templates for different purposes:

- **meeting-notes/**
  - **Meeting_Notes_Template.tex**: A two-page template for streamlined meeting note-taking.
    - **Page 1**: Meeting Details (Date, Subject, Location), Key Takeaways (3 lines), and Notes (10 lines for extensive note-taking).
    - **Page 2**: Action Items (table for tasks, assignees, and due dates) and Quadrant Notes (Eisenhower Matrix with large 0.9in boxes for prioritization).
    - **Features**: Compact 10pt font, customizable logo, large Quadrant Notes boxes for ample writing space.
    - **Use Case**: Ideal for professionals capturing meeting discussions, action items, and task prioritization.

- **daily-planner/**
  - (Placeholder for future templates) Templates for daily task management, goal setting, and scheduling.
  - Planned templates: Daily Planner with hyperlinked dates, to-do lists, and habit trackers.

- **journal/**
  - (Placeholder for future templates) Templates for personal reflection, journaling, and wellness tracking.
  - Planned templates: Daily Journal with sections for reflections, today-I-learned, and behavior tracking.

- **specialized/**
  - (Placeholder for future templates) Templates for niche use cases like fitness tracking, budgeting, or student planning.
  - Planned templates: Fitness Tracker, Budget Planner, and Student Assignment Planner.

## Prerequisites

To use these templates, you’ll need:
- A LaTeX editor (e.g., [Overleaf](https://www.overleaf.com)) or a local LaTeX installation (e.g., TeX Live with `latexmk`).
- A reMarkable device (Paper Pro, 1, or 2).
- Tools for transferring PDFs to your reMarkable (e.g., reMarkable desktop/mobile app, [rM2 Tool](https://github.com/reMarkable/rm2-tool), or [RCU](https://github.com/reMarkable/rcu)).
- (Optional) A graphics editor (e.g., Photoshop, GIMP, or Canva) for adding custom logos.

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/remarkable-templates.git
   cd remarkable-templates
   ```

2. **Navigate to a Subfolder**:
   ```bash
   cd meeting-notes
   ```
   Replace `meeting-notes` with the desired subfolder (e.g., `daily-planner`, `journal`, `specialized`).

3. **Compile the LaTeX File**:
   - Open the `.tex` file (e.g., `Meeting_Notes_Template.tex`) in a LaTeX editor like Overleaf, or use a local LaTeX installation.
   - Compile the file to generate a PDF:
     ```bash
     latexmk -pdf Meeting_Notes_Template.tex
     ```
   - The output PDF is sized for the reMarkable Paper Pro (4.97x6.63 inches at 226 PPI).

4. **Add a Custom Logo (Optional)**:
   - For templates supporting logos (e.g., Meeting Notes), uncomment the `\includegraphics` line in the `.tex` file:
     ```latex
     \includegraphics[width=0.25\textwidth]{logo.png}
     ```
   - Replace `logo.png` with the path to your logo file (PNG format recommended).
   - Adjust the width (e.g., `0.25\textwidth`) for proper scaling.
   - Recompile the LaTeX file to include the logo.

5. **Import to reMarkable**:
   - Transfer the compiled PDF to your reMarkable device using:
     - The reMarkable desktop or mobile app (drag and drop the PDF).
     - Tools like rM2 Tool or RCU:
       ```bash
       rm2-tool upload Meeting_Notes_Template.pdf
       ```
   - Organize the PDF in a folder (e.g., “Meeting Notes”) on your reMarkable for easy access.

## Usage

- **Meeting Notes Template** (`meeting-notes/Meeting_Notes_Template.tex`):
  - **Page 1**: Fill in Meeting Details (Date, Subject, Location), Key Takeaways (3 lines), and Notes (10 lines).
  - **Page 2**: List tasks, assignees, and due dates in Action Items; use Quadrant Notes for task prioritization (Eisenhower Matrix).
  - **Tips**: Write directly on the PDF using reMarkable’s Marker. Duplicate the PDF for multiple meetings (e.g., create a 756-page version by repeating the layout).

- **Other Templates**:
  - Refer to subfolder-specific READMEs (if available) for detailed usage instructions once additional templates are added.
  - General tip: Favorite or tag templates on your reMarkable for quick access.

## Creating Additional Templates

To create new templates or extend existing ones:
- Duplicate a `.tex` file in the appropriate subfolder and modify its content.
- Ensure the PDF dimensions remain 1404x1872 pixels (4.97x6.63 inches at 226 PPI).
- Use tools like [ReCalendar](https://recalendar.app) or [Hyperpaper.me](https://hyperpaper.me) for inspiration or to generate custom layouts.
- Add new templates to relevant subfolders (e.g., `daily-planner`, `journal`) and update this README.

## Limitations

- **PDF Constraints**: These templates do not support handwriting-to-text conversion, layer functionality, or typed text (Type Folio) on reMarkable.
- **Exporting**: For proper display when emailing or exporting, pair PDFs with SVG versions (create using a graphics editor and import with rM2 Tool or RCU).
- **Personal Use**: Templates are for personal use only. Do not distribute or modify for commercial purposes without permission.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/new-template`).
3. Add or modify `.tex` files in the appropriate subfolder (e.g., `meeting-notes`, `daily-planner`).
4. Update this README to reflect new templates or subfolders.
5. Submit a pull request with a description of your changes.

Ensure all templates are compatible with reMarkable devices (1404x1872 pixels) and use packages from `texlive-full` or `texlive-fonts-extra`.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. Templates are for personal use only; commercial distribution is prohibited.

## Acknowledgments

- Inspired by community templates from [TabletTemplates](https://tablettemplates.com), [Hyperpaper.me](https://hyperpaper.me), and Reddit’s reMarkable community.
- Built with LaTeX for compatibility with [reMarkable Methods](https://remarkable.com) and third-party tools like rM2 Tool and RCU.

For questions or support, open an issue in this repository or contact the maintainer at [your-email@example.com].