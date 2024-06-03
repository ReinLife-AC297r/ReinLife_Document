# ReinLife_Document

Document of ReinLife mobile health platform.

## What is ReinLife

ReinLife is a mobile health (mHealth) app, but not only an app. It aims to serve as a mHealth platform that allow clinicians and machine learning (ML) researchers to customize the app contents to send personalized questionnaires and provide interventions as push notifications based on their customized reinforcement learning (RL) algorithms. 

The current version of ReinLife is based on Google Flutter and Google Firebase. Here are the links to the [frontend repo](https://github.com/ReinLife-AC297r/reinlife_flutter) and [backend python APIs](https://github.com/ReinLife-AC297r/reinlife_backend) for researchers and clinicians. Here are a detailed [manuscript](to be linked) and [slides](to be linked) introducing ReinLife.

The Flutter framework allows us to build cross-platform apps that support both iOS and Android systems. For demonstration purpose, a web version has also been created, that allow interested users to easily get a flavor of our app.

## A Quick Start Guide

This quick start guide aims to provide ML researchers the workflow of our platform, especially python backend APIs.

### Open Frontend App

As a quick starter, please go to this [website](https://flutternotification-ebd50.web.app) to try out a web version of our app that is deployed on Google Firebase. Please make sure to give your web browser access to push notifications to ensure the web app can function properly. 

**Potential issues for the web version of our app:**
1) If using browsers on iOS, it will only work on iOS 16.4 or later, and you need to "add the website to home page" before trying the app.
2) If using browsers on MacOS, make sure to give notification access to your browswer.
3) It might have issues on FireFox.
4) The push notification logics has not been optimized for the web version, so please only consider this as a demo of our app.

### Run Backend Python APIs






