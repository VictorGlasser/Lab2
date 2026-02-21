# CST8917 - Lab 2

## Local Test

![alt text](image.png)
This screenshot shows the function app working for a local image container

## Azure Test
![alt text](image-1.png)
This screenshot was taken before 11:59, showing that it was woring and the video was recorded before 11:59 PM

## Video Link
### Single File
YouTube Link: https://youtu.be/LMog0kZrnuc
### Multiple Files
YouTube Link: https://youtu.be/Rs76VFYfb-I

## Instructions

### Prerequisites
- Python 3.11 or 3.12
- Azure Functions Core Tools installed
- An Azure account

### Preparing your environemt

- clone the repo using:
```
git clone https://github.com/VictorGlasser/Lab2
```
- install the packages using
```
source .venv/bin/activate
python -m pip install -r requirements.txt
```

### Preparing Azure

- Press F1 > Azure Functions: Create Function App in Azure...(Advanced)

- Create your function app for a consumption plan and take note of your globally unique name to use later.

- Add the ImageStorageConnection setting to your Function App by going to Settings > Environment variables

- Click + Add and then add the connection string to your storage account, which is found by going to Storage Account > Access keys > copy the Connection string

- Create a container names images by going to Data Storage > Containers, and then clicking "+ container".

### Deploying

- Press F1 > Azure Functions: Deploy to Function App

### Testing

- Upload an image to the image container

- Copy in paste this URL "https://function-app-name.azurewebsites.net/api/results", while replacing "function-app-name" to whatever you names your function app