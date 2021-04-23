# Dark PDF 

[![Convert PDF to PDF by inverting colours](https://github.com/mrtrkmnhub/darkpdf/actions/workflows/automater.yml/badge.svg)](https://github.com/mrtrkmnhub/darkpdf/actions/workflows/automater.yml)

This is an automated tool which converts background of PDF to Dark and automatically releases it. 

CI file runs when something is changed on files which ends with `*.pdf` under [./uploads](./uploads). 

To run the automated tool it is enough to add PDF files to [./uploads](./uploads) then CI file will automatically start. 

# How to run 


```bash 
$ git clone --depth 1 git@github.com:mrtrkmnhub/darkpdf.git
$ cd darkpdf
```
Once you have added your PDF files to [uploads](./uploads) folder, it is time to commit and push them to master branch as shown below. 

```bash 
$ git add uploads/*
$ git commit -m "<commit-message>" 
$ git push origin master
```

Once you have pushed it, dark version of PDF will be available under [releases](https://github.com/mrtrkmnhub/darkpdf/releases)


## Example 

![Example output of the tool](.github/images/readme_pic.png)
 
 
## How to run on local 

-  Create virtual python environment 

  ```python3
     python3 -m venv ./venv
  ```

- Source venv 

 ```bash 
     source ./venv/bin/activate
 ```
  
 -  Upgrade pip and Install requirements 

 ```bash 
    pip install --upgrade  pip
    pip install -r requirements.txt
 ```

-  Place PDF files to [./uploads](./uploads) folder  and run script
 *(Converted PDF Files will be in root folder of the project )

```python3
    python run converter.py 
```

The script can be extended more such as integration of Telegram, Slack, Discord bots and more. 

