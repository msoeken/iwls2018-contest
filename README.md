# IWLS 2018 Programming Contest: "All the Best!"

## Description

In 2018, we will organize a programming contest at the [International
Workshop on Logic & Synthesis](http://www.iwls.org/iwls2018/) (IWLS).
To participate, please follow these steps:

1. Read the [contest description](contest.pdf).

2. Write a computer program that takes as input a truth table in
   hexadecimal representation, a number of fanins *k*, and a number of
   gates *r*, that generates a BLN file as explained in the contest
   description.  For example to synthesize the majority-of-three
   function as 4-gate circuits with 2-input gates, the program is
   called

```
program 8e 2 4
```

3. We will publish the contest benchmark functions on **April 27,
   2018**.  These will be used to evaluate your algorithms.

4. You need to submit your binary or source code and the resulting BLN
   files for the contest benchmarks until **May 4, 2018**.  Please
   send everything via email to [Mathias
   Soeken](https://github.com/msoeken).  We must be able to reproduce
   your results on our machines within a timeout of 60 minutes for
   each benchmark.

5. We will submit the generated BLN files from your submissions until
   **May 11, 2018** and announce all the results on this webpage.

6. The submissions are rated according to the number of found
   solutions within the runtime limit of one hour.  If for some
   benchmark a wrong solution is reported (i.e., it computes the wrong
   function or it does not respect the normalization rules), the
   overall count for that benchmark is halved for each wrong solution.
   (Example: If 3 wrong solutions are found, only 12.5% of the overall
   count will be considered in the final evaluation.)

7. You are encouraged to share your source code with the IWLS
   community, but it's not required or has any effect on the rating.
   If you want to share, you can either point us to an online
   repository that we will link to this and the IWLS webpage.  If you
   prefer to share the source code only among the IWLS participants,
   we will copy your code onto the proceeding pen drives.

If you have any question, please create an
[issue](https://github.com/msoeken/iwls2018-contest/issues).

## Useful software

Several algorithms for exact synthesis are available as open source
implemenations and may be used as a starting point, including:

- [ABC](https://bitbucket.org/alanmi/abc): Commands `exact`, `twoexact`, `majexact`, `lutexact`

- [CirKit](https://github.com/msoeken/cirkit): Commands `exact_mig`, `exact_xmg`

