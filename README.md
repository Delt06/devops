
<p>
  <h1 align="center">DevOps Labs</h3>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#python-app">Python App</a>
      <ol>
        <li>
          <a href="#getting-started">Getting started</a>
        </li>
        <li>
          <a href="#usage-example">Usage example</a>
        </li>
      </ol>
    </li>
    <li>
      <a href="#docker">Docker</a>
      <ol>
        <li>
          <a href="#building-an-image">Building an image</a>
        </li>
        <li>
          <a href="#launching-the-prebuilt-image">Launching the prebuilt image</a>
        </li>
      </ol>
    </li>
    <li>
      <a href="#acknowledgements">Acknowledgements</a>
    </li>
  </ol>
</details>

## Python App

A Flask app displaying current time in Moscow.

<!-- GETTING STARTED -->
### Getting started

To get a local copy up and running follow these simple steps.

#### Prerequisites

* python3

#### Installation

* Clone the repo

```sh
git clone https://github.com/Delt06/devops
```

* Go to the `app_python` directory

```sh
cd ./devops/app_python
```

* Install `pip` requirements

```sh
pip install -r /path/to/requirements.txt
```

### Usage example

* Launch the app

```sh
flask run
```

* Open the app by the suggested link

## Docker

A docker image for the Python App.

### Building an image

* Install Docker by following the [official instructions](https://docs.docker.com/engine/install/)
* Go to the `app_python` directory

```sh
cd ./devops/app_python
```

* Launch the build

```sh
docker build -t deltation/devops-app-python .
```

### Launching the prebuilt image

* Pull the image from [Docker Hub](https://hub.docker.com/repository/docker/deltation/devops-app-python)
* Run the image

```sh
docker run -p 5000:5000 deltation/devops-app-python
```

## Acknowledgements

* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
