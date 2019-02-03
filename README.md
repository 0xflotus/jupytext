# A JupyterLab extension for Jupytext

This extension adds a few [Jupytext](https://github.com/mwouts/jupytext) commands to the command palette. Use these to select the desired ipynb/text pairing for your notebook.

![Jupytext commands](jupytext_commands.png)

## Installation

Please [install Jupytext](https://github.com/mwouts/jupytext/blob/master/README.md#installation) first. Make sure Jupyter is configured to use Jupytext's contents manager. Then, install the extension with:

:construction:

At this stage the extension is not functional. Thus we have not distributed it yet, so

```bash
jupyter labextension install jupyterlab-jupytext
```

won't work.

# How to develop this extension

We started developping the extension following the [xkcd extension tutorial](https://jupyterlab.readthedocs.io/en/stable/developer/xkcd_extension_tutorial.html). Follow the instructions there to create a conda environment in which you will be able to develop the extension. In that environment, install JupyterLab's plugin manager, and the extension with
```bash
jlpm install
jupyter labextension install . --no-build
```

Then, in another shell on the same environment, start JupyterLab:
```bash
jupyter lab --watch
```

Finally, make changes to the extension and rebuild it (in the first shell) with:
```bash
jlpm run build
```

Refresh the JupyterLab interface and see your changes in action.
