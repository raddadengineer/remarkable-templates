# reMarkable Meeting Notes Templates

This repository contains LaTeX-based PDF templates designed for the reMarkable Paper Pro (and compatible with reMarkable 1 and 2), optimized for streamlined meeting note-taking. These templates help users capture key points, action items, and prioritized tasks with a professional, customizable layout.

## Template Overview

The **Meeting Notes Template** is a two-page PDF designed for the reMarkable Paper Pro (1404x1872 pixels, ~4.97x6.63 inches at 226 PPI). It includes:

- **Page 1**: Meeting Details (Date, Subject, Location), Key Takeaways (3 lines), and Notes (10 lines for extensive note-taking).
- **Page 2**: Action Items (table for tasks, assignees, and due dates) and Quadrant Notes (Eisenhower Matrix with large boxes for prioritization).
- **Features**:
  - Compact 10pt font for readability and space efficiency.
  - Customizable with a business logo (PNG format).
  - Large Quadrant Notes boxes (0.9in height) for ample writing space.
  - Structured layout to enhance collaboration and project management.

## Prerequisites

To use these templates, you’ll need:
- A LaTeX editor (e.g., [Overleaf](https://www.overleaf.com)) or a local LaTeX installation (e.g., TeX Live with `latexmk`).
- A reMarkable device (Paper Pro, 1, or 2).
- Tools for transferring PDFs to your reMarkable (e.g., reMarkable desktop/mobile app, [rM2 Tool](https://github.com/reMarkable/rm2-tool), or [RCU](https://github.com/reMarkable/rcu)).
- (Optional) A graphics editor (e.g., Photoshop, GIMP, or Canva) for adding a custom logo.

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/raddadengineer/remarkable-templates.git
   cd meeting-notes
   ```

2. **Compile the LaTeX File**:
   - Open the `.tex` file (e.g., `Meeting_Notes_Template.tex`) in a LaTeX editor like Overleaf, or use a local LaTeX installation.
   - Compile the file to generate a PDF using:
     ```bash
     latexmk -pdf Meeting_Notes_Template.tex
     ```
   - The output PDF is sized for the reMarkable Paper Pro (4.97x6.63 inches at 226 PPI).

3. **Add a Custom Logo (Optional)**:
   - Uncomment the `\includegraphics` line in the `.tex` file:
     ```latex
     \includegraphics[width=0.25\textwidth]{logo.png}
     ```
   - Replace `logo.png` with the path to your logo file (PNG format recommended).
   - Adjust the width (e.g., `0.25\textwidth`) for proper scaling.
   - Recompile the LaTeX file to include the logo in the PDF.

4. **Import to reMarkable**:
   - Transfer the compiled PDF to your reMarkable device using:
     - The reMarkable desktop or mobile app (drag and drop the PDF).
     - Tools like rM2 Tool or RCU for advanced users:
       ```bash
       rm2-tool upload Meeting_Notes_Template.pdf
       ```
   - Organize the PDF in a folder (e.g., “Meeting Notes”) for easy access.

## Usage

- **Page 1**:
  - Fill in Meeting Details (Date, Subject, Location).
  - Use Key Takeaways for 3 concise points.
  - Use the Notes section (10 lines) for detailed meeting notes.
- **Page 2**:
  - List tasks, assignees, and due dates in the Action Items table.
  - Use the Quadrant Notes (Eisenhower Matrix) to prioritize tasks by urgency and importance, with large 0.9in boxes for ample writing space.
- **Tips**:
  - Write directly on the PDF using reMarkable’s Marker for handwritten notes.
  - Duplicate the PDF for multiple meetings (e.g., create a 756-page version by repeating the layout in a LaTeX loop or manually copying pages).
  - Favorite or tag the template on your reMarkable for quick access.

## Creating Additional Templates

To create more templates or extend the page count:
- Duplicate the `\clearpage` and content sections in the `.tex` file for additional pages.
- Use tools like [ReCalendar](https://recalendar.app) or [Hyperpaper.me](https://hyperpaper.me) for inspiration or to generate similar layouts.
- Ensure the PDF dimensions remain 1404x1872 pixels (4.97x6.63 inches at 226 PPI).

## Limitations

- **PDF Constraints**: These templates do not support handwriting-to-text conversion, layer functionality, or typed text (Type Folio) on reMarkable.
- **Exporting**: For proper display when emailing or exporting, pair the PDF with an SVG version (create using a graphics editor and import with rM2 Tool or RCU).
- **Personal Use**: Templates are for personal use only. Do not distribute or modify for commercial purposes without permission.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/new-template`).
3. Add or modify `.tex` files with new template designs.
4. Submit a pull request with a description of your changes.

Please ensure all templates are compatible with reMarkable devices (1404x1872 pixels) and use packages from `texlive-full` or `texlive-fonts-extra`.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. Templates are for personal use only; commercial distribution is prohibited.

## Acknowledgments

- Inspired by community templates from [TabletTemplates](https://tablettemplates.com), [Hyperpaper.me](https://hyperpaper.me), and Reddit’s reMarkable community.
- Built with LaTeX for compatibility with [reMarkable Methods](https://remarkable.com) and third-party tools like rM2 Tool and RCU.

For questions or support, open an issue in this repository or contact the maintainer at [your-email@example.com].
