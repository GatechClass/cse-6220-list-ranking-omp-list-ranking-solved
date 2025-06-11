# cse-6220-list-ranking-omp-list-ranking-solved
**TO GET THIS SOLUTION VISIT:** [CSE 6220 List Ranking OMP List Ranking Solved](https://mantutor.com/product/cse-6220-list-ranking-omp-list-ranking-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top kksr-disabled" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;26708&quot;,&quot;readonly&quot;:&quot;1&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE 6220 List Ranking OMP List Ranking Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
In this lab, you will implement Wyllie’s list ranking algorithm as discussed in the videos, plus another algorithm due to Helman and Jaja. The efficiency of your code will be compared to a reference implementation to help determine your grade.

## Getting Started

Begin by obtaining the starter code from the github repository.

&lt;pre&gt;&lt;code&gt;

git clone –recursive https://github.gatech.edu/omscse6220/lab1.git

&lt;/code&gt;&lt;/pre&gt;

Optionally, you may choose use a git hosting service for your code. As always, please **do not make your repository public** on Github or another git hosting service. Anyone will be able to see it. If you feel the need to use a hosting service for your project, please keep your repository private. Your GT account allows you to create free private repositories on [the GT github server](https:github.gatech.edu).

## Programming

You should only modify the function contents in listrank_wyllie.c and listrank_hj.c. Do not modify any other files, and do not modify the function signature. You may add helper functions to be used inside listrank_wyllie.c and listrank_hj.c.

&lt;!–

First implement the parallel list ranking algorithms using Cilk Plus, an extension of C++ and C for shared memory parallel applications. Cilk Plus is available on Intel compilers and GCC 5.2.0. There is a wealth of documentation about Cilk Plus online. Here are a few resources to help you get started:

* [cilkplus.org](https://www.cilkplus.org/)

* [Wikipedia](https://en.wikipedia.org/wiki/Cilk)

* [Cilk Plus Tutorial](https://www.cilkplus.org/cilk-plus-tutorial)

You should allow Cilk Plus to decide how many threads are available rather than choosing for yourself. Thus, for example, using ‘cilk_for’ should not entail tuning the number of iterations.

–&gt;

First implement the parallel list ranking algorithms using OpenMP, an API for shared memory parallel applications. (Intel’s Cilk is a popular competitor in this category.) There is a wealth of documentation about OpenMP online. Here are a few resources to help you get started

* [LLNL](https://computing.llnl.gov/tutorials/openMP/)

* [Wikipedia](https://en.wikipedia.org/wiki/OpenMP)

* [OpenMP.org](http://openmp.org/wp/resources/)

You should allow OpenMP to decide how many threads are available rather than choosing for yourself. Thus, a simple

&lt;pre&gt;&lt;code&gt;

#pragma omp parallel

&lt;/code&gt;&lt;/pre&gt;

directive will be sufficient for the purposes of this lab.

Your first task is to implement Wyllie’s algorithm, which is described in the lesson videos, in the file listrank_wyllie.c.

Next, you are to implement the Helman-Jaja algorithm for list ranking in the listrank_hj.c file. You should be able to use your GT credentials to access the [the original paper](http://link.springer.com.prx.library.gatech.edu/chapter/10.1007/3-540-48518-X_3) via the GT library, though you may find that the summary below is sufficient.

1. Sequentially, partition the input list into *s* sublists, by randomly choosing *s* sublist head nodes.

2. In parallel, traverse each sublist computing the list ranking of each node within the sublists.

3. Sequentially, compute the list ranking of the head nodes overall (by doing a prefix sum of the head node ranks).

4. In parallel, traverse the sublists again to convert the sublist ranking to the complete list ranking (by adding the previously determined prefix sum values).

### Compilation

In addition to the starter code discussed above, the repository also contains a number of other files to help you test and measure the performance of your code. The file correctness.c contains a simple test to see if your code is correct. By default, the Makefile will compile the file listrank_wyllie.c. To have it compile listrank_hj.c instead, use the command

&lt;pre&gt;&lt;code&gt;

make correctness IMPL=hj

&lt;/code&gt;&lt;/pre&gt;

Note that the value for the variable IMPL given on the command line overrides the one given in the Makefile.

### Performance Testing

You should measure the performance of your code on the PACE cluster. The main file metrics.c performs some the same tests on which your code will be evaluated. Use the IMPL command line parameter to change which implementation of the parallelListRanks is compiled. Thus, if you wanted to time your Helman-Jaja algorithm, you might implement it in a file listrank_hj.c and compile it with

&lt;pre&gt;&lt;code&gt;

make metrics IMPL=hj

&lt;/code&gt;&lt;/pre&gt;

The file timing_hj.sub serves as an example for how to use qsub for the Helman-Jaja algorithm. Thus, to measure the performance of you code you should run

&lt;pre&gt;&lt;code&gt;

qsub timing_hj.pbs

&lt;/code&gt;&lt;/pre&gt;

from your PACE login node.

### Sample Performance Values

&gt; Note: You can use the timing_serial.pbs job to acquire the serial reference point.

You can see the speedup based on median values of timings on PACE. With the Wyllie algorithm, you should expect speedups of around 0.2 or greater (slowdowns) for array sizes of 1e6 and 1e7. With the Helman-Jaja algorithm, you can obtain speedups greater than 5 for array sizes of 1e6 and 1e7.

### Submitting Your Code

&gt; Note: As a reminder, the deliverables for this lab are listrank_wyllie.c and listrank_hj.c.

Once you have completed and tested your implementations, please submit using the **submit.py** script,

&lt;pre&gt;&lt;code&gt;

python submit.py

&lt;/code&gt;&lt;/pre&gt;

which will do a quick correctness test. You may submit as many times as you like before the deadline. At the deadline, the TA will download the code and perform some timing runs. These results along with a manual inspection of the code will determine your grade.
