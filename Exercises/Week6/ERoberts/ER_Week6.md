##
#Week 6 Assignment
###Name: Erin Roberts
###Date: March 7th, 2018

syntax "markdown" "\.(md|mdt|mdwn)$"

First, I ran the following code from Step 33 of Ref.Ex

`$ bash ReferenceOpt.sh 4 8 4 8 PE 16 &`

Next, I disowned the process using

`$ disown -a`

This produced the following output:

`
K1 is 4 K2 is 4 c is 0.9
K1 is 4 K2 is 4 c is 0.92
K1 is 4 K2 is 4 c is 0.94
K1 is 4 K2 is 4 c is 0.96
K1 is 4 K2 is 4 c is 0.98
K1 is 4 K2 is 5 c is 0.80
K1 is 4 K2 is 5 c is 0.82
K1 is 4 K2 is 5 c is 0.84
K1 is 4 K2 is 5 c is 0.86
K1 is 4 K2 is 5 c is 0.88
K1 is 4 K2 is 5 c is 0.9
K1 is 4 K2 is 5 c is 0.92
K1 is 4 K2 is 5 c is 0.94
K1 is 4 K2 is 5 c is 0.96
K1 is 4 K2 is 5 c is 0.98
K1 is 4 K2 is 6 c is 0.80
K1 is 4 K2 is 6 c is 0.82
K1 is 4 K2 is 6 c is 0.84
K1 is 4 K2 is 6 c is 0.86
K1 is 4 K2 is 6 c is 0.88
K1 is 4 K2 is 6 c is 0.9
K1 is 4 K2 is 6 c is 0.92
K1 is 4 K2 is 6 c is 0.94
K1 is 4 K2 is 6 c is 0.96
K1 is 4 K2 is 6 c is 0.98
K1 is 4 K2 is 7 c is 0.80
K1 is 4 K2 is 7 c is 0.82
K1 is 4 K2 is 7 c is 0.84
K1 is 4 K2 is 7 c is 0.86
K1 is 4 K2 is 7 c is 0.88
K1 is 4 K2 is 7 c is 0.9
K1 is 4 K2 is 7 c is 0.92
K1 is 4 K2 is 7 c is 0.94
K1 is 4 K2 is 7 c is 0.96
K1 is 4 K2 is 7 c is 0.98
K1 is 4 K2 is 8 c is 0.80
K1 is 4 K2 is 8 c is 0.82
K1 is 4 K2 is 8 c is 0.84
K1 is 4 K2 is 8 c is 0.86
K1 is 4 K2 is 8 c is 0.88
K1 is 4 K2 is 8 c is 0.9
K1 is 4 K2 is 8 c is 0.92
K1 is 4 K2 is 8 c is 0.94
K1 is 4 K2 is 8 c is 0.96
K1 is 4 K2 is 8 c is 0.98
K1 is 5 K2 is 4 c is 0.80
K1 is 5 K2 is 4 c is 0.82
K1 is 5 K2 is 4 c is 0.84
K1 is 5 K2 is 4 c is 0.86
K1 is 5 K2 is 4 c is 0.88
K1 is 5 K2 is 4 c is 0.9
K1 is 5 K2 is 4 c is 0.92
K1 is 5 K2 is 4 c is 0.94
K1 is 5 K2 is 4 c is 0.96
K1 is 5 K2 is 4 c is 0.98
K1 is 5 K2 is 5 c is 0.80
K1 is 5 K2 is 5 c is 0.82
K1 is 5 K2 is 5 c is 0.84
K1 is 5 K2 is 5 c is 0.86
K1 is 5 K2 is 5 c is 0.88
K1 is 5 K2 is 5 c is 0.9
K1 is 5 K2 is 5 c is 0.92
K1 is 5 K2 is 5 c is 0.94
K1 is 5 K2 is 5 c is 0.96
K1 is 5 K2 is 5 c is 0.98
K1 is 5 K2 is 6 c is 0.80
K1 is 5 K2 is 6 c is 0.82
K1 is 5 K2 is 6 c is 0.84
K1 is 5 K2 is 6 c is 0.86
K1 is 5 K2 is 6 c is 0.88
K1 is 5 K2 is 6 c is 0.9
K1 is 5 K2 is 6 c is 0.92
K1 is 5 K2 is 6 c is 0.94
K1 is 5 K2 is 6 c is 0.96
K1 is 5 K2 is 6 c is 0.98
K1 is 5 K2 is 7 c is 0.80
K1 is 5 K2 is 7 c is 0.82
K1 is 5 K2 is 7 c is 0.84
K1 is 5 K2 is 7 c is 0.86
K1 is 5 K2 is 7 c is 0.88
K1 is 5 K2 is 7 c is 0.9
K1 is 5 K2 is 7 c is 0.92
K1 is 5 K2 is 7 c is 0.94
K1 is 5 K2 is 7 c is 0.96
K1 is 5 K2 is 7 c is 0.98
K1 is 5 K2 is 8 c is 0.80
K1 is 5 K2 is 8 c is 0.82
K1 is 5 K2 is 8 c is 0.84
K1 is 5 K2 is 8 c is 0.86
K1 is 5 K2 is 8 c is 0.88
K1 is 5 K2 is 8 c is 0.9
K1 is 5 K2 is 8 c is 0.92
K1 is 5 K2 is 8 c is 0.94
K1 is 5 K2 is 8 c is 0.96
K1 is 5 K2 is 8 c is 0.98
K1 is 6 K2 is 4 c is 0.80
K1 is 6 K2 is 4 c is 0.82
K1 is 6 K2 is 4 c is 0.84
K1 is 6 K2 is 4 c is 0.86
K1 is 6 K2 is 4 c is 0.88
K1 is 6 K2 is 4 c is 0.9
K1 is 6 K2 is 4 c is 0.92
K1 is 6 K2 is 4 c is 0.94
K1 is 6 K2 is 4 c is 0.96
K1 is 6 K2 is 4 c is 0.98
K1 is 6 K2 is 5 c is 0.80
K1 is 6 K2 is 5 c is 0.82
K1 is 6 K2 is 5 c is 0.84
K1 is 6 K2 is 5 c is 0.86
K1 is 6 K2 is 5 c is 0.88
K1 is 6 K2 is 5 c is 0.9
K1 is 6 K2 is 5 c is 0.92
K1 is 6 K2 is 5 c is 0.94
K1 is 6 K2 is 5 c is 0.96
K1 is 6 K2 is 5 c is 0.98
K1 is 6 K2 is 6 c is 0.80
K1 is 6 K2 is 6 c is 0.82
K1 is 6 K2 is 6 c is 0.84
K1 is 6 K2 is 6 c is 0.86
K1 is 6 K2 is 6 c is 0.88
K1 is 6 K2 is 6 c is 0.9
K1 is 6 K2 is 6 c is 0.92
K1 is 6 K2 is 6 c is 0.94
K1 is 6 K2 is 6 c is 0.96
K1 is 6 K2 is 6 c is 0.98
K1 is 6 K2 is 7 c is 0.80
K1 is 6 K2 is 7 c is 0.82
K1 is 6 K2 is 7 c is 0.84
K1 is 6 K2 is 7 c is 0.86
K1 is 6 K2 is 7 c is 0.88
K1 is 6 K2 is 7 c is 0.9
K1 is 6 K2 is 7 c is 0.92
K1 is 6 K2 is 7 c is 0.94
K1 is 6 K2 is 7 c is 0.96
K1 is 6 K2 is 7 c is 0.98
K1 is 6 K2 is 8 c is 0.80
K1 is 6 K2 is 8 c is 0.82
K1 is 6 K2 is 8 c is 0.84
K1 is 6 K2 is 8 c is 0.86
K1 is 6 K2 is 8 c is 0.88
K1 is 6 K2 is 8 c is 0.9
K1 is 6 K2 is 8 c is 0.92
K1 is 6 K2 is 8 c is 0.94
K1 is 6 K2 is 8 c is 0.96
K1 is 6 K2 is 8 c is 0.98
K1 is 7 K2 is 4 c is 0.80
K1 is 7 K2 is 4 c is 0.82
K1 is 7 K2 is 4 c is 0.84
K1 is 7 K2 is 4 c is 0.86
K1 is 7 K2 is 4 c is 0.88
K1 is 7 K2 is 4 c is 0.9
K1 is 7 K2 is 4 c is 0.92
K1 is 7 K2 is 4 c is 0.94
K1 is 7 K2 is 4 c is 0.96
K1 is 7 K2 is 4 c is 0.98
K1 is 7 K2 is 5 c is 0.80
K1 is 7 K2 is 5 c is 0.82
K1 is 7 K2 is 5 c is 0.84
K1 is 7 K2 is 5 c is 0.86
K1 is 7 K2 is 5 c is 0.88
K1 is 7 K2 is 5 c is 0.9
K1 is 7 K2 is 5 c is 0.92
K1 is 7 K2 is 5 c is 0.94
K1 is 7 K2 is 5 c is 0.96
K1 is 7 K2 is 5 c is 0.98
K1 is 7 K2 is 6 c is 0.80
K1 is 7 K2 is 6 c is 0.82
K1 is 7 K2 is 6 c is 0.84
K1 is 7 K2 is 6 c is 0.86
K1 is 7 K2 is 6 c is 0.88
K1 is 7 K2 is 6 c is 0.9
K1 is 7 K2 is 6 c is 0.92
K1 is 7 K2 is 6 c is 0.94
K1 is 7 K2 is 6 c is 0.96
K1 is 7 K2 is 6 c is 0.98
K1 is 7 K2 is 7 c is 0.80
K1 is 7 K2 is 7 c is 0.82
K1 is 7 K2 is 7 c is 0.84
K1 is 7 K2 is 7 c is 0.86
K1 is 7 K2 is 7 c is 0.88
K1 is 7 K2 is 7 c is 0.9
K1 is 7 K2 is 7 c is 0.92
K1 is 7 K2 is 7 c is 0.94
K1 is 7 K2 is 7 c is 0.96
K1 is 7 K2 is 7 c is 0.98
K1 is 7 K2 is 8 c is 0.80
K1 is 7 K2 is 8 c is 0.82
K1 is 7 K2 is 8 c is 0.84
K1 is 7 K2 is 8 c is 0.86
K1 is 7 K2 is 8 c is 0.88
K1 is 7 K2 is 8 c is 0.9
K1 is 7 K2 is 8 c is 0.92
K1 is 7 K2 is 8 c is 0.94
K1 is 7 K2 is 8 c is 0.96
K1 is 7 K2 is 8 c is 0.98
K1 is 8 K2 is 4 c is 0.80
K1 is 8 K2 is 4 c is 0.82
K1 is 8 K2 is 4 c is 0.84
K1 is 8 K2 is 4 c is 0.86
K1 is 8 K2 is 4 c is 0.88
K1 is 8 K2 is 4 c is 0.9
K1 is 8 K2 is 4 c is 0.92
K1 is 8 K2 is 4 c is 0.94
K1 is 8 K2 is 4 c is 0.96
K1 is 8 K2 is 4 c is 0.98
K1 is 8 K2 is 5 c is 0.80
K1 is 8 K2 is 5 c is 0.82
K1 is 8 K2 is 5 c is 0.84
K1 is 8 K2 is 5 c is 0.86
K1 is 8 K2 is 5 c is 0.88
K1 is 8 K2 is 5 c is 0.9
K1 is 8 K2 is 5 c is 0.92
K1 is 8 K2 is 5 c is 0.94
K1 is 8 K2 is 5 c is 0.96
K1 is 8 K2 is 5 c is 0.98
K1 is 8 K2 is 6 c is 0.80
K1 is 8 K2 is 6 c is 0.82
K1 is 8 K2 is 6 c is 0.84
K1 is 8 K2 is 6 c is 0.86
K1 is 8 K2 is 6 c is 0.88
K1 is 8 K2 is 6 c is 0.9
K1 is 8 K2 is 6 c is 0.92
K1 is 8 K2 is 6 c is 0.94
K1 is 8 K2 is 6 c is 0.96
K1 is 8 K2 is 6 c is 0.98
K1 is 8 K2 is 7 c is 0.80
K1 is 8 K2 is 7 c is 0.82
K1 is 8 K2 is 7 c is 0.84
K1 is 8 K2 is 7 c is 0.86
K1 is 8 K2 is 7 c is 0.88
K1 is 8 K2 is 7 c is 0.9
K1 is 8 K2 is 7 c is 0.92
K1 is 8 K2 is 7 c is 0.94
K1 is 8 K2 is 7 c is 0.96
K1 is 8 K2 is 7 c is 0.98
K1 is 8 K2 is 8 c is 0.80
K1 is 8 K2 is 8 c is 0.82
K1 is 8 K2 is 8 c is 0.84
K1 is 8 K2 is 8 c is 0.86
K1 is 8 K2 is 8 c is 0.88
K1 is 8 K2 is 8 c is 0.9
K1 is 8 K2 is 8 c is 0.92
K1 is 8 K2 is 8 c is 0.94
K1 is 8 K2 is 8 c is 0.96
K1 is 8 K2 is 8 c is 0.98


                                         Histogram of number of reference contigs

  200 ++--------------+--------------+---------------+---------------+---------------+--------------+--------------++
      +               +              +               +       'plot.kopt.data' using (bin($1,binwidth)):(1.0)*********
  180 ++                                                                                            *              +*
      |                                                                                             *               *
      |                                                                                             *               *
  160 ++                                                                                            *              +*
      |                                                                                             *               *
  140 ++                                                                                            *              +*
      |                                                                                             *               *
  120 ++                                                                                            *              +*
      |                                                                                             *               *
  100 ++                                                                                            *              +*
      |                                                                                             *               *
      |                                                                                             *               *
   80 ++                                                                                            *              +*
      |                                                                                             *               *
   60 ++                                                                                            *              +*
      |                                                                                             *               *
   40 ++                                             ************************************************              +*
      |                                              *                                              *               *
      |                                              *                                              *               *
   20 ++                                             *                                              *              +*
      ************************************************               +               +              *               *
    0 ***************************************************************************************************************
     988             990            992             994             996             998            1000            1002
                                                Number of reference contigs

Average contig number = 999.452
The top three most common number of contigs
X	Contig number
164	1000
19	998
18	999
The top three most common number of contigs (with values rounded)
X	Contig number
250	1000.0`

Finally, I viewed the output of kopt.data

`$ cat kopt.data
4 4 0.80 1000
4 4 0.82 1000
4 4 0.84 1000
4 4 0.86 1000
4 4 0.88 1000
4 4 0.9 1000
4 4 0.92 1001
4 4 0.94 1001
4 4 0.96 1001
4 4 0.98 1004
4 5 0.80 1000
4 5 0.82 1000
4 5 0.84 1000
4 5 0.86 1000
4 5 0.88 1000
4 5 0.9 1000
4 5 0.92 1000
4 5 0.94 1000
4 5 0.96 1000
4 5 0.98 1002
4 6 0.80 1000
4 6 0.82 1000
4 6 0.84 1000
4 6 0.86 1000
4 6 0.88 1000
4 6 0.9 1000
4 6 0.92 1000
4 6 0.94 1000
4 6 0.96 1000
4 6 0.98 1002
4 7 0.80 1000
4 7 0.82 1000
4 7 0.84 1000
4 7 0.86 1000
4 7 0.88 1000
4 7 0.9 1000
4 7 0.92 1000
4 7 0.94 1000
4 7 0.96 1000
4 7 0.98 1002
4 8 0.80 1000
4 8 0.82 1000
4 8 0.84 1000
4 8 0.86 1000
4 8 0.88 1000
4 8 0.9 1000
4 8 0.92 1000
4 8 0.94 1000
4 8 0.96 1000
4 8 0.98 1002
5 4 0.80 1000
5 4 0.82 1000
5 4 0.84 1000
5 4 0.86 1000
5 4 0.88 1000
5 4 0.9 1000
5 4 0.92 1001
5 4 0.94 1001
5 4 0.96 1001
5 4 0.98 1004
5 5 0.80 1000
5 5 0.82 1000
5 5 0.84 1000
5 5 0.86 1000
5 5 0.88 1000
5 5 0.9 1000
5 5 0.92 1000
5 5 0.94 1000
5 5 0.96 1000
5 5 0.98 1002
5 6 0.80 1000
5 6 0.82 1000
5 6 0.84 1000
5 6 0.86 1000
5 6 0.88 1000
5 6 0.9 1000
5 6 0.92 1000
5 6 0.94 1000
5 6 0.96 1000
5 6 0.98 1002
5 7 0.80 1000
5 7 0.82 1000
5 7 0.84 1000
5 7 0.86 1000
5 7 0.88 1000
5 7 0.9 1000
5 7 0.92 1000
5 7 0.94 1000
5 7 0.96 1000
5 7 0.98 1002
5 8 0.80 999
5 8 0.82 999
5 8 0.84 999
5 8 0.86 999
5 8 0.88 999
5 8 0.9 999
5 8 0.92 999
5 8 0.94 999
5 8 0.96 999
5 8 0.98 1001
6 4 0.80 1000
6 4 0.82 1000
6 4 0.84 1000
6 4 0.86 1000
6 4 0.88 1000
6 4 0.9 1000
6 4 0.92 1001
6 4 0.94 1001
6 4 0.96 1001
6 4 0.98 1004
6 5 0.80 1000
6 5 0.82 1000
6 5 0.84 1000
6 5 0.86 1000
6 5 0.88 1000
6 5 0.9 1000
6 5 0.92 1000
6 5 0.94 1000
6 5 0.96 1000
6 5 0.98 1002
6 6 0.80 1000
6 6 0.82 1000
6 6 0.84 1000
6 6 0.86 1000
6 6 0.88 1000
6 6 0.9 1000
6 6 0.92 1000
6 6 0.94 1000
6 6 0.96 1000
6 6 0.98 1002
6 7 0.80 1000
6 7 0.82 1000
6 7 0.84 1000
6 7 0.86 1000
6 7 0.88 1000
6 7 0.9 1000
6 7 0.92 1000
6 7 0.94 1000
6 7 0.96 1000
6 7 0.98 1002
6 8 0.80 999
6 8 0.82 999
6 8 0.84 999
6 8 0.86 999
6 8 0.88 999
6 8 0.9 999
6 8 0.92 999
6 8 0.94 999
6 8 0.96 999
6 8 0.98 1001
7 4 0.80 1000
7 4 0.82 1000
7 4 0.84 1000
7 4 0.86 1000
7 4 0.88 1000
7 4 0.9 1000
7 4 0.92 1000
7 4 0.94 1000
7 4 0.96 1000
7 4 0.98 1002
7 5 0.80 1000
7 5 0.82 1000
7 5 0.84 1000
7 5 0.86 1000
7 5 0.88 1000
7 5 0.9 1000
7 5 0.92 1000
7 5 0.94 1000
7 5 0.96 1000
7 5 0.98 1002
7 6 0.80 1000
7 6 0.82 1000
7 6 0.84 1000
7 6 0.86 1000
7 6 0.88 1000
7 6 0.9 1000
7 6 0.92 1000
7 6 0.94 1000
7 6 0.96 1000
7 6 0.98 1002
7 7 0.80 1000
7 7 0.82 1000
7 7 0.84 1000
7 7 0.86 1000
7 7 0.88 1000
7 7 0.9 1000
7 7 0.92 1000
7 7 0.94 1000
7 7 0.96 1000
7 7 0.98 1002
7 8 0.80 998
7 8 0.82 998
7 8 0.84 998
7 8 0.86 998
7 8 0.88 998
7 8 0.9 998
7 8 0.92 998
7 8 0.94 998
7 8 0.96 998
7 8 0.98 1000
8 4 0.80 1000
8 4 0.82 1000
8 4 0.84 1000
8 4 0.86 1000
8 4 0.88 1000
8 4 0.9 1000
8 4 0.92 1000
8 4 0.94 1000
8 4 0.96 1000
8 4 0.98 1002
8 5 0.80 1000
8 5 0.82 1000
8 5 0.84 1000
8 5 0.86 1000
8 5 0.88 1000
8 5 0.9 1000
8 5 0.92 1000
8 5 0.94 1000
8 5 0.96 1000
8 5 0.98 1002
8 6 0.80 998
8 6 0.82 998
8 6 0.84 998
8 6 0.86 998
8 6 0.88 998
8 6 0.9 998
8 6 0.92 998
8 6 0.94 998
8 6 0.96 998
8 6 0.98 1000
8 7 0.80 997
8 7 0.82 997
8 7 0.84 997
8 7 0.86 997
8 7 0.88 997
8 7 0.9 997
8 7 0.92 997
8 7 0.94 997
8 7 0.96 997
8 7 0.98 998
8 8 0.80 989
8 8 0.82 989
8 8 0.84 989
8 8 0.86 989
8 8 0.88 989
8 8 0.9 989
8 8 0.92 989
8 8 0.94 989
8 8 0.96 989
8 8 0.98 990`



