---
layout: default
title: Data Collection Guide
nav_order: 3
parent: "Guides"
---

# Data Collection Guide

Now that you read through the guide and used the product, we hope you’ll have a good idea of how it works. 
You can now start collecting your own data, train a model, then analyze user behavior. The data you collect has a great impact on the final output, so please read through the following remarks carefully. 
**You can start only after you’ve checked off all the boxes**.

- [ ] Evaluate the type of prototype you are designing. Could features like gender, age, physical strength or intelligence influence the way people will be using your product in any way? If that’s the case, make sure to have a _representative group_ of people collect data. For example, if you’re designing a vacuum cleaner, the data left-handed people generate will look different than right-handed subjects’ data. Taking this into account will also give insight about how inclusive your prototype is.
- [ ] When you’re collecting your data, the algorithm works by trying to find patterns. In order for the models to work properly, you need to perform activities that consist of _repetitive movements_. 
- [ ] The longer the movement, the easier it is for the algorithm to differentiate between activities. Think of long arm strokes, but also duration of a single movement. This means that placing the sensor is an important step of collecting data. The more and longer the movements, the better the results will be. Sensor placement should allow for maximum movement. For vacuum cleaning, this could be the hands for example.
- [ ] The sensor you will be using collects data about position, as well as rotation. Try to move in a natural way, so that your model is trained on data that approaches real-life use of your product as much as possible. 
- [ ] Sensor placement is up to you. Because the sensors detect movement based on deviation from a set point, it’s important to stay consistent. If you have multiple people collecting data, make sure to place them on the _same position_ on either their body or your prototype. The same applies when you put the sensor back on after taking a coffee break for instance.
- [ ] You will be asked later on to evaluate activities based on their timestamp and a short clip. Inform all test subjects of the fact that you will be using camera footage. It is very important that you have your subjects’ [written consent](LINK) to appear in these recordings. 

Now that you went through the points listed above, you can start off by placing the sensor in a way that’s easily reproducible for you. After doing this, you can test if this placement works, i.e. doesn’t move around, is comfortable for the test subject, and doesn’t strain their movement. Having found a suitable sensor placement, you can finally start recording! **Read through the following requirements**:

Record about **15 minutes** of consecutive movement, where:

You are using no other sensor than an accelerometer and/or gyroscope. For sources other than GoPro, please keep in mind that other steps might be necessary to convert the data to the right import type.

Each of the expected activities gets recorded for **at least 30 seconds**

Now that you have your data, you can start processing it. export gopro?..., continue to notebook
