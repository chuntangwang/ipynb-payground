# ipynb-playground

Playground for Jupyter notebook with vscode

## Tools

* [vscode](https://code.visualstudio.com/)
* [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

## Usage

### Python with asdf

* [asdf](https://github.com/asdf-vm/asdf)
* [asdf-python](https://github.com/asdf-community/asdf-python)

```bash
$ ~ > asdf update
$ ~ > asdf list all python
$ ~ > asdf install python 3.13.1

$ ~ > cd ipynb-playground
$ ~/ipynb-playground > asdf local python 3.13.1
$ ~/ipynb-playground > python --version
Python 3.13.1
```

### Virtual Environment in Project

**Create venv**

```bash
$ ~/ipynb-playground > python -m venv env

# ignore this, use Jupyter extension to select env
# $ ~/ipynb-playground > source ./env/bin/activate
```

**Select venv on Notebook**

1. Select [numpy_tab.ipynb](numpy_tab.ipynb) on vscode explorer.
2. If Juypter extension installed no problem, you will see `Select Kernal` on top right instead of text editor.
3. Click `Select Kernal` -> `Python Environments` -> Select `env (Python 3.13.1) env/bin/python`
4. Click `Run All` to run the notebook. (click install if show up a alert view to install `ipykernel`)
