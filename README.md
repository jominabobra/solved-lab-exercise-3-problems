Download Link: https://assignmentchef.com/product/solved-lab-exercise-3-problems
<br>
<h1>Lab exercise 3 objectives</h1>

<ol>

 <li>Write C++ programs</li>

 <li>Compile C++ programs</li>

 <li>Implement programs that use <code>std::cin</code> and <code>std::cout</code> correctly</li>

 <li>Implement programs that use conditional statements</li>

</ol>

<h1><a id="user-content-instructions" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03#instructions" aria-hidden="true"></a>Instructions</h1>

Answer the programming problems sequentially (i.e., answer prob01 before prob02). If you have questions let your instructor or the lab assistant know. You can also consult your classmates.

When you answer two programming problems correctly, let your instructor know and wait for further instruction.

<h1><a id="user-content-lab-exercise-guide" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03#lab-exercise-guide" aria-hidden="true"></a>Lab exercise guide</h1>

Here’s a link to the <a href="https://docs.google.com/document/d/1EX01EtrO-pkHNLVPxiq7HNh1f5KnJZnr_dlJcO4T7t0/edit?usp=sharing" rel="nofollow">Lab exercise guide</a> in case you need to review the lab exercise objectives, grading scheme, or evaluation process.




<h1>Holideals at the Movies!</h1>

We have special movie tickets on holidays! Prices are discounted when you buy a pair of tickets.

Create a program for the HoliDeals event that computes the subtotal for a pair of tickets. The program should ask the the ages of the first and second guests to compute the price.

There are different pricing structures based on the guests’ age.

<em>Children tickets cost $10 (age below 13)</em>

<em>Young Adult tickets cost $13 (age below 21)</em>

<em>Adult tickets cost $15 (age below 65)</em>

<em>Senior tickets cost $10 (age 65 and over)</em>

To simplify the problem, let’s assume that parents/guardians will always accompany pairs of children who will watch a movie.

The pricing structure should be displayed to the user. Please see the sample output below to guide the design of your program.

<pre><code>Welcome to HoliDeals at the Movies!Tickets tonight can only be bought in pairs.Here are our movie ticket deals:Children - $10.00Young Adults - $13.00Adults - $15.00Seniors - $10.00Please enter the age of the person for the first guest: 15Please enter the age of the person for the second guest: 16The Subtotal for the ticket cost is: $26.00</code></pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob01#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Compiled and ran the driver (main).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (make test).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob01#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>main.cpp</code> and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob01#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.<pre><code>git add main.cpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="1a6e6f7c7c635a79696f347c6f76767f686e7574347f7e6f">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

</ol>

<h1>Roller coaster ride height</h1>

Create a program that prompts the passenger for their height to determine if they can safely ride the roller coaster. Print the appropriate messages according to their height. Please see the sample outputs below to guide the design of your program.

<h2><a id="user-content-safe" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob02#safe" aria-hidden="true"></a>Safe</h2>

<pre><code>You must be at least 55 inches to safely ride the TuffyTwister.Please enter your height in inches: 72Congratulations! You are tall enough to ride!</code></pre>

<h2><a id="user-content-unsafe" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob02#unsafe" aria-hidden="true"></a>Unsafe</h2>

<pre><code>You must be at least 55 inches to safely ride the TuffyTwister.Please enter your height in inches: 50Safety is our first priority. Unfortunately, we can't let you ride yet.</code></pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob02#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Compiled and ran the driver (main).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (make test).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob02#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>main.cpp</code> and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob02#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.<pre><code>git add main.cpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="34404152524d745747411a524158585146405b5a1a515041">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

</ol>




<h1>Salary Calculator</h1>

Create a program that computes the salary based on an employee’s hourly wage and hours worked. Use the following formulas:

Less than or equal to 40 hours worked

<code>hourly wage * hours worked</code>

Over 40, but less than or equal to 65 hours worked

<code>(hourly wage * 40) + (hours worked - 40) * (hourly wage * 1.5)</code>

Over 65 hours worked

<code>(hourly wage * 40) + (hourly wage * 1.5) * 25 + (hours worked - 65) * hourly wage * 2</code>

Please see the sample output below to guide the design of your program.

<pre><code>Hourly wage: 12Hours worked: 20Total Salary Owed: $240.00</code></pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob03#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Compiled and ran the driver (main).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (make test).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob03#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>main.cpp</code> and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob03#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.<pre><code>git add main.cpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5c28293a3a251c3f2f29723a293030392e28333272393829">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

</ol>

<h1>Cash Back</h1>

There are three credit card tiers available. The green card has a 10% cash back bonus, the yellow card has a 5% cash back bonus, and the red card has a 2% cash back bonus. Write a program that will compute the total cash back you receive. The program should ask the user to enter the type of card (‘g’ = green, ‘y’ = yellow, ‘r’ = red) as well as the amount of money spent. Display the amount of cash back earned showing 2 decimal places.

Take note that different user input results in a different output. Your program should also account for invalid card types by displaying an error message. Please see the sample outputs below to guide the design of your program.

<h2><a id="user-content-valid-input" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob04#valid-input" aria-hidden="true"></a>Valid input</h2>

<pre><code>Please enter type of card ('g' = green, 'y' = yellow, 'r' = red): yPlease enter amount of money spent: $42.12Amount of cash back received: $2.11</code></pre>

<h2><a id="user-content-invalid-input" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob04#invalid-input" aria-hidden="true"></a>Invalid input</h2>

<pre><code>Please enter type of card: cPlease enter amount of money spent: $42.12Invalid card type.</code></pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob04#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Compiled and ran the driver (main).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (make test).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob04#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>main.cpp</code> and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob04#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.<pre><code>git add main.cpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="b8cccddedec1f8dbcbcd96decdd4d4ddcaccd7d696dddccd">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

</ol>

<h1>Credit Card Approval</h1>

Create a program that will recommend a credit card to a customer based on their credit score. The list below shows the required credit scores for each type of credit card.

<pre><code>0   -  579: Ineligible for Tuffy credit cards580 -  669: Eligible for the Silver Tuffy Card670 -  799: Eligible for the Gold Tuffy Card800 -  850: Eligible for the Platinum Tuffy Card</code></pre>

Take note that credit scores below 0 and above 850 are invalid. Inform the customer when they provide invalid credit score values.

Please see the sample output below to guide the design of your program.

<h2><a id="user-content-sample-valid-inputs" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob05#sample-valid-inputs" aria-hidden="true"></a>Sample valid inputs</h2>

<pre><code>Thank you for applying for the Tuffy Credit card. Please enter your credit score.Credit Score: 600You are eligible for the Silver Tuffy Card.Thank you for using our program, please come again!</code></pre>

<pre><code>Thank you for applying for the Tuffy Credit card. Please enter your credit score.Credit Score: 560Unfortunately, you are ineligible for Tuffy credit cards at the moment. Please try again at a later date.Thank you for using our program, please come again!</code></pre>

<h2><a id="user-content-sample-invalid-input" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob05#sample-invalid-input" aria-hidden="true"></a>Sample invalid input</h2>

<pre><code>Thank you for applying for the Tuffy Credit card. Please enter your credit scoreCredit Score: 900That is an invalid credit score. Please run the program again and provide a valid credit score.</code></pre>

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob05#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Compiled and ran the driver (main).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (make test).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob05#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>main.cpp</code> and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp-o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/8324c2972e48a026f42453dd7879fd7b15ef6956/Labs/Lab_03/prob05#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.<pre><code>git add main.cpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="26525340405f664555530840534a4a435452494808434253">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

</ol>