# Insight-Center Project Launcher (Version 1.0)

### About

This tool automatically launches an Insight-Center project's development environment:

1. VSCode with the project's target folder
2. Chrome on _localhost:8080_
3. `yarn`
4. `yarn start`

---

### Installation

_Important!_ Edit the path on **line 4** of `launch-ic` and **line 5** of `launch-ic-completion` with the location of your work folder (by default, for Ubuntu based machines, it is set for `~/Documents/ics`).

Install the tool with:

```
sudo ./launch-ic-install
```

A new bash session may be required or `source ~/.bashrc` in order for the changed to be applied.

After instalation, `launch-ic` will be available from everywhere in the terminal as a standalone command.

---

### Usage

To launch the lastly modified project (keep in mind that in loops over all the projects in the target folder), run:

```
launch-ic --last
```

To launch any other project in the folder, run:

```
launch-ic project-name
```

The tool also has completion support, so you can list all the possibilities with `<tab><tab>`, start typing the first letters and `<tab>` to complete.

---

### Removal

If you want to remove the script, run:

```
sudo rm /usr/bin/launch-ic
sudo rm /etc/bash_completion.d/launch-ic-completion
```
