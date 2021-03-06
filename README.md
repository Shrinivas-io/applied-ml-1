<div align="center">
<h1><img width="30" src="https://madewithml.com/static/images/rounded_logo.png">&nbsp;<a href="https://madewithml.com/">Made With ML</a></h1>
Applied ML · MLOps · Production
<br>
Join 20K+ developers in learning how to responsibly <a href="https://madewithml.com/about/">deliver value</a> with applied ML.
</div>

<br>

<div align="center">
    <a target="_blank" href="https://madewithml.com/subscribe/"><img src="https://img.shields.io/badge/Subscribe-20K-brightgreen"></a>&nbsp;
    <a target="_blank" href="https://github.com/GokuMohandas/madewithml"><img src="https://img.shields.io/github/stars/GokuMohandas/madewithml.svg?style=social&label=Star"></a>&nbsp;
    <a target="_blank" href="https://www.linkedin.com/in/goku"><img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social"></a>&nbsp;
    <a target="_blank" href="https://twitter.com/GokuMohandas"><img src="https://img.shields.io/twitter/follow/GokuMohandas.svg?label=Follow&style=social"></a>
</div>

<br>

> If you need refresh yourself on ML algorithms, check our out [ML Foundations](https://github.com/GokuMohandas/madewithml) repository (🔥&nbsp; Among the <a href="https://github.com/topics/deep-learning" target="_blank">top ML</a> repositories on GitHub)

<br>

<table>
    <tr>
        <td align="center"><b>📦&nbsp; Product</b></td>
        <td align="center"><b>🔢&nbsp; Data</b></td>
        <td align="center"><b>📈&nbsp; Modeling</b></td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/objective/">Objective</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/annotation/">Annotation</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/baselines/">Baselines</a></td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/solution/">Solution</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/exploratory-data-analysis/">Exploratory data analysis</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/experiment-tracking/">Experiment tracking</a></td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/evaluation/">Evaluation</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/splitting/">Splitting</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/optimization/">Optimization</a></td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/iteration/">Iteration</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/preprocessing/">Preprocessing</a></td>
        <td></td>
    </tr>
</table>

<table>
    <tr>
        <td align="center"><b>📝&nbsp; Scripting</b></td>
        <td align="center"><b>(cont.)</b></td>
        <td align="center"><b>📦&nbsp; Application</b></td>
        <td align="center"><b>✅&nbsp; Testing</b></td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/organization/">Organization</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/styling/">Styling</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/cli/">Command line</a></td>
        <td>Code</td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/packaging/">Packaging</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/makefile/">Makefile</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/api/">RESTful API</a></td>
        <td>Data</td>
    </tr>
    <tr>
        <td><a href="https://madewithml.com/courses/applied-ml/documentation/">Documentation</a></td>
        <td><a href="https://madewithml.com/courses/applied-ml/logging/">Logging</a></td>
        <td></td>
        <td>Model</td>
    </tr>
</table>

<table>
    <tr>
        <td align="center"><b>⏰&nbsp; Version control</b></td>
        <td align="center"><b>🚀&nbsp; Production</b></td>
        <td align="center"><b>(cont.)</b></td>
    </tr>
    <tr>
        <td>Git</td>
        <td>Dashboard</td>
        <td>Serving</td>
    </tr>
    <tr>
        <td>Precommit</td>
        <td>Docker</td>
        <td>Feature stores</td>
    </tr>
    <tr>
        <td>Versioning</td>
        <td>CI/CD</td>
        <td>Workflow management</td>
    </tr>
    <tr>
        <td></td>
        <td>Monitoring</td>
        <td>Active learning</td>
    </tr>
</table>

📆&nbsp; new lesson every week!<br>
<a href="https://madewithml.com/subscribe/" target="_blank">Subscribe</a> for our monthly updates on new content.

<br>

## Set up
```bash
python3 -m venv venv
source venv/bin/activate
python -m pip install --upgrade pip setuptools wheel
make install-dev
```

## Start Jupyterlab
```bash
python -m ipykernel install --user --name=tagifai
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter labextension install @jupyterlab/toc
jupyter lab
```
> You can also run all notebooks on [Google Colab](https://colab.research.google.com/github/GokuMohandas/applied-ml/blob/main/notebooks/tagifai.ipynb).

## Directory structure
```bash
app/
├── api.py        - FastAPI app
└── cli.py        - CLI app
├── schemas.py    - API model schemas
tagifai/
├── config.py     - configuration setup
├── data.py       - data processing utilities
├── models.py     - model architectures
├── predict.py    - inference utilities
├── train.py      - training utilities
└── utils.py      - supplementary utilities
```
> Documentation can be found [here](https://gokumohandas.github.io/applied-ml/).

## Workflow
1. View all available options using the CLI app:
```bash
tagifai --help
tagifai train-model --help
```
2. Download the necessary data files to `assets/data`.
```bash
tagifai download-data
```
3. Optimize using distributions specified in `tagifai.train.objective`. This also writes the best model's args to `config/args.json`
```bash
tagifai optimize --num-trials 100
```
> We'll cover how to train using compute instances on the cloud from Amazon Web Services (AWS) or Google Cloud Platforms (GCP) in later lessons. But in the meantime, if you don't have access to GPUs, check out the [optimize.ipynb](https://colab.research.google.com/github/GokuMohandas/applied-ml/blob/main/notebooks/optimize.ipynb) notebook for how to train on Colab and transfer to local. We essentially run optimization, then train the best model to download and transfer it's arguments and artifacts. Once we have them in our local machine, we can run `tagifai set-artifact-metadata` to match all metadata as if it were run from your machine.
4. Train a model (and save all it's artifacts) using args from `config/args.json`
```bash
tagifai train-model --args-fp config/args.json
```
5. Predict tags for an input sentence. It'll use the best model saved from `train-model` but you can also specify a `run-id` to choose a specific model.
```bash
tagifai predict-tags --text "Transfer learning with BERT"
```

## API
```bash
uvicorn app.api:app --host 0.0.0.0 --port 5000 --reload --reload-dir tagifai --reload-dir app # start API
gunicorn -c config/gunicorn.py -k uvicorn.workers.UvicornWorker app.api:app  # gunicorn
```

## MLFlow
```bash
mlflow server -h 0.0.0.0 -p 5000 --backend-store-uri assets/experiments/
```

## Mkdocs
```bash
python -m mkdocs serve
```

## FAQ

### Why is this free?
While this content is for everyone, it's especially targeted towards people who don't have as much opportunity to learn. I firmly believe that creativity and intelligence are randomly distributed but opportunity is siloed. I want to enable more people to create and contribute to innovation.

### Who is the author?
- I've deployed large scale ML systems at Apple as well as smaller systems with constraints at startups and want to share the common principles I've learned along the way.
- I created [Made With ML](https://madewithml.com/) so that the community can explore, learn and build ML and I learned how to build it into an end-to-end product that's currently used by over 20K monthly active users.
- Connect with me on <a href="https://twitter.com/GokuMohandas" target="_blank"><i class="fab fa-twitter ai-color-info mr-1"></i>Twitter</a> and <a href="https://www.linkedin.com/in/goku" target="_blank"><i class="fab fa-linkedin ai-color-primary mr-1"></i>LinkedIn</a>
