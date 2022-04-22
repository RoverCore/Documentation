---
title: "Background Tasks"
linkTitle: "Background Tasks"
weight: 1
description: >
  Learn about background tasks in ASP.NET Core.
---

## What is a background task?

A background task, as the name suggests, is an action that happens within the background of a program. The background is usually unseen and inaccessible to the person using the program. Background tasks are often asynchronous, which means that they occur independently of other actions going on within the program. These tasks usually don't require user input and are designed to work independent of what the user is doing.

[This article](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services?view=aspnetcore-6.0&tabs=visual-studio) by Microsoft shows various ways to create and use background tasks.

## Why use them?

Background tacks are incredibly useful if not essential to many softwares. If people use software for any reason, having the ability to perform tasks without their input is extremely beneficial. Good examples of background tasks would be a task that monitors a user's activity on a certain page or one that sends an email after a user performs a certain action. Tasks like these could really only exist in the background and would not work properly if they needed input from a user. For an example of how important background tasks are, open the task manager on any computer and take note of just how many programs are required to run in the background to make the computer perform properly
