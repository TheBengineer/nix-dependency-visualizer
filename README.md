# nix-dependency-viewer
A dependency viewer for Nix




# How to use
- Generate a nix dependency graph using:
- ```nix-store -q --graph /nix/store/{root package} > graph.dot```
  - If you don't know the root package, you can graph all dependencies with:
  - ```nix-store -q --find-file /nix/store/*  > graph.dot```
  - You can also look for the root package by running:
  - ```nix show-derivation```  in the root directory.
- Browse to https://thebengineer.github.io/nix-dependency-visualizer/
- Paste the contents of graph.dot into the top textbox on http://localhost:8000/
- Click the "Generate Graph" button


# Running Locally
- Clone Repo
- Start the server using:
- ```python3 server.py```
- Open http://localhost:8000/ in your browser
