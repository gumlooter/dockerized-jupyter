# Jupyter Docker Stack with extra flavour for data analysis

Based on https://hub.docker.com/r/jupyter/datascience-notebook/ from https://github.com/jupyter/docker-stacks

[![Telegram](https://img.shields.io/badge/telegram-chat%20with%20me-blueviolet)](https://t.me/gumlooter "Open Telegram with gumlooter") [![](https://images.microbadger.com/badges/version/gumlooter/dockerized-jupyter.svg)](https://hub.docker.com/r/gumlooter/dockerized-jupyter "DockerHub")

![WYSIWYG](https://github.com/gumlooter/dockerized-jupyter/raw/master/screenshot.png "Funny title")

## As simple as
```docker run -p 8888:8888 gumlooter/dockerized-jupyter:latest```

## Additions

### Linux
* jq
* openssh-client

### Python
* gspread
* oauth2client
* pyopenssl
* psycopg2
* pymystem3
* tensorflow (1.15)
* plotly
* dash
jupyter labextension install jupyterlab-plotly@1.3.0 --no-build

# FigureWidget support
jupyter labextension install plotlywidget@1.3.0 --no-build

### R
* hmisc
* psych
* ROCR
* xtable
* stargazer
* ~gvlma~ temporary excluded

### Jupyter/JupyterLab extensions
* jupyterlab-git (+nbdime)
* @ryantam626/jupyterlab_code_formatter, jupyterlab_code_formatter (+black, yapf)
* jupyterlab_sql
* @jupyterlab/toc
* jupyter_nbextensions_configurator
* freeze/main
* autosavetime/main
* collapsible_headings/main
* execute_time/ExecuteTime
* datestamper/main
* hide_input_all/main
* varInspector/main
* code_prettify/autopep8
* toc2/main
* jupyterlab-plotly
* plotlywidget

---
Can be deployed to GCP using https://github.com/gumlooter/infra
