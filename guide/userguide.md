---
layout: default
title: User Guide
nav_order: 1
parent: "Guides"
---

# User Guide
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---

In this guide, we will introduce you to the process of using machine learning in product development. To give a general overview, we will start off by going through the steps, then briefly explaining the idea behind them. In Appendix A you will find a more detailed explanation of some machine learning terms you might not be familiar with.



# Getting acquainted with ML

1. Read through this document to learn more about the machine learning process
→ [Python Installation Guide](https://datacentricdesign.github.io/iot-ml-design-kit/Guides/installation-guide.html)
2. Open the [Notebook](LINK...) and go through the Use Case

# Preparing your data

3. Collecting your own data
4. Preprocessing

# Inspecting user behavior

5. Labeling and training
6. Investigating output and results


_Steps 2-3_: To collect data, you will be using a sensor with a camera yourself. The data collection process consists of a test person using your prototype while the sensor is picking up signals. Looking at the raw sensor data will probably not make any sense, so to actually generate useful data, we will have to extract all information we need to be able to tell activities apart. This is called preprocessing. 

_Steps 4-5_: You will notice that collecting just a few minutes of data generates thousands of data points. To make sure you will have to label as few of those as possible, you will be shown some points and be asked to label those. After that you can just sit back, let our system do its thing and evaluate the results! If you want to find out more about what’s going on behind the scenes, consider taking a look at Appendix B. 

