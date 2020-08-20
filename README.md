NixOS Configuration for JupyterHub
---

TODO:

- [ ] Include [jupyterlab-git][jupyterlab-git] to easily clone workshop repository
  - [ ] Need to add jupyterlab-git as nixpkg
- [ ] Use [tmpauthenticator][tmpauthenticator] to give anyone that logs in access
  - [ ] Need to add tmpauthenticator as nixpkg
- [ ] Figure out how to "deploy" this somewhere in the cloud

A NixOS configuration which starts Jupyter Hub on port 8000. It uses
[tmpauthenticator][tmpauthenticator] to automatically log users in to the hub.
This is useful for my workshops because people tend to roll in without signing
up and therefore they don't have accounts. I wouldn't recommend this setup for
general use.

Python packages included:

- pandas and numpy
- scikit-learn
- pytorch and torchvision
- matplotlib
- pillow

[tmpauthenticator]: https://github.com/jupyterhub/tmpauthenticator
[jupyterlab-git]: https://github.com/jupyterlab/jupyterlab-git
