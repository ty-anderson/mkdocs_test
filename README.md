# Getting started with MKDocs

1. Create a python project.
2. Create a venv and activate it. \
    Windows: ``venv\Scripts\activate`` \
    MacOS/Linux: ``venv/bin/activate``

3. Once activated, ``pip install mkdocs``
4. Next create the project with ``mkdocs new .`` which creates a yml file.

You now have your project setup. You can create and edit markdown files 
in the ``/docs`` directory.

### Commands:

``mkdocs serve`` - generate hot reloading docs to access and view \
``mkdocs build`` - generate the files in a directory called ``/site``

To add configuration and navigation, edit the ``mkdocs.yml`` file. The only required
field in this is ``site_name``.

Add nav:

```yaml
site_name: Test Docs
nav:
  - Home: index.md
  - About: about.md
```

### Deploy:

If you're connected to GitHub, you can build and deploy into a separate branch
with one command ``mkdocs gh-deploy``
