---
layout: post
title: "SAS Advanced Certification Study Tips"
date: 2015-07-23
categories: 
published: true
---

### What I studied when preparing for the SAS Advanced Certification Exam

A word of caution, both the SAS Base and SAS Advanced Certifications are **hard**.  If you're like me and felt that you've done all the practice questions.. do them again, and focus on in depth version or consider the most complicated way you can be asked a question or tested on a concept.

The advanced certification exam tests understanding of three courses: SQL 1, Macro 1 and Programming 3.

#### **Updated 2015-09-11**

#### Legend of the abbreviations I use
* Mvar = Macro Variable
* Dx = Data or dataset
* IDx = Input dataset
* ODx = Output dataset
* Ps = PROC SQL

***

* PROC SQL
  * When using Ps to create a Mvar, remember that the syntax is `SELECT INTO :Mvar-name`
    * The colon comes BEFORE the Mvar-name
  * Set operators
    * UNION, OUTER UNION, EXCEPT, INTERSECT
    * Both when used alone and with optional modifiers `ALL` and `CORR`
    * With OUTER UNION, only the `CORR` option makes a difference
  * What's the difference between WHERE and HAVING clauses? How do you use each?
  * What's the syntax for using the WHERE clause to condition on a missing value?
  * What is considered ANSI standard SQL and what is a SAS enhancement?

Much more to come once I get a little time to settle back in.
