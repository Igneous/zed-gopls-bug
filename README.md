# Hi.
This is a demo repo for recreating a situation where gopls offers no suggestions under a nested directory structure with zed-git

If you cd into this directory and open the root of this repo from zed (`Zed .`), gopls should offer no suggestions when editing go.project/main.go.

However, if you cd directly into the go.project directory and launch zed from there, gopls works as expected. (In my case).

Running `go work init && go work use go.project` from the project root works around the issue.
