Information for understanding Jupyter's Notebook is captured using resources:
1. https://www.dataquest.io/blog/jupyter-notebook-tutorial/
2. 

# Overview
The Jupyter Notebook is an incredibly powerful open source tool for interactively developing and presenting data science projects. A notebook integrates code and its output into a single document that combines visualisations, narrative text, mathematical equations, and other rich media. It is essentially just an advanced word processor. The intuitive workflow promotes iterative and rapid development, making notebooks an increasingly popular choice at the heart of contemporary data science, analysis, and increasingly science at large. 

Jupyter’s Notebooks and dashboard are web apps, and Jupyter starts up a local Python server to serve these apps to your web browser, making it essentially platform independent and opening the door to easier sharing on the web.

# Installation
The easiest way for a beginner to get started with Jupyter Notebooks is by installing Anaconda. Anaconda is the most widely used Python distribution for data science and comes pre-loaded with all the most popular libraries and tools. As well as Jupyter, some of the biggest Python libraries wrapped up in Anaconda include NumPy, pandas and Matplotlib, though the full 1000+ list is exhaustive.

To get Anaconda, simply:

<li>
<ul>Download the latest version of Anaconda for Python 3 (ignore Python 2.7).
<ul>Install Anaconda by following the instructions on the download page and/or in the executable.
<ul>If you are a more advanced user with Python already installed and prefer to manage your packages manually, you can just use pip:
    pip3 install jupyter
</li>

# About ipynb File
It will be useful to understand what this file really is. Each .ipynb file is a text file that describes the contents of your notebook in a format called JSON. Each cell and its contents, including image attachments that have been converted into strings of text, is listed therein along with some metadata. You can edit this yourself — if you know what you are doing! — by selecting “Edit > Edit Notebook Metadata” from the menu bar in the notebook.

# The Notebook interface
There are two fairly prominent terms that you should notice, which are probably new to you: cells and kernels are key both to understanding Jupyter and to what makes it more than just a word processor. Fortunately, these concepts are not difficult to understand.

1. A kernel is a “computational engine” that executes the code contained in a notebook document.
2. A cell is a container for text to be displayed in the notebook or code to be executed by the notebook’s kernel.

## Cells
Cells form the body of a notebook. There are two main cell :

1. A code cell contains code to be executed in the kernel and displays its output below.
2. A Markdown cell contains text formatted using Markdown and displays its output in-place when it is run.

The first cell in a new notebook is always a code cell.

There is always one “active” cell highlighted with a border whose colour denotes its current mode, where green means “edit mode” and blue is “command mode.”

### Markdown
Markdown is a lightweight, easy to learn markup language for formatting plain text. Its syntax has a one-to-one correspondance with HTML tags.

## Kernels
Behind every notebook runs a kernel. When you run a code cell, that code is executed within the kernel and any output is returned back to the cell to be displayed. The kernel’s state persists over time and between cells — it pertains to the document as a whole and not individual cells.

For example, if you import libraries or declare variables in one cell, they will be available in another. In this way, you can think of a notebook document as being somewhat comparable to a script file, except that it is multimedia. 

Options:
1. Restart: restarts the kernel, thus clearing all the variables etc that were defined.
2. Restart & Clear Output: same as above but will also wipe the output displayed below your code cells.
3. Restart & Run All: same as above but will also run all your cells in order from first to last.

If your kernel is ever stuck on a computation and you wish to stop it, you can choose the Interupt option.