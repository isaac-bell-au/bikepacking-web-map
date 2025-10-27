# bikepacking-web-map
Code and GPX file repository to generate a simple webmap documenting Caitlin and my bikepacking trip as we go

Access the web map at: https://isaac-bell-au.github.io/bikepacking-web-map/

Log
2025-10-26
- index.html generated entirely from ChatGPT, then debugging with GH Copilot in VS Code
- Got it working in a basic form, first troubleshooting involved:
    - Dealing with the fact that GitHub Pages doesn't allow indexing of directories, so need to have the names of
      the GPX files to map hardcoded somewhere in the root directory, since you can't identify them by searching
      through the /gpx/ folder. The GPX files should already be named in the summaris.json, so the new loadAllGPX()
      function now just loads GPX files listed there.
    - Dealing with "CORS" issue -- i.e. the browser is prevented from looking at local files, so need to run index.html
      from a local server (or something along those lines). Could do this with a local python server, but the Live Preview
      extension within VS Code also works, probably best.

