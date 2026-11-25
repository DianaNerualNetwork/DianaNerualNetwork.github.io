# Bing Xiong's academic homepage

Live site: https://diananerualnetwork.github.io/

A build-free, multi-page HTML/CSS academic website. The layout follows https://hy-li.com/: a shared masthead and author sidebar, a concise homepage, and separate publication and talk pages.

## Pages

- `index.html`: biography, Research Directions, Education & Work Experience, and Academic Service (including IEEE Transactions on Multimedia (2025) under Journal Reviewer).
- `publications/index.html`: Selected Publications (USIGAN and the AAAI 2025 paper), Publications (all five published papers without conference/journal subdivisions), and Preprints (PGLStain). Papers use a bulleted list; all authors use abbreviated names, with only B Xiong in bold; author-role labels and journal ranking/impact-factor annotations are omitted. Existing paper/code links and author markers are preserved.
- `talks/index.html`: invited talks.
- `activities/index.html`: existing news, competition awards, honors, and community activities.
- `assets/css/main.css`: shared typography, responsive layouts, navigation, focus states, and print styles.
- `assets/images/photo.jpg`: user-provided portrait, displayed as a circular photo using CSS.
- `assets/icons/`: locally bundled Font Awesome icons and their license/source attribution.

Each page uses relative links with explicit `index.html` filenames so both a local file preview and GitHub Pages navigation work. The canonical public routes are `/`, `/publications/`, `/talks/`, and `/activities/`.

Existing images remain in their original folders. Education and work experience now use a text-only list; publications no longer display thumbnails. Competition logos appear only on the Activities page. `jemdoc.css` is retained but not loaded. The standalone `CPCL/` project page is unchanged.

## Publication citations

Published entries show the venue in italics followed by the formal publication year, with Paper / Code links inline immediately afterward. Paper labels also cover links whose destination is arXiv. Existing resource URLs are preserved for both selected entries and the complete list. Publication typography follows the reference page: 18px on desktop, 16px below 768px, 1.5 line height, and paper titles at the same size as the citation text.

- USIGAN: *IEEE Transactions on Image Processing*, 2026. [IEEE DOI](https://doi.org/10.1109/TIP.2026.3679993).
- Dual Path Prompted Inversion: *AAAI*, 2025. [AAAI proceedings](https://ojs.aaai.org/index.php/AAAI/article/view/32949).
- UTADC-Net: *IEEE Journal of Biomedical and Health Informatics*, 2026. [IEEE DOI](https://doi.org/10.1109/JBHI.2025.3596007). The article appeared online in 2025; the citation uses its 2026 volume/issue year.
- SynMSE: *Medical Image Analysis*, 2025. [Author's official repository](https://github.com/MIXAILAB/SynMSE).
- AGWNet: *Displays*, 2024. [Publisher](https://www.sciencedirect.com/science/article/abs/pii/S0141938224000945).

PGLStain is listed under Preprints with the supplied title and author order. No publication year, venue, or resource URL has been supplied for that entry.

## Confirmed profile

- First-year Ph.D. student at the National University of Singapore (NUS).
- Ph.D. supervisor: [Prof. Xiaohan Xing](https://hathawayxxh.github.io/).
- M.S., University of Chinese Academy of Sciences (UCAS).
- B.S., Wuhan University of Technology.

The homepage combines these education entries with the existing research assistant and Deepwise internship records, plus a PuzzleLogic Research Intern entry working with Dr. Xiaohan Xing. Dates are displayed exactly as supplied by the user: NUS, `2027.09 – Present`; PuzzleLogic, `2026.07 – Present`. Previous degree years follow the existing education timeline.

## Preview

No Node.js, package installation, or build step is needed. Open `index.html` in a browser, or serve this repository:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then visit `http://127.0.0.1:8000/` on the same machine. Forward port 8000 first when running on a remote host.

Check the homepage and all three navigation destinations at desktop and phone widths. Below 800px the profile moves above the content; text lists and the navigation wrap to fit narrow screens. All navigation works without JavaScript.

Local edits do not change the public GitHub Pages site until committed and pushed to its configured publishing branch. Keep the existing GitHub Pages configuration when publishing.

## Remaining content details

- The sidebar displays `Email` and retains the `mailto:b.xiong@siat.ac.cn` destination; no new NUS email address has been supplied.
- UTADC-Net, SynMSE, and AGWNet currently share the same ScienceDirect paper URL. The Medical Image Analysis news entry also uses that URL. Verify each destination before replacing it.
- UTADC-Net's code link currently points to the SynMSE repository.
- The PPDE URL contains another person's name. Verify the intended profile URL.

The user-provided portrait is preserved unchanged. Its circular display and crop are controlled by `.author-avatar` in the shared stylesheet. All four pages share the same portrait, name, affiliation, and contact icons.
