

### **Hello there!** ###

Welcome to your lab environment for this hands-on experience. 

To log in, you will need to use the following credentials:

Username: +++**Admin**+++

Password: +++**Passw0rd!**+++


Let us know if you need assistance. We are always happy to help!


### **When you are logged in follow these steps:** ###

- Open the workbook **HOT - 1842 - Game, Set, Match Rallying Between Sets & Parameters.twbx**

!IMAGE[Open Workbook v2.gif](instructions258611/Open Workbook v2.gif){500}

- Close **Show Me** and **Data Guide**

!IMAGE[Prepare Desktop.gif](instructions258611/Prepare Desktop.gif)

- Move to **Next: Introduction Page** in the lower right corner

!IMAGE[Go To First Exercise.gif](instructions258611/Go To First Exercise.gif)



===
# **Introduction Page**#
​
Thanks for attending **Game, Set, Match: Rallying Between Sets and Parameters! ** 

We're glad you're here, and we hope you're enjoying Tableau Conference 2024!
This is **page 1** of your lab instructions. It provides an overview of your virtual machine (VM), the materials we're using, and what you will be working on today.

Please read through this section as you get settled in so that we can hit the ground running.
​
### :boom: **About Today's Session**
#### **Overview**

* This is a beginner session! We will guide you through the first steps of working with **Sets** and **Parameters**.
* Our goal is to give you an entertaining learning experience while nerding out about tennis and Grand Slams. Be advised that we will make bad jokes, but be ensured that you will learn something along the way.
* A hands-on can be challenging and time is always a constraint. If there is something you are not able to finish, stay calm and use the sheets and dashboards colored blue, they show the solution for each exercise.
* If you have questions, raise your hand and one of our room assistants will come over to help.
​
​
### :thinking: **About Sets & Parameters**
#### **What are Sets and Parameters?**
**Sets** and **Parameters** are ways to store data and make it accessible in various places in Tableau Desktop. **Parameters** can store arbitrary data of any data type Tableau Desktop understands except Geometries. They are a way to use data that is not within your data set and make it interact with your data set. **Sets** can store more complex structures, but only data that is within your data set. Both have unique use cases and some overlaps. We will cover the basics today, but make sure to stick around 'til the end to see the true power of **Sets** and **Parameters**.
​
#### **Quick Resources**
* [Sets](https://help.tableau.com/current/pro/desktop/en-us/sortgroup_sets_create.htm)
* [Parameters](https://help.tableau.com/current/pro/desktop/en-us/parameters_create.htm)
​
### :tennis: **Put on your A game**
* We will dive into sport history and explore the winners and runner-ups of the Grand Slam tournaments from 2011 'til 2023! Follow your beloved Williams sisters on their road to victory, glory, equality and loads of :dollar: .
​
>[!knowledge] **What is a Grand Slam?**
Also referred to as majors, Grand Slams are the world's four most important annual professional tennis tournaments. They offer the most ranking points, prize money, public and media attention, the greatest strength and size of field. The four tournaments are: the Austrialian Open in Melbourne, the French Open in Paris, Wimbledon in London, and the US Open in New York.

* We will rally between explanations, hands-on examples, and use cases of **Sets** and **Parameters** throughout the session. There will be two slots for exercises where you will create **Sets** and **Parameters** respectively and use them for everyday tasks in Tableau Desktop.
* After each exercise we will redo the exercises on stage to give you more information, side-notes, and time to relax.
* After the exercises we will demonstrate more advanced techniques and uses cases as teasers for other sessions you can attend during TC24!

​
### :page_with_curl: **Materials**
On your VM desktop, you will see a file named 'HOT - 1842 - Game, Set, Match Rallying Between Sets & Parameters.twbx' which contains all the exercises, solutions, and data you'll be working with today. The data is already embedded into the workbook. Each row represents a year in which a male or female player was winner or runner-up of a Grand Slam. Since there are 4 Grand Slams a year and our data set contains winner and runner-up since 2011, we will be using 208 rows of greatness.
​
>[!note] **Time for a little challenge?**
>How many rows do you have in your data set? What is missing and why?

​
### :athletic_shoe: **About the Exercises**
Each exercise is made up of multiple use cases which will need individual steps to complete. We will give you a rough outline of where to start and leave it to the exercise steps you will find on the following pages to guide you through each use case and through the exercises. You will find yellow colored sheets in the workbook which are named as each exercise - these are your playground. You will find blue colored sheets in the workbooks named similarly which show you the solution. If you follow along with the instructions, you will get to these solutions as well.
​
* [Get a copy of the file](bit.ly/HOT-1842)

That's the end of the introduction section. You can navigate to subsequent sections by clicking the arrows below. The next section contains our first exercise!

===
# **Parameters - Exercise 1 - <span style="color:orange">we will do this exercise together!</span>** 
​
### :bulb: **Key Points**  
* **Parameters** are like a safe for a single value of the type float, integer, string, date, datetime or boolean.
* **Parameters** can be used in calculations, filters and reference lines, etc.
* **Parameters** can be controlled by the end user and can accept any value, or given values by the creator, or have values determined by a dimension or measure in the data set.
​
### :orange_book: **Resource Quick Links** 
* [Tableau Documentation - Parameters](https://help.tableau.com/current/pro/desktop/en-us/parameters_create.htm)
​
### :memo: **Exercise 1 - Parameter in Calculated Field** 
Andre Agassi does not go to just any Slam. He values his time in retirement and only picks up the tennis racket if the prize is right! We will give him an overview which Grand Slams would have been feasible as winner or runner-up to attend.
​
* **If you haven't had time to go through the initial instructions:** double-click on **'HOT - 1842 - Game, Set, Match Rallying Between Sets & Parameters.twbx'** on your lab's desktop to open the workbook in Tableau Desktop. Close **Show Me** and **Data Guide**.
* We will create a new **Parameter** for an integer value. It will be formated as currency. 
* The new **Paramter** will be shown and made available for input.
* In a new calculated field we will check if the prize money for a Grand Slam tournament was less than the the value of our **Parameter**.
* This calculated field will be used on shape to indicate the Slams above or below our **Parameter**.
​

Complete the following steps for **Exercise 1**, or <span style="color:orange">**lean back as we will go through this exercise together as an example**</span>:
​
- [ ] **Step 1 -** Right click on any white space in the data pane and click on **Create Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.00.58.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.00.58.png){300}


- [ ] **Step 2 -** Name your **Parameter**, for example **My Prize Money Threshold**, change Data type to **Integer**, change  Display format to **Currency (Standard)** (English (United States)), change Current value to **1000000** and click **Ok**.

>[+hint] Click here to show the step
> 
> !IMAGE[Exercise 1 Step 2.png](instructions258611/Exercise 1 Step 2.png)

- [ ] **Step 3 -** Right click on your new **Parameter** and select **Show Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.14.35.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.14.35.png){300}

- [ ] **Step 4 -** Right click any white space in the data pane and click on **Create Calculated Field**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.16.49.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.16.49.png){300}

- [ ] **Step 5 -** Give the new calculated field a name, for example **Should I attend?**. Write a calculation that gives back <span style="color:grey">"Let's play some tennis!"</span> when the **Parameter** is above or equal to <span style="color:orange">[Prize Money $ USD]</span> and else <span style="color:grey">"Watch Netflix instead"</span>. Hit **OK**.

>[+hint] Click here to show the step
> 
> ``` -nocolor
> IF [Prize Money $ USD] >= [My Prize Money Threshold]
> THEN "Let's play some tennis!"
> ELSE "Watch Netflix instead"
> END
> ```

- [ ] **Step 6 -** Drag your new calculated field to the **Shapes** area.

>[+hint] Click here to show the step
> 
> !IMAGE[Exercise 1 Step 6.png](instructions258611/Exercise 1 Step 6.png)

- [ ] **Step 7 -** Click on the **Shapes** area, choose the **Game Set Match** shapes palette and hit **Assign Palette**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.46.27.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.46.27.png){500}

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint1A]

> [Hint1A]:
> !IMAGE[Parameter - Exercise 1v3.gif](instructions258611/Parameter - Exercise 1v3.gif)

### :rocket: **DONE** :rocket:
Now play around with it and put some values into the **Parameter**.

**Move to the next section when you are done!**
​
===
# **Parameters - Exercise 2**
​
### :bulb: **Key Points** 
* **Parameters** can be used in **Reference Lines**, **Reference Bands** and **Distribution Bands** as values.
* Lines and Bands will be calculated anew every time the **Parameter** is changed.
​
### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Parameters](https://help.tableau.com/current/pro/desktop/en-us/parameters_create.htm)
​
### :memo: **Exercise 2 - Parameter in Reference Line**
​
Is there a way to make the Slams we would have loved to attend stand out even more visually? As Andre Agassi, I'm known for my skills on hard surfaces and I detest clay! 
​
* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 2 - Parameter in Reference Line - Start**.
* We will add a reference line to our view and its value will be the **Parameter** we created in the first exercise.
* We will color the area above and below the reference line to indicate Andre Agassi's preference of grass surface on a tennis court.

>[!knowledge] **Andre Agassi a legend on hard?**
Andre Agassi won six Grand Slams on hard: the US Open twice and the Australian Open four times. He also won the French Open and Wimbledon once each, which are played on clay and grass respectively.

​
Complete the following steps for **Exercise 2**:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 2 - Parameter in Reference Line - Start** and switch to the **Analytics tab**. You could also use your view from **Exercise 1**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 23.10.47.png](instructions258611/Bildschirmfoto 2024-04-11 um 23.10.47.png){300}

- [ ] **Step 2 -** Drag the **Reference Line** into the view on **Table** and **SUM(Prize Money $ USD)**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 23.14.45.png](instructions258611/Bildschirmfoto 2024-04-11 um 23.14.45.png){700}

- [ ] **Step 3 -** Change the Value to your created **Parameter** from **Exercise 1** or the provided **Parameter: *Solution - Prize Money Threshold***. Set **Label** to **None**. Hit **OK**. Remember to **Show Parameter** that you selected.

>[+hint] Click here to show the step
> 
> !IMAGE[Exercise 2 Step 3.png](instructions258611/Exercise 2 Step 3.png){500}
> !IMAGE[Exercise 2 Step 3 1.png](instructions258611/Exercise 2 Step 3 1.png){500}

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint1B]

> [Hint1B]:
> !IMAGE[Parameter - Exercise 2v2.gif](instructions258611/Parameter - Exercise 2v2.gif)
    
### :rocket: **AWESOME** :rocket:
Feel free to play around with it again. It does not add much to our use case, but as you progress in your Tableau journey you will find unexpected uses for reference lines and you just learned your first step of making them interactive!

**Move to the next section when you are done!**
​
===
# **Parameters - Exercise 3**
​
### :bulb: **Key Points**
* **Parameters** can be used in filters to make the N in Top N filters user-dependant, or to filter out values using the formula option in Condition or Top filters.
* We have seen that **Parameters** can be used in calculated fields. These calculated fields can be used as filters themselves.

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Parameters](https://help.tableau.com/current/pro/desktop/en-us/parameters_create.htm)
​
### :memo: **Exercise 3 - Parameter in Filter**

Money is just one metric. Andre knows, he just can't hold up with the world's elite in a fully fledged 5 set match. Ever so slightly 20 years in age seem to make a difference! Therefore, let's look for finals where the fewest points were made. In retirement, Andre loves the low effort win.

* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 3 - Parameter in Filter - Start**.
* We will create a new **Parameter** based on a field. This allows end users to only input eligible values.
* We will add a formula to a conditioned filter. The formula needs to be aggregated and the result of it needs to be **TRUE** or **FALSE**.


Complete the following steps for **Exercise 3**:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 3 - Parameter in Filter - Start** and create a new **Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.00.58.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.00.58.png){300}
​

- [ ] **Step 2 -** Give the **Parameter** a proper name like **Points per Game**. Data type must be **Integer**. Click on **Range** in Allowable values. Check **When workbook opens**. Click on the dropdown menu displaying None and select **Point Number**. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Exercise 3 Step 2.png](instructions258611/Exercise 3 Step 2.png){500}

>[!knowledge] **How to update Parameters based on Dimensions or Measures?**
You can choose **Fixed** and the values of a **Parameter** won't change even if the values of the underlying dimension or measure change. This saves queries and therefore loading time when a dashboard is opened. Usually you want the **Parameter** to update and the option **When workbooks opens** does that. It will query the underlying data when the workbooks opens in Tableau Desktop or the dashboard is opened in Tableau Server or Tableau Cloud and change the respective values of the **Parameter**.

- [ ] **Step 3 -** Right click on the discrete field named **Every Player, Slam and Year** in the filter shelf and **Edit Filter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Exercise 3 Step 3.png](instructions258611/Exercise 3 Step 3.png){300}

- [ ] **Step 4 -** Change to **Condition**, check **By formula** and write <span style="color:#5DADE2">SUM</span>(<span style="color:orange">[Point Number]</span>) <= <span style="color:#9B59B6">[Points per Game]</span>. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Exercise 3 Step 4.png](instructions258611/Exercise 3 Step 4.png){500}

- [ ] **Step 5 -** Show the controls for your **Parameter**

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-13 um 22.28.43.png](instructions258611/Bildschirmfoto 2024-04-13 um 22.28.43.png){300}

- [ ] **Step 6 -** Change the value of your **Paramter** to above **141** to see games for both events. Switch to the dashboard **Exercise 3 Result** for a more immersive experience.

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint1C]

> [Hint1C]:
> !IMAGE[Parameter - Exercise 3v2.gif](instructions258611/Parameter - Exercise 3v2.gif)


### :rocket: **YOU GOT THIS** :rocket:
Well done! This concludes our exercises introducing **Parameter**. If you are done before the timer runs out: look for us or our assistants, or give yourself a high five! We will move on shortly and guide you through the exercises again, and give you some tips along the way.
​
​
===
# **Sets - Exercise 4 - <span style="color:orange">we will do this exercise together!</span>** 
​
### :bulb: **Key Points**
* **Sets** can be created a few different ways, one of them being visually. 
* **Sets** can be dynamic or fixed. The members of a **Fixed Set** do not change, even if the underlying data changes. A **Fixed Set** can be based on a single dimension or multiple dimensions.
* Keep in mind that **Sets** are meant to make comparisons on subsets of data. Groups, which are also fixed, are meant to combine related members in a field.

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Sets](https://help.tableau.com/current/pro/desktop/en-us/sortgroup_sets_create.htm)

### :memo: **Exercise 4 - Visual Set**

A variety of players have been finalists in the US Open in this snapshot of history, more than for the other Grand Slams. Serena Williams wonders, who were the winners of the US Open?


* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 4 - Visual Set - Start**.
* We will create a new **Set** visually, based on a few conditions. This allows us to intuitively and flexibly create sets from visualized data.
* This set will later be able to be used to answer our questions.


Complete the following steps for **Exercise 4**, or <span style="color:orange">**lean back as we will go through this exercise together as an example**</span>:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 4 - Visual Set - Start**.
​

- [ ] **Step 2 -** From the list of fields on the left, double-click **Placement**. The field should now be added to your viz.


>[+hint] Click here to show the step
> 
> ​!IMAGE[Set 4, step 2.png](instructions258611/Set 4, step 2.png)


- [ ] **Step 3 -**  From the list of fields on the left, double-click **Player**. The field should now be added to your viz.


>[+hint] Click here to show the step
> 
> !IMAGE[Set 4, step 3.png](instructions258611/Set 4, step 3.png)

- [ ] **Step 4 -** On the viz, click **Winner** under the **US Open** text. From the tooltip menu, select the **Set** symbol, which looks like a Venn diagram. Select **Create Set...**. 

>[+hint] Click here to show the step
> 
> !IMAGE[Set 4, step 4.png](instructions258611/Set 4, step 4.png)

- [ ] **Step 5 -** Name the **Set** **US Open Winners**. The **Set** should have **18 members**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 4, step 5.png.png](instructions258611/Set 4, step 5.png.png)


- [ ] **Step 6 -** In the **Set** creation window, **remove** the **Slam** and **Placement** fields, keeping only the **Player** field. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 4, step 6.png.png](instructions258611/Set 4, step 6.png.png)

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint2A]

> [Hint2A]:
> !!IMAGE[Set Ex 4.gif](instructions258611/Set Ex 4.gif)

### :rocket: **WAY TO GO** :rocket:

**Move to the next section when you are done!**

​
===
# **Sets - Exercise 5**
​
### :bulb: **Key Points**
* **Sets** can be created similarly to filters by general selection, condition, or top of a field.
* **Sets** can be dynamic or fixed. The members of a **Dynamic Set** change when the underlying data changes. **Dynamic Sets** can only be based on a single dimension.

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Sets](https://help.tableau.com/current/pro/desktop/en-us/sortgroup_sets_create.htm)

### :memo: **Exercise 5 - Conditional Set**

A majority of these top tennis players have US nationality, including Serena herself. If Serena wants to dig deeper into these US players and how they perform across the Slams, she has to create a set.


* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 5 - Conditional Set - Start**.
* We will create a new **Set** using a condition in a formula. The formula needs to be aggregated and the result of it needs to be **TRUE** or **FALSE**.
* This set will be used in the next exercise to make comparisons on subsets of data.

Complete the following steps for **Exercise 5**:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 5 - Conditional Set - Start**.


- [ ] **Step 2 -** From the list of fields on the left, right-click **Player**. From the menu, go to **Create**, then select **Set...**. From the new window that opens, name the **Set** **US Players Set**.


>[+hint] Click here to show the step
> 
> !IMAGE[Set 5 and 8, step 2.png](instructions258611/Set 5 and 8, step 2.png)


- [ ] **Step 3 -**  At the top of the **Set** creation window, select **Condition**, then select the third option, **By formula**. Write a calculation that gives us only the <span style="color:orange">[Nationality]</span> **USA**. Make sure to aggregate your calculation. Hit **OK**.


>[+hint] Click here to show the step
> 
> !IMAGE[Set 5, step 3.png](instructions258611/Set 5, step 3.png)

>[+hint] Click here to show the calculation
> 
> ``` -nocolor
> MAX(Nationality="USA")
> ```

>[!knowledge] **Aggregating booleans**
The result of the calculation needs to be true or false, making it a boolean. Commonly used aggregations for boolean fields are MIN() and MAX(). 


- [ ] **Step 4 -** From the list of fields on the left, drag the **US Players Set** to color to confirm the USA bar is **In** the **Set**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 5, step 4.png](instructions258611/Set 5, step 4.png)


>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint2B]

> [Hint2B]:
> !IMAGE[Set Ex 5.gif](instructions258611/Set Ex 5.gif)

### :rocket: **AMAZING** :rocket:
Now play around with it! What insights can you gain if you change which set is on color, for example, the US Open Winners Set? 

**Move to the next section when you are done!**


===
# **Sets - Exercise 6**
​
### :bulb: **Key Points**
*  **Proportional Brushing** is a very common method of seeing parts of a whole. Using **Sets** is an easier and more dynamic way of achieving this than using Level of Detail calculations.

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Sets](https://help.tableau.com/current/pro/desktop/en-us/sortgroup_sets_create.htm)

### :memo: **Exercise 6 - Proportional Brushing**

It's time to dig deeper! How did the US players perform across the Slams, both as winners and runner-ups?


* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 6 - Proportional Brushing - Start**.
* We will use our **US Players Set** we created in the last exercise to see how many US Players won the different Grand Slams.


Complete the following steps for **Exercise 6**:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 6 - Proportional Brushing - Start**.
​

- [ ] **Step 2 -** From the list of fields on the left, drag the **US Players Set** to color.


>[+hint] Click here to show the step
> 
> !IMAGE[Set 6, step 2.png](instructions258611/Set 6, step 2.png)


>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint2C]

> [Hint2C]:
> !IMAGE[Set Ex 6.gif](instructions258611/Set Ex 6.gif)

### :rocket: **WELL DONE** :rocket:
See how the results change when using the Placement filter. Notice how the number of US Players who placed in the US Open changes.

**Move to the next section when you are done!**


===
# **Sets - Exercise 7**
​
### :bulb: **Key Points**
* **Sets** can be combined in order to ask complex questions and compare cohorts of data. 
* You can choose to view **Sets** by which values are **In** or **Out** of the set, or by the **Individual Members**.
* **Sets** can also be used as filters.

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Sets](https://help.tableau.com/current/pro/desktop/en-us/sortgroup_sets_create.htm)

### :memo: **Exercise 7 - Combine Sets**

Serena has seen how the US players performed at Slams, but now she wonders who else, besides her, has both US nationality and won the US Open? Is there an easy way to use the work she's already put in to answer her next question?


* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 7 - Combine Sets - Start**.
* We will create a new **Set** by combining our **US Open Winners Set** and **US Players Set**.
* We will look at the **Individual Members** of our combined **Set**.


Complete the following steps for **Exercise 7**:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 7 - Combine Sets - Start**.
​

- [ ] **Step 2 -** From the list of fields on the left, right-click the **US Players Set**. From the menu, select **Create Combined Set...**. 


>[+hint] Click here to show the step
> 
> !IMAGE[Set 7, step 2.png](instructions258611/Set 7, step 2.png)


- [ ] **Step 3 -**  From the new window that opens, name the **Set** something relevant, for example, **US US Open Winners Set**. Combine the **US Players Set** with the **US Open Winners Set**. Select **Shared members in both sets** from the options listed. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 7, step 3.png](instructions258611/Set 7, step 3.png)


>[!knowledge] **Combining Sets**
You can combine two **Sets** to compare the members. When you combine **Sets** you create a new **Set** containing either the combination of all members, just the members that exist in both, or members that exist in one **Set** but not the other.
Combining **Sets** allows you to answer complex questions and compare cohorts of your data. For example, to determine the percentage of customers who purchased both last year and this year, you can combine two **Sets** containing the customers from each year and return only the customers that exist in both **Sets**.
To combine two **Sets**, they must be based on the **same dimensions**.


- [ ] **Step 4 -** From the list of fields on the left, drag the **US US Open Winners Set** onto **rows**. From there, right-click on the pill. From the menu, select **Show Members in Set** (instead of Show In/Out of Set). You should see 3 names in the viz. 

>[+hint] Click here to show the step
> 
> !IMAGE[Set 7, step 4.png](instructions258611/Set 7, step 4.png)


>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint2D]

> [Hint2D]:
> !IMAGE[Set Ex 7.gif](instructions258611/Set Ex 7.gif)

### :rocket: **KEEP IT UP** :rocket:
These 3 players have won the US Open and have US nationality. 

**Move to the next section when you are done!**


===
# **Sets - Exercise 8**
​
### :bulb: **Key Points**
* **Parameters** and **Sets** can be used together to allow for more flexibility when looking at subsets of data.
* **Set Controls** allow end users to control the members of a **Set**. 

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Sets for Top N and Others](https://help.tableau.com/current/pro/desktop/en-us/sortgroup_sets_topn.htm)

### :memo: **Exercise 8 - Set & Parameter**

She's looked into the US competition, but Serena knows she doesn't just stand out as a tennis winner; she also stands out as a prize winner. It's time to put individual competition aside and step onto the court as partners. Can Serena use sets and parameters together to find the top earners, and see how she compares?


* Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 8 - Set & Parameter - Start**.
* We will create a new, dynamic **Set** using the **Top N** of a field. You can choose to display a **Set Control** to let users choose the members of the **Set**.
* We will create a new **Parameter** to input the **number** of values that will be displayed from our **Set**. 


Complete the following steps for **Exercise 8**:

- [ ] **Step 1 -** Move to the next <span style="color:#FFD700">yellow</span> colored sheet named **Exercise 8 - Set & Parameter - Start**.
​

- [ ] **Step 2 -** From the list of fields on the left, right-click **Player**. From the menu, go to **Create**, then select **Set...**. From the new window that opens, name the **Set** **Top N Earners Set**.


>[+hint] Click here to show the step
> 
> !IMAGE[Set 5 and 8, step 2.png](instructions258611/Set 5 and 8, step 2.png)

- [ ] **Step 3 -** At the top of the **Set** creation window, select **Top**, then select the second option, **By field**. 
Select **Top** and **Create a New Parameter...** for the first two drop-down selections.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 8, step 3.png](instructions258611/Set 8, step 3.png)


- [ ] **Step 4 -** From the new window that opens, name the **Parameter** **Top N Parameter**. Change **Current value** to **5**. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 8, step 4.png](instructions258611/Set 8, step 4.png)

- [ ] **Step 5 -** In the **Set** creation window, make sure **Prize Money $ USD** and **Sum** are selected for the last two drop-down selections. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 8, step 5.png](instructions258611/Set 8, step 5.png)

- [ ] **Step 6 -** Right click on your new **Top N Parameter** and select **Show Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 8, step 6.png](instructions258611/Set 8, step 6.png)

- [ ] **Step 7 -** From the list of fields on the left, drag the **Top N Earners Set** to **Filters**. The viz should automatically filter to the top players by prize money based on the value you entered into the **Top N Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Set 8, step 7.png](instructions258611/Set 8, step 7.png)

- [ ] **Step 8 -** From **Filters**, right-click the **Top N Earners Set**. From the menu, select **Show Set**. 

>[+hint] Click here to show the step
> 
> !IMAGE[Set 8, step 8.png](instructions258611/Set 8, step 8.png)

>[!knowledge] **Set Control**
To give your audience the ability to quickly modify members of a **Set**, you can also display a **Set Control**. A **Set Control** is a worksheet card that is very similar to a parameter control or filter card. You can add **Set Controls** to worksheets and dashboards.
You can only display a set control for **dynamic sets—not fixed sets**. This is by design, as fixed sets aren’t meant to change in membership. In addition, if the dynamic set is not in play in the view (that is, if it’s not referenced in a calculation or is not on the sheet), the context menu item will be disabled, reminding you to add the set to the view.


>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint2E]

> [Hint2E]:
> !IMAGE[Set Ex 8.gif](instructions258611/Set Ex 8.gif)

### :rocket: **GAME OVER** :rocket:
Now play around with it! What insights can you gain if you add previous **Sets** to color to see who didn't win the US Open or who is a US player? What happens if you change which players are in your **Set** using the **Set Control**?

Well done! This concludes our exercises introducing **Sets**. If you are done before the timer runs out: look for us or our assistants, or give yourself a high five! We will move on shortly and guide you through the exercises again, and give you some tips along the way.
​

**Move to the final section when you are done to review what you've learned!**

===
# **Wrapping Up**
## Thanks again for joining us today!
​
That's it! We've covered a lot today:
​
1. We created a Parameter independently and dependent on a measure.
2. We used a Parameter in a calcualated field, in a reference line, and in a filter.
3. We learned how Andre Agassi can get the most money for the least effort.
4. We created a Set visually, conditionally, and by combining other sets.
5. We displayed Set members individually, aggregated, and with set controls.
6. We learned that Serena Williams is an outlier amongst women in tennis.

We hope you've enjoyed today's session! Please feel free to chat with us, ask questions, and keep in touch!
​

Lastly, here are some resources as you continue along with your **Parameter** and **Sets** journey:
​
### **Exercise Resources**
* [The Workbook with all Exercises and Solutions](bit.ly/HOT-1842)
​
### **Parameter Examples**
* [Parameter Driven Forecasting](https://public.tableau.com/app/profile/daria5688/viz/ParameterDrivenForecasting/ParameterDrivenForecasting)
* [Great Example of Parameter Actions](https://public.tableau.com/app/profile/marc.reid/viz/ParameterActionsExample/DateZoom)
* [Dynamic Drill Down with Zone Visibility](https://public.tableau.com/app/profile/ellen4268/viz/Dynamiczoningdemo/Dashboard1)
​
### **Set Examples**
* [8 analytic concepts to express with Tableau set actions](https://www.tableau.com/blog/8-analytic-concepts-express-tableau-set-actions-99108)
* [Relative Map](https://www.sirvizalot.com/2018/11/how-to-create-relative-map-using-set.html)
* [Single Member Drill Down] (https://public.tableau.com/app/profile/bethany.lyons/viz/SingleMemberDrillDown/GIF)
