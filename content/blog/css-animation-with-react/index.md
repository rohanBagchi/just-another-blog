---
title: CSS Animation with React
date: "2021-07-21"
description: A brief run down of how to thinnk about CSS animations with React based web app
published: true
---

Welcome to CSS Animation with React.

At a high level, I can think of 4 ways / kinds of CSS animation we can attempt.

1. A component is in view and we are animating a part of it.

   Example: a notification bubble showing up next to a nav item.

2. Show / Hide animation of a component.

   Example: a Modal that has to fade into view and fade out on close.

3. Animate mount and unmount of a component inside a list.

   Example: a TODO app. We animate addition and removal of a TODO item.

4. A `Preview` & `View More` kind of layout where the `Preview` & `View More` components are different. This kind is what we will talk about in this post.