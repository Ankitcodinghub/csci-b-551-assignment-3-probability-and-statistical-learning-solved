# csci-b-551-assignment-3-probability-and-statistical-learning-solved
**TO GET THIS SOLUTION VISIT:** [CSCI-B-551 Assignment 3-Probability and Statistical Learning Solved](https://www.ankitcodinghub.com/product/csci-b-551-assignment-3-probability-and-statistical-learning-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91830&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI-B-551 Assignment 3-Probability and Statistical Learning Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Part 0: Getting started

We’ve assigned you to a team; find it as usual by logging into IU Github, look for a repo called userid1-a3, userid1-userid2-a3, or userid1-userid2-userid3-a3, where the other user ID(s) correspond to your team- mate(s). Now that you know their userid(s), you can write them an email at userid@iu.edu. To get started, clone the github repository using one of the two commands:

git clone git@github.iu.edu:cs-b551-fa2021/your-repo-name-a3 git clone https://github.iu.edu/cs-b551-fa2021/your-repo-name-a3

Part 1: Part-of-speech tagging

A basic problems in Natural Language Processing is part-of-speech tagging, in which the goal is to mark every word in a sentence with its part of speech (noun, verb, adjective, etc.). Sometimes this is easy: a sentence like “Blueberries are blue” clearly consists of a noun, verb, and adjective, since each of these words has only one possible part of speech (e.g., “blueberries” is a noun but can’t be a verb).

But in general, one has to look at all the words in a sentence to figure out the part of speech of any individual word. For example, consider the — grammatically correct! — sentence: “Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo.” To figure out what it means, we can parse its parts of speech:

Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo. Adjective Noun Adjective Noun Verb Verb Adjective Noun

(In other words: the buffalo living in Buffalo, NY that are buffaloed (intimidated) by buffalo living in Buffalo, NY buffalo (intimidate) buffalo living in Buffalo, NY.)

That’s an extreme example, obviously. Here’s a more mundane sentence:

Her position covers a number of daily tasks common to any social director. DET NOUN VERB DET NOUN ADP ADJ NOUN ADJ ADP DET ADJ NOUN

where DET stands for a determiner, ADP is an adposition, ADJ is an adjective, and ADV is an adverb.1 Many of these words can be different parts of speech: “position” and “covers” can both be nouns or verbs, for example, and the only way to resolve the ambiguity is to look at the surrounding words. Labeling parts of speech thus involves an understanding of the intended meaning of the words in the sentence, as well as the relationships between the words.

Fortunately, statistical models work amazingly well for NLP problems. Consider the Bayes net shown in Figure 1(a). This Bayes net has random variables S = {S1,…,SN} and W = {W1,…,WN}. The W’s represent observed words in a sentence. The S’s represent part of speech tags, so Si ∈ {VERB, NOUN, . . .}. The arrows between W and S nodes model the relationship between a given observed word and the possible parts of speech it can take on, P(Wi|Si). (For example, these distributions can model the fact that the word “dog” is a fairly common noun but a very rare verb.) The arrows between S nodes model the probability that a word of one part of speech follows a word of another part of speech, P(Si+1|Si). (For example, these arrows can model the fact that verbs are very likely to follow nouns, but are unlikely to follow adjectives.)

Data. To help you with this assignment, we’ve prepared a large corpus of labeled training and testing data. Each line consists of a sentence, and each word is followed by one of 12 part-of-speech tags: ADJ (adjective), ADV (adverb), ADP (adposition), CONJ (conjunction), DET (determiner), NOUN, NUM (number), PRON (pronoun), PRT (particle), VERB, X (foreign word), and . (punctuation mark).2

1If you didn’t know the term “adposition”, neither did I. The adpositions in English are prepositions; in many languages, there are postpositions too. But you won’t need to understand the linguistic theory between these parts of speech to complete the assignment; if you’re curious, check out the “Part of Speech” Wikipedia article for some background.

2This dataset is based on the Brown corpus. Modern part-of-speech taggers often use a much larger set of tags – often over 2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
S1 S2 S3 S4 … SN

W1 W2 W3 W4 WN

</div>
</div>
<div class="layoutArea">
<div class="column">
S1 S2 S3 S4

W1 W2 W3 W4

(b)

</div>
<div class="column">
… SN

WN

</div>
</div>
<div class="layoutArea">
<div class="column">
(a)

</div>
<div class="column">
(c)

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 1: Bayes Nets for part of speech tagging: (a) HMM, and (b) simplified model, and (c) complicated model.

What to do. Your goal in this part is to implement part-of-speech tagging in Python, using Bayes networks.

<ol>
<li>To get started, consider the simplified Bayes net in Figure 1(b). To perform part-of-speech tagging,we’ll want to estimate the most-probable tag s∗i for each word Wi, s∗i = argmaxP(Si = si|W).
si Implement part-of-speech tagging using this simple model.
</li>
<li>Now consider Figure 1(a), a richer Bayes net that incorporates dependencies between words. Implement Viterbi to find the maximum a posteriori (MAP) labeling for the sentence,(s∗1,…,s∗N) = arg max P(Si = si|W). s1 ,…,sN</li>
<li>Consider the Bayes Net of Figure 1c, which could be a better model because it incorporates richer dependencies between words. But it’s not an HMM, so we can’t use Viterbi. Implement Gibbs Sampling to sample from the posterior distribution of Fig 1c, P(S|W). Then estimate the best labeling for each</li>
</ol>
word (by picking the maximum marginal for each word, s∗i = arg maxsi P (Si = si |W ). (To do this, just generate many (thousands?) of samples and, for each individual word, check which part of speech occurred most often.)

Your program should take as input a training filename and a testing filename. The program should use the training corpus to estimate parameters, and then display the output of Steps 1-3 on each sentence in the testing file. For the result generated by each of the three approaches (Simple, HMM, Complex), as well as for the ground truth result, your program should output the logarithm of the joint probability P (S, W ) for each solution it finds under each of the three models in Figure 1. It should also display a running evaluation showing the percentage of words and whole sentences that have been labeled correctly so far. For example:

<pre>[djcran@raichu djc-sol]$ python3 ./label.py training_file testing_file
Learning model...
Loading test data...
Testing classifiers...
</pre>
<pre>                      Simple     HMM  Complex  Magnus     ab integro seclorum nascitur  ordo .
  0. Ground truth     -48.52  -64.33   -73.43    noun   verb     adv     conj     noun  noun .
    1. Simplified     -47.29  -66.74   -75.29    noun   noun    noun      adv     verb  noun .
           2. HMM     -47.48  -63.83   -74.12    noun   verb     adj     conj     noun  verb .
    3.    Complex     -47.50  -64.21   -72.02    noun   verb     adv     conj     noun  noun .
</pre>
<pre>==&gt; So far scored 1 sentences with 17 words.
</pre>
100 tags, depending on the language of interest – that carry finer-grained information like the tense and mood of verbs, whether nouns are singular or plural, etc. In this assignment we’ve simplified the set of tags to the 12 described here; the simple tag set is due to Petrov, Das and McDonald, and is discussed in detail in their 2012 LREC paper if you’re interested.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
<pre>0. Ground truth
  1. Simplified
         2. HMM
     3. Complex
</pre>
</div>
<div class="column">
<pre>Words correct:
      100.00%
       42.85%
       71.43%
      100.00%
</pre>
</div>
<div class="column">
<pre>Sentences correct:
        100.00%
</pre>
0.00%

<pre>          0.00%
        100.00%
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
We’ve already implemented some skeleton code to get you started, in three files: label.py, which is the main program, pos scorer.py, which has the scoring code, and pos solver.py, which will contain the actual part-of-speech estimation code. You should only modify the latter of these files; the current version of pos solver.py we’ve supplied is very simple, as you’ll see. In your report, please make sure to include your results (accuracies) for each technique on the test file we’ve supplied, bc.test. Your code should finish within about 10 minutes.

Part 2: Ice tracking

In this problem, we’ll help solve global warming. 🙂

To understand how rising global temperatures affect ice at the Earth’s north and south poles, glaciologists need information about the structure of the ice sheets. The traditional way of doing this is to drill into the ice and remove an ice core. But a single ice core can take many months to drill, and only gives information about the ice at a single latitude-longitude point. To expedite this process, scientists have developed radar systems that allow an airplane to collect an approximate “cross section” of the ice below the airplane’s flight path (Fig 2a). This produces a radar echogram like the one shown in Fig 2b. The horizontal axis is the distance along the flight path, while the vertical axis is the depth below the plane. The echogram shows two prominent features. One is the very dark line near the top, which is the boundary between the air and the ice. There’s also a deeper line which shows the boundary between the ice and the bedrock. Fig 2c shows the same echogram but with the air-ice (red) and ice-rock (green) boundaries manually labeled. These echograms reveal the complex structure of the ice — note the ridges and valleys in the bedrock in Fig 2c, for example — and contain rich information for glaciologists to calculate volumes of ice and to estimate how it will change with warming temperatures. But as you can see from the figure, these echograms are also extremely noisy, so finding the layer boundaries is quite challenging. Even human experts, when presented with the same echogram, often disagree on where the boundaries are.

In this part, we’ll create code to try to find these two boundaries (air-ice and ice-rock). We’ll make some assumptions to make this possible. First, you can assume that the air-ice boundary is always above the ice-rock boundary by a significant margin (say, 10 pixels). Second, you can assume that the two boundaries span the entire width of the image. Taken together these, two assumptions mean that in each column of the image, there is exactly one air-ice boundary and exactly one ice-rock boundary, and the ice-rock boundary is always below. Third, we assume that each boundary is relatively “smooth” — that is, a boundary’s row in one column will be similar in the next column. Finally, you can assume that the pixels along the boundaries are generally dark and along a strong image edge (sharp change in pixel values)..

We’ve given you code that reads an image file into a two-dimensional array. For an m × n echogram, the code creates a 2-d array I(x,y) that stores the radar return at each pixel (x,y) ∈ [1,m]×[1,n] where smaller values indicate greater probability of a boundary. Your goal is to estimate, for each column x ∈ [1, m], the row ax corresponding to the air-ice boundary, and the row rx corresponding to the ice-rock boundary. (In image processing, the coordinate system convention is for the upper-left of the image to be the point (1,1), and for column indices to increase as you go right and row indices to increase as you go down.) Each of these boundaries can be solved for using a Bayes net. For example, for the air-ice problem, the Bayes net would have hidden variables a1,a2,…am, and observed variables (specifically w1,w2,…wm, where w1 is a vector corresponding to column 1 of the image).

Since the air-ice boundary is generally stronger than ice-rock and easier to estimate, it makes sense to

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
(a) (b) (c)

Figure 2: Figure 2: (a) An airplane with a ground-penetrating radar system flies along the ice, generating an echogram such as (b). The annotations in (c) show key features of the echogram.

first estimate the air-ice boundary, and then estimate the ice-rock boundary but require that it be at least (for example) 10 pixels below the air-ice boundary in each column (i.e., require that rx ≥ ax + 10 for all x ∈ [1, m]).

<ol>
<li>Perhaps the simplest technique would be to use the Bayes’ Net in Figure 1b to estimate the two boundaries. Implement this technique, showing the boundaries in yellow.(Hint: What should your emission probabilities look like? This is for you to decide, but intuitively a stronger edge and/or darker (lower) pixel value should correspond to higher probability. Our skeleton code includes a function to compute edge strength, in case this is helpful.)</li>
<li>A better approach would use the Bayes Net in Figure 1a. Use Viterbi, showing the boundaries in blue.(Hint: What should your transition probabilities look like? It’s up to you, but you probably want to use a distribution that encourages “smoothness,” i.e. that P(si+1|si) is high if si+1 = si and is low if they are very different.)</li>
<li>A simple way of improving the results further is to incorporate some human feedback. Assume that a human gives you two (x,y) points, one that is known to lie somewhere on the air-ice boundary, and one that is known to lie somewhere on the ice-rock boundary. Modify your answer to step 2 to incorporate this additional information. (Hint: you can do this by just tweaking the HMM’s probability distributions – no need to change the algorithm itself!) Show the resulting boundaries in red and the human-provided point with an asterisk (our skeleton code already does this for you).</li>
</ol>
Your program should be run like this:

<pre>   python3 ./polar.py input_file.jpg airice_row_coord airice_col_coord icerock_row_coord icerock_col_coord
</pre>
where airice row coord and airice col coord are the image row and column coordinates of the human-labeled air-ice pixel, and icerock row coord and icerock col coord are the coordinates of the human-labeled ice-rock pixel. The program should generate two files: air ice output.jpg, which should show the original image with the yellow, blue, and red lines superimposed on the echogram for the estimated air-ice layers, and ice rock output.jpg, which should show the same for the ice-rock layers.

Run your code on our sample images and please show a few sample outputs in your report.

Part 3: Reading text

To show the versatility of HMMs, let’s try applying them to another problem; if you’re careful and you plan ahead, you can probably re-use much of your code from Parts 1 and 2 to solve this problem. Our goal is to

</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
Figure 3: Our goal is to extract text from a noisy scanned image of a document.

recognize text in an image – e.g., to recognize that Figure 2 says “It is so ordered.” But the images are noisy, so any particular letter may be difficult to recognize. However, if we make the assumption that these images have English words and sentences, we can use statistical properties of the language to resolve ambiguities, just like in Part 2.

We’ll assume that all the text in our images has the same fixed-width font of the same size. In particular, each letter fits in a box that’s 16 pixels wide and 25 pixels tall. We’ll also assume that our documents only have the 26 uppercase latin characters, the 26 lowercase characters, the 10 digits, spaces, and 7 punctuation symbols, (),.-!?’”. Suppose we’re trying to recognize a text string with n characters, so we have n observed variables (the subimage corresponding to each letter) O1,…,On and n hidden variables, l1…,ln, which are the letters we want to recognize. We’re thus interested in P(l1,…,ln|O1,…,On). As in part 1, we can rewrite this using Bayes’ Law, estimate P(Oi|li) and P(li|li−1) from training data, then use probabilistic inference to estimate the posterior, in order to recognize letters.

What to do. Write a program called image2text.py that is called like this:

<pre>python3 ./image2text.py train-image-file.png train-text.txt test-image-file.png
</pre>
The program should load in the train-image-file, which contains images of letters to use for training (we’ve supplied one for you). It should also load in the text training file, which is simply some text document that is representative of the language (English, in this case) that will be recognized. (The training file from Part 1 could be a good choice). Then, it should use the classifier it has learned to detect the text in test- image-file.png, using (1) the simple Bayes net of Figure 1b and (2) the HMM of Fig 1a with MAP inference (Viterbi). The last two lines of output from your program should be these two results, as follows:

<pre>[djcran@tank]$ python3 ./image2text.py train-image-file.png train-text.txt test-image-file.png
 Simple: 1t 1s so orcerec.
</pre>
<pre>    HMM: It is so ordered.
</pre>
Hints. We’ve supplied you with skeleton code that takes care of all the image I/O for you, so you don’t have to worry about any image processing routines. The skeleton code converts the images into simple Python list-of-lists data structures that represents the characters as a 2-d grid of black and white dots. You’ll need to define an HMM and estimate its parameters from training data. The transition and initial state probabilities should be easy to estimate from the text training data. For the emission probability, we suggest using a simple naive Bayes classifier. The train-image-file.png file contains a perfect (noise-free) version of each letter. The text strings your program will encounter will have nearly these same letters, but they may be corrupted with noise. If we assume that m% of the pixels are noisy, then a naive Bayes classifier could assume that each pixel of a given noisy image of a letter will match the corresponding pixel in the reference letter with probability (100 − m)%.

</div>
</div>
</div>
