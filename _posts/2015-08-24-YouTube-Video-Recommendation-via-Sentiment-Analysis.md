---
layout: post
title: YouTube Video Recommendation via Sentiment Analysis
---

I built a YouTube video recommendation system based on sentiment of video comments. The sentiment analysis is done using MonkeyLearn. The results were stored into a MongoDB database. The sentiment scores were adjusted for the number of comments with scores adjusted downward with fewer comments. This adjustment was done using a customized sigmoid function. A neural network is used to predict up and downvotes of the video based on sentiment score and other features.
