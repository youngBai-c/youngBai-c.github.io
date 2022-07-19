---
title: "Data100_lecture12_modeling"
date: 2022-07-19T14:25:29+08:00
draft: false
math: true
ShowToc: true
categories: [Data Science]
---

# 12.1 Motivating examples of models

## What is a model

> A model is an **idealized representation** of a system

## Why do we build models

- Most of case, we try to strike a balance between **interpretability and accuracy.**
  - To understand complex phenomenon occuring in the world we live in.
  - To make accurate predictions about unseen data.
    - **Black-box** model: Other times，extremely accurate predictions，the cost of having an uninterpretable model.

## Physical(mechanistic) model

Some models,such as the aforementioned model Of the acceleration due to gravity on Earth,
are laws that govern how the world works.We call these physical models.

- Kepler's Third Law of Planetary Motion(1619) $$ T^2 \propto R^3 $$
- Newton's Laws:motion and gravitation(1687)

$$ \mathbf{F}=m\mathbf{a} $$
$$ F = G\frac{m_1m_2}{r^2} $$

## Statistical models

Other times, we don't have such a precise understanding of some natural relationship. In such
cases, we collect data and use statistical tools to learn more about the relationships between
variables.

# 12.2 Defining the constant model. Formalizing the notion of a parameter

## A simple model - the constant model

Suppose you want to build a model to predict the percentage tip（小费）given at restaurants:

- For instance，tips likely depend on many factors...
- Ignoring these factors is **simplifying assumption.**

![](https://github.com/youngBai-c/picgo/blob/main/data100/image-12-1.png?raw=true)

## Notation

![](https://github.com/youngBai-c/picgo/blob/main/data100/image-12-2.png?raw=true)

![](https://github.com/youngBai-c/picgo/blob/main/data100/image-12-3.png?raw=true)

## Prediction vs. estimation

These terms are often used somewhat interchangeably, but there is a subtle difference
between them.

> **Estimation** is the task of using data to determine model parameters.

> **Prediction** is the task of using a model to predict outputs for unseen data.
> Once we have estimates for our model's parameters, we can use our model for prediction.
