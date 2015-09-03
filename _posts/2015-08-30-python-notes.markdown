---
layout: post
title: "Python Notes"
date: 2015-08-30
categories: 
published: true 
---

####**Updated 2015-08-30**

* NumPy "ndarray" object
  * properties
    * homogenous, all dx must be the same type
    * has a shape, a **tuple** indicating the size of each dimension
      * `dx.shape`
    * has a dtype, an object describing the data TYPE contained within
      * `dx.dtype`
    * has a ndim, a counter indicating how many dimensions the array is
      * `dx.ndim`
  * creation
    * use the np.array(data) fn/method: accepts any sequence like obj, creates ndarray
      * ex: `array = np.array(data)`