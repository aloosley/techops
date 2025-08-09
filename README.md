# TechOps

## Introduction

* Are you looking for guidance on how to create technical documentation for your AI/ML system 
  and/or its constituent models and datasets?  
* Should your AI/ML system documentation provide value to a wide variety of user personas 
  (e.g. managers, system users, developers, researchers, regulators, etc.)?
* Does your AI/ML system need to comply with the EU AI Act, or are you developing a model or dataset that
  you want to be used as part of an AI/ML system that needs to comply with the EU AI Act?

If you answered yes to any of these questions, TechOps is for you.  

TechOps, published in [AIES 2025](https://www.aies-conference.com/2025/) (see [citation details](#citing) below), 
is a set of documentation templates and examples designed to help technical teams and companies
document their AI/ML applications, models, and datasets. TechOps is also the first set of documentation 
templates that we know of to completely map its sections to the EU AI Act, for developers and providers 
that need to comply with this regulation that first came into force in August 2024.

While rendering agnostic content is the primary contribution of TechOps, content rendering is almost 
always needed to make such content useful to a real world audience.  For documentation developers that do 
not already have their own systems of documentation rendering, we provide a [blueprint for rendering TechOps Documentation](#blueprint-for-rendering-techops-documentation).  This blueprint is designed to make TechOps Documentation readable by a wide variety of reader personas (technical users, business analysts, regulators, etc.), by rendering these complex documents with a side navbar so readers can quickly drill down to find the information they most need to see, without losing track of the big picture (see screenshot below).

<img src="paper/aies/rendering.png" width="700" alt="Example of rendering TechOps Documentation">

See [the TechOps website](https://aloosley.github.io/techops/) to dive in deeper and/or explore our templates
and examples.

## Citing

If you use and parts of this work, we kindly ask that you cite our paper:

```bibtex
@inproceedings{lucaj2025techops,
   title     = {TechOps: Technical Documentation Templates for the AI Act},
   author    = {Laura Lucaj and Alex Loosley and H{\aa}kan Jonsson and Urs Gasser and Patrick van der Smagt},
   booktitle = {Proceedings of the Eighth {AAAI/ACM} Conference on AI, Ethics, and Society {(AIES-25)}},
   publisher = {{AAAI} Press},
   year      = {2025}
}
```

## Blueprint for Rendering TechOps Documentation

Developing TechOps Documentation is easy, it's just markdown!  TechOps Documentation is, on purpose, rendering 
agnostic, so it can be integrated with any existing documentation systems as needed.  However, we also provide
an [mkdocs](https://www.mkdocs.org/) based blueprint for rendering TechOps Documentation.

Follow these instructions to get started.

### Prerequisites

* Python 3.12 or later is installed (we've tested this with Python 3.12, but it likely also works with older versions)
* Optional, but recommended, [uv](https://docs.astral.sh/uv/) is installed
* You are in your own fork/copy of this documentation repo, where you can create your own documentation.

### Install Rendering Dependencies

#### With UV

<details>

1. UV will automatically install dependencies into a virtual environment (venv) under the current folder (`/.venv):

    ```bash
    uv sync
    ```

2. Install the pre-commit hooks

    ```bash
    uv run pre-commit install
    ```

    These commit hooks are purely optional, but help ensure markdown stay clean while creating TechOps Documentation.
3. Going forward, whenever the command `uv run` is used, all the follows will run instead the correct python venv

</details>

#### With PIP

<details>

1. It is recommended that you create a [virtual environment](https://docs.python.org/3/library/venv.html) (venv) before installation with pip (Python's Preferred Installer Program)
2. Install with pip:

    ```bash
    pip install .
    ```

3. Install the pre-commit hooks 

    ```bash
    pre-commit install
    ```

    These commit hooks are purely optional, but help ensure markdown stay clean while creating TechOps Documentation.
4. Going forward, you'll need to ensure the correct venv is activated before developing or rendering

</details>

### Rendering

#### Dependencies Installed with UV

<details>

Start rendering with

```bash
uv run mkdocs serve
```

</details>

#### Dependencies Installed without UV

<details>

1. Ensure the correct virtual environment where you installed the dependencies (above) is activated
2. Start rendering with

    ```bash
    mkdocs serve
    ```

</details>

### Create Your Own TechOps Documentation

Assuming you didn't change any documentation in the `docs/` folder, your first rendering via `mkdocs serve`
will render a local version of the
[TechOps Website](https://aloosley.github.io/techops/).  Now you are ready to replace the examples with 
TechOps documentation of your AI/ML system.  Happy documenting.

### Deploying

Mkdocs websites can be deployed like any other webapp, but some online sites provide out-of-the-box online 
deployments.  For more information on deploying, see the official [mkdocs deployment documentation](https://www.mkdocs.org/user-guide/deploying-your-docs/).
