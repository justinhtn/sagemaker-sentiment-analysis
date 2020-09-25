# Sagemaker sentiment analysis

<img src="https://repository-images.githubusercontent.com/273963529/91012480-fe88-11ea-8444-71c065a1c6c8" width="700" />

The notebook provided in this repository are intended to be executed using Amazon's SageMaker platform. But if you're looking just to play with the web app, see instructions below.

---

 
 ## Update:
To avoid uncessary costs, the sagemaker endpoint has been deleted. If you're interested in working together and would like to test out the web app, please contact me and I'd be more than happy to create a new endpoint! In the meantime, you can view the static notebook inside of deepnote using the button below.
 
 <a href=" https://deepnote.com/project/348acfd6-62f0-4d91-937b-a244079511f1"> <img src="https://beta.deepnote.com/buttons/launch-in-deepnote.svg"> </a>

## ~~Steps to play with web app~~
 
1. ~~Head over to [Sentiment app](https://justinhtn.github.io/sagemaker-sentiment-analysis/) (running on github pages)~~

2. ~~Copy and paste a review from imdb, yelp or make your own up.~~

3. ~~Submit the review and check the results!~~

## Steps to run in Sagemaker

Log in to the AWS console and create a notebook instance
Log in to the AWS console and go to the SageMaker dashboard. Click on 'Create notebook instance'. The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. For the role, creating a new role works fine. Using the default options is also okay. Important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or object with sagemaker in the name is available to the notebook.

Use git to clone the repository into the notebook instance
Once the instance has been started and is accessible, click on 'open' to get the Jupyter notebook main page. We will begin by cloning the SageMaker Deployment github repository into the notebook instance. Note that we want to make sure to clone this into the appropriate directory so that the data will be preserved between sessions.

Click on the 'new' dropdown menu and select 'terminal'. By default, the working directory of the terminal instance is the home directory, however, the Jupyter notebook hub's root directory is under 'SageMaker'. Enter the appropriate directory and clone the repository as follows.

cd SageMaker
`git clone https://github.com/justinhtn/sagemaker-sentiment-analysis.git`
