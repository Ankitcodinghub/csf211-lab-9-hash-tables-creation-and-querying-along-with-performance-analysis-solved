# csf211-lab-9-hash-tables-creation-and-querying-along-with-performance-analysis-solved
**TO GET THIS SOLUTION VISIT:** [CSF211 Lab 9-Hash tables: Creation and Querying along with performance analysis Solved](https://www.ankitcodinghub.com/product/csf211-lab-9-hash-tables-creation-and-querying-along-with-performance-analysis-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91915&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSF211 Lab 9-Hash tables: Creation and Querying along with performance analysis Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Lab IX ==========================================

Topics: Hash tables: Creation and Querying along with performance analysis

Hash tables are used for faster querying on large datasets. Their creation and querying

performance depends upon many factors including size of hash table and hashing function.

Exercise 1: Identification of best hash function for a given input domain

<ol>
<li>a) &nbsp;Hash function: Implement a hash function which takes a string, a baseNumber, and a tableSize variables as inputs and returns a number in range [0, tableSize). Hashing
should be done as:

= (((sum of ASCII values of characters in string) mod baseNumber) mod tableSize)
</li>
<li>b) &nbsp;Collision count: A collision is said to occur whenever two inputs are mapped to same value by the hash function. Implement a function which takes an array of strings, a baseNumber, and a tableSize as inputs. It should call the hash function in 1(a) for all the strings in input array and return the number of times collision will occur if the given hash function is used for hashing.</li>
<li>c) &nbsp;Parsing: Implement an input parser which reads a text file in UTF-8 format and returns an array of all strings in the file which follows certain rule. For now, assume that the rule is, “Any white space separated sequence of only English characters”. Use the provided “Project Gutenberg’s Alice’s Adventures in Wonderland, by Lewis Carroll” file as the test case. The function should also print the total number of valid strings before returning the array of strings (let’s call it, book).</li>
</ol>
d) Profiling: Assuming that the metric for selection of best hash function is the one with minimal collisions, implement a function to identify the best value of baseNumber and tableSize from following range of parameters, for the book (input array of strings returned from parser in 1(c)):

<ol>
<li>Possible choices for baseNumber: 3 prime numbers between tableSize and 2*tableSize and 3 prime numbers larger than 1000*tableSize (6 choices, hardcoding allowed)</li>
<li>Possible choices for tableSize: 5000, 50000, and 500000 (3 choices, hardcoding allowed)</li>
</ol>
Implement the profiling function such that it prints the collision values of all 18 choices and then prints the indices of best parameters in baseNumbers and tableSize arrays.

Exercise 2: Creating and using a hash table

One of the strategies to create a hash table is with separate chaining such that collided values are inserted at the end of list. A hash table may additionally store a few fields with it, like:

<ul>
<li> &nbsp;elementCount: total number of elements (strings) in the table</li>
<li> &nbsp;insertionCost: total number of jumps done in any of the lists (chains) to insert the
element at the end. Increment only in case of collision.
</li>
<li> &nbsp;queryingCost: total number of comparisons done in any of the chains during all lookups</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Notes:

<ol>
<li>Implement the chain as a linked list of records containing:
a. The index of the first occurrence of the string in the book array (i.e. there should be only one copy of each string, even if there are multiple occurrences).

b. The count of occurrences of that string
</li>
<li>Also, hard code the hash function to use best values of baseNumber and tableSize
and only take a string as input.
</li>
</ol>
End of notes.

<ol>
<li>a) &nbsp;Creation: Implement a function to create an empty hash table with best value of tableSize returned from Exercise 1(d). All the fields of hash table should be appropriately initialized.</li>
<li>b) &nbsp;Insert: Implement a function which takes a hash table, an array of strings, say A, an index into the array, say j, and:</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
 

</div>
<div class="column">
inserts the string at given index i.e. A[j] in the hash table if the string at Aj] is not present;

update the count if it is already present

Note that only the index and count are stored in the Hashtable. i.e. if index=5 andbook[5] contains the first occurrence of the string “alice”, then the value 5 should be added in the hash table in the chain identified by hashing “alice” along with a count of 1. If index = 237 and book[237] contains a subsequent occurrence of “alice” then the count of the record – already inserted in the hashtable – should be incremented. It should also update insertionCost variableofthehashtable.Anynewvalueshouldbeinsertedat the end of chain.

</div>
</div>
<div class="layoutArea">
<div class="column">
c) InsertAll: Implement a function which inserts all strings of the book array in an empty hash table passed as argument. Once all values are inserted return the value of insertionCost.

<ol start="4">
<li>d) &nbsp;Lookup: Implement a function to take a hash table and a string as input and return the corresponding record. It should also update queryingCost.</li>
<li>e) &nbsp;LookupAll: Implement a function to take a hash table, an array of strings and a real numberm asinput.Itshouldlookupallstringsinthegivenhashtablewhichappearin firstm% indicesofthearrayofstrings.E.g.m = 0.05 shouldtriggerqueryingoffirst 5% entries of the input array to be looked up in the given hash table. It should reset queryingCost in the beginning and return it in the end.</li>
</ol>
Exercise 3: Profiling and Optimizing hash table for an input domain

a) Profiling: Implement a function which calls LookupAll with varying number of percentages from 10% to 200% with a step of 10%, to determine the percentage where queryingCost overtakes insertionCost for this input book and the given

parameters.

Cleanup: Given a list of stop words (given in a separate file), delete all entries of stop words from the hashtable. Call profiling function on the updated hash table to identify the percentage where queryingCost overtakes insertionCost for this input book and the given parameters.

Solution to be uploaded as a part of this lab: Solve Exercise-2 and upload its solution. It is required to implement all the functions in a single file, named as YOUR_BITS_ID.c

No need to upload executable files, just upload a single .c file.

</div>
</div>
</div>
