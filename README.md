# ReinLife_Document

Document of ReinLife mobile health platform.

## What is ReinLife

ReinLife is a mobile health (mHealth) app, but not only an app. It aims to serve as a mHealth platform that allow clinicians and machine learning (ML) researchers to customize the app contents to send personalized questionnaires and provide interventions as push notifications based on their customized reinforcement learning (RL) algorithms. 

The current version of ReinLife is based on Google Flutter and Google Firebase. Here are the links to the [frontend repo](https://github.com/ReinLife-AC297r/reinlife_flutter) and [backend python APIs repo](https://github.com/ReinLife-AC297r/reinlife_backend_APIs) for researchers and clinicians. Here are a detailed [manuscript]([to be linked](https://github.com/ReinLife-AC297r/ReinLife_Document/blob/main/manuscript_and_slides/AC297r_Final_Report.pdf)) and [slides](to be linked) introducing ReinLife.

The Flutter framework allows us to build cross-platform apps that support both iOS and Android systems. For demonstration purpose, a web version has also been created, that allow interested users to easily get a flavor of our app.

## A Quick Start Guide

This quick start guide aims to provide ML researchers the workflow of our platform, especially python backend APIs.

### 1. Open Frontend App

As a quick starter, please go to this [website](https://flutternotification-ebd50.web.app) to try out a web version of our app that is deployed on Google Firebase. Please make sure to give your web browser access to push notifications to ensure the web app can function properly. 

**Potential issues for the web version of our app:**
1) If using browsers on iOS, it will only work on iOS 16.4 or later, and you need to "add the website to home page" before trying the app.
2) If using browsers on MacOS, make sure to give notification access to your browswer.
3) It might have issues on FireFox.
4) The push notification logics has not been optimized for the web version, so please only consider this as a demo of our app.

### 2. Run Backend Python APIs

#### 2.1 Download Code
The backend python APIs are written as a python module `ReinLifeResearcher.py`. Researchers should download the code at the [backend python APIs repo](https://github.com/ReinLife-AC297r/reinlife_backend_APIs), create a virtual environment (optionally), and install dependencies in `requirements.txt` using `pip install -r requirements.txt`



#### 2.2 Run a Jupyter Notebook Tutorial
`example_researcher_defined_code.ipynb` serves as an interactive tutorial to our APIs.

##### 2.2.1 Download Private Key For Firebase AdminSDK
The backend python APIs are communicating with the firebase backend service via Firebase AdminSDK. To quickly try out our demo, researchers can contact us for the key that is linked to our firebase account for the demo project, and put it into the repo for the backend APIs. (The name of the private key is currently hardcoded in `server2firestore.py` and need to be improved in the future. We expect that in the long run, researchers should integrate the frontend to their own firebase accounts.)

##### 2.2.2 Configuration files
To experiment configuration file `experiment_info.json` and questionnaire configuration `questionnaires.json` files serve as examples.

##### 2.2.3 Explore the tutorial
In this example code, you will set experiment information, push different questionnaires to frontend app users, and run a dummy ML code to send interventions to advocate healthier diet based on the frequency of the answers 'broccoli' and 'asparagus' in each user's answers to the first question.

### 3. Conduct your own experiments
Congratulations! Now you should be able to configure your own experiments with our Python APIs.

**Final notes:**
1) In our current version, we have not configured notification message for iOS systems. We will need to register a developer account and pay a $100 membership fee to do the configuration.
2) The backend has been configured on our personal google Firebase accounts. We expect each researcher/research group should copy our Flutter code and deploy the app to their own Firebase accounts following the [instruction document](https://tbd).

## Full Document
[Frontend Documents](https://tbd)

[Backend Documents](https://tbd)



 











