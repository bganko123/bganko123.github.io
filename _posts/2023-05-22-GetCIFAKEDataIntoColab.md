# Get CIFAKE image set into Google Collab

I was **struggling** to train and test models based on the CIFAKE data set. I was using a github codespace which was just running its normal CPU rather than a GPU. It was taking 40mins+ per epoch to train and then often the kernel would crash or the window would reload or some combination there of - Clearly untenable. So I decided to make the switch. It had taken a bit of rigmarole to get the data set into codespace and I was buckled in for the same proess in Collab but it turned out to be much easier. S0, here it is in a few easy steps.

1. TOC
{:toc}

## Get your kaggle api token
First get into kaggle and make an account if you don't already have one. Once you account is made click on the account image in the top write and select settings from the drop down. Scroll down about halfway to the API heading and click create new token. This should start a download of a *kaggle.json* file.

![](/images/kaggle1.png "albert causing trouble")

## Set up in Collab

In collab set up a new workbook or project. Then run the following:
python
``` 
! pip install -q kaggle
from google.colab import files
files.upload()
```
The should give you the option to upload a file. Browse through your file explorer to find the *kaggle.json* you just downloaded

Next, run these three commands to create a directory, move the *json* and configure the permissions
python
```
! mkdir ~/.kaggle
! cp kaggle.json ~/.kaggle/
! chmod 600 ~/.kaggle/kaggle.json
```
## Getting the Data set

Now you are pretty much could to go. You can access kaggle using your API token. To get the CIFAKE data set simply run the command below and you should see the files appear in the list of files on the right.
python
```
!pip install kaggle
import kaggle
kaggle.api.dataset_download_files('birdy654/cifake-real-and-ai-generated-synthetic-images', path='CIFAKE-dataset', unzip=True)
```
and you are good to go. Happy training

