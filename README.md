Hugging Face models
https://huggingface.co/kc928/AI4ALL-UCSF-Reddit-2023-Age

https://huggingface.co/kc928/AI4ALL-UCSF-Reddit-2023-Gender

https://huggingface.co/kc928/AI4ALL-UCSF-Reddit-2023-Subject


# Setup Instructions

1. Download Repository
2. Install Miniconda
3. Setup Reddit API Key
4. Install Necessary Libraries

## 1. Download Repository
The GitHub Repo is located at https://github.com/AlbertLeeUCSF/reddit_2023. From there, you can download the entire repo as a zip file, and unzip it on your computer.

## 2. Install Miniconda
You'll need to install Miniconda to get Python and other libraries required for this project. The download links for the installation files of Miniconda are located at https://docs.conda.io/en/main/miniconda.html#installing

## 3. Setup Reddit API Key
Follow the instructions on https://rymur.github.io/setup to create a new app on Reddit. Once you create the new application, not the *personal use script*, *secret*, and *developers* on the page that summarizes the app's information.

Create a new file inside of the unzipped repo on your computer called *reddit_api.json*. Add the following details to *reddit_api.json* and save the file.
```
{
  "client_id": "replace_with_personal_use_script",
  "secret": "replace_with_secret",
  "user_agent": "replace_with_developer"
}

```

## 4. Install Necessary Libraries
Open command line (*terminal* or *command prompt*) and navigate to the repository using the `cd` command.
```
cd replace_with_your_path/reddit_2023
```

Then install virtualenv using `conda install ...`.
```
conda install virtualenv
```

Then create a new virtual environment call *env* inside of the repo.
```
python -m venv env
```

Now let's activate the environment. Be sure to do this each time you need to work on the project.
```
. env/bin/activate
```

Now that the environment has been activated, you can go ahead and install the libraries listed in *requirements.txt*.
```
pip install -r requirements.txt
```

At this point, you can now access the project in Jupyter.
```
jupyter lab
```
