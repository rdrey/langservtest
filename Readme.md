Reproducing https://github.com/microsoft/python-language-server/issues/1137

Steps:

- `pip install -r requirements.txt`
- Update `.vscode/settings.json` to point at python in venv

Full log:
```
Starting Microsoft Python language server.
[Info  - 4:38:23 PM] GetCurrentSearchPaths /home/rainer/.virtualenvs/langeservtest/bin/python 
[Info  - 4:38:23 PM] Python search paths:
[Info  - 4:38:23 PM]     /home/rainer/.virtualenvs/langeservtest/lib/python2.7
[Info  - 4:38:23 PM]     /home/rainer/.virtualenvs/langeservtest/lib/python2.7/lib-dynload
[Info  - 4:38:23 PM]     /usr/lib/python2.7
[Info  - 4:38:23 PM]     /usr/lib/python2.7/plat-x86_64-linux-gnu
[Info  - 4:38:23 PM]     /usr/lib/python2.7/lib-tk
[Info  - 4:38:23 PM]     /home/rainer/.virtualenvs/langeservtest/local/lib/python2.7/site-packages
[Info  - 4:38:23 PM]     /home/rainer/work/langservtest/langservtest
[Info  - 4:38:23 PM]     /home/rainer/.virtualenvs/langeservtest/lib/python2.7/site-packages
[Info  - 4:38:23 PM] Configuration search paths:
[Info  - 4:38:23 PM] Microsoft Python Language Server version 0.2.86.0
[Info  - 4:38:23 PM] Initializing for /home/rainer/.virtualenvs/langeservtest/bin/python
Opening document file:///home/rainer/work/langservtest/langservtest/langservtest/test.py
Analysis of langservtest.langservtest.test(User) queued
Import:  langservtest.langservtest.errors /home/rainer/work/langservtest/langservtest/langservtest/errors/__init__.py 
Analysis of langservtest.langservtest.errors(User) queued
Import:  langservtest.langservtest.noerror /home/rainer/work/langservtest/langservtest/langservtest/noerror/__init__.py 
Analysis version 3 of 2 entries has started.
Analysis of langservtest.langservtest.errors(User) completed in 11.3395 ms.
Analysis of langservtest.langservtest.test(User) completed in 12.3166 ms.
Missing keys: langservtest.langservtest.noerror(/home/rainer/work/langservtest/langservtest/langservtest/noerror/__init__.py)
Analysis version 3 of 2 entries has been completed in 36.7452 ms.
Analysis of langservtest.langservtest.noerror(User) queued
Analysis version 5 of 2 entries has started.
Analysis of langservtest.langservtest.noerror(User) completed in 0.1714 ms.
Analysis of langservtest.langservtest.test(User) completed in 1.851 ms.
Analysis version 5 of 2 entries has been completed in 2.295 ms.
```
