<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1znFGGhNTQMWz3NG4cn0YebsjlsdPr9BN">
</div>

# Aipaca Datathon Starter Code for UW CxC Summit

Hello students! Welcome to CxC Summit's Aipaca Data Challenge. You will build an alpaca binary classifier and deploy your model with the Aibro inference tool.

# Getting Started

## Step 1: Get an account

Join Aipaca's [Discord community](https://discord.gg/bYB7EuXzWW) and register for an Aipaca account on https://aipaca.ai.

## Step 2: Download data

Download the alpaca training data from https://drive.google.com/drive/u/0/folders/1JlEHvLpuLWsio3rZZaok_2tjSlhXxBfG. Consider expanding the size of the dataset yourself.

## Step 3: Build a model

Build and train your alpaca classifier with your chosen frameworks. Make sure you save your model! The internet is your friend, but feel free to ask any questions about Python, ML, data sci, etc in our discord!

## Step 4: Deploy the template model

1. Clone this repository: `git clone https://github.com/aipaca-mlops/cxc_datathon.git`
2. **(Optional)** Create a virtual environment by `python3 -m venv venv`, and activate it with `. venv/bin/activate`. If you are a Windows user, use `. venv/Script/activate` instead.
3. Install the newest version of aibro in your terminal with `pip install aibro`.
4. Run `python3 turnon_deploy.py`. You will be asked to input your Aipaca account's email & password. We recommend you to use an [access token](https://doc.aipaca.ai/inference#authentication) instead.
5. After step 4, you will receive an inference API URL. You can input the URL into `test_api.sh` then use `bash test_api.sh` to test your API.

## Step 5: Deploy your own model

Modify `model.py` and `predict.py` with respect to your own alpaca classifier. As long as `run(load_model())` from `predict.py` can return the prediction result, your model repository is ready to deploy. Please make sure that your API return is a dictionary, where the key is the image file name and the value is the inference result. Feel free to add other artifacts if there is a need.

Before the final deployment, we recommend you to turn on `DRYRUN` in `turnon_deploy.py` to validate your model repository. Once `DRYRUN` test is passed, you can turn off `DRYRUN` and start the deployment.

## Tips

- Remember to update `requirement.txt` if your model is built by extra libraries.
- You can find more inference examples at [Aibro-examples](https://github.com/aipaca-mlops/Aibro-examples).
- The Colab inference demo and documentation are all available on https://aipaca.ai.
- If you found any technical issues, feel free to contact Aipaca's **Admin** team in Aipaca's [Discord community](https://discord.gg/bYB7EuXzWW). If you are not a Discord user, you can also send us an email to hello@aipaca.ai.

# We need your feedback

Share your Aipaca experience with us. We would like to hear how we can improve to better serve you in the future!
