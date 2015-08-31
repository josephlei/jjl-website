---
layout: post
title: "Python Notes"
date: 2015-08-30
categories: 
published: true 
---

####Python Notes

####**Updated 2015-08-30**

* NumPy "ndarray" object
  * properties
    * homogenous, all dx must be the same type
    * has a shape, a tuple indicating the size of each dimension
    * has a dtype, an object describing the data TYPE contained within
    * use `data.shape` and `data.dtype` to access
  * creation
    * use the np.array(data) fn/method: accepts any sequence like obj, creates ndarray
      * ex: array_1 = np.array(data)
