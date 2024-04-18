Hello there!

Welcome to your lab environment.

To log in, you will need to use the following credentials:

Username: +++**@lab.VirtualMachine(Win11-TC24).Username**+++

Password: +++**@lab.VirtualMachine(Win11-TC24).Password**+++

Let us know if you need assistance with developing your lab. We are always happy to help!


===
# **Introduction Page:** Hello @lab.User.FirstName!
​
Thanks for attending **Game, Set, Match: Rallying Between Sets and Parameters! ** 

We're glad you're here, and we hope you're enjoying Tableau Conference 2024!
This is **page 1** of your lab instructions. It provides an overview of your virtual machine (VM), the materials we're using, and what you will be working on today.

Please read through this section as you get settled in so that we can hit the ground running.
​
### :boom: **About Today's Session**
#### **Overview**

* This is a beginner session! We will guide you through the first steps of working with **Sets** and **Parameters**.
* Our goal is to give you an entertaining learning experience while nerding out about Tennis and Grand Slams. Be advised that we will make bad jokes. But be ensured that you will learn something along the way.
* A hands-on can be challenging and time is always a constraint. If there is something you are not able to finish, stay calm and use the sheets and dashboards colored blue, they are showing the solution for any exercise.
* If you have questions, raise your hand and one of our room assistants will come over to help.
​
​
### :thinking: **About Sets & Parameters**
#### **What are Sets and Parameters?**
**Sets** and **Parameters** are ways to store data and make it accessible in various places in Tableau Desktop. **Parameters** can store arbitrary data of any data type Tableau Desktop understands except Geometries. They are a way to use data that is not within your data set and make it interact with your data set. **Sets** can store more complex structures, but only data that is within your data set. Both have unique use cases and some overlays. We will cover the basics today, but make sure to stick around till the end to see the true power of **Sets** and **Parameters**.
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
On your VM desktop, you will see a file named 'OUR SESSION TWBX' which contains all the exercises, solutions, and data you'll be working with today. The data is already embedded into the workbook. Each row represents a year in which a male or female player was winner or runner-up of a Grand Slam. Since there are 4 Grand Slams a year and our data set contains winner and runner-up since 2011, we will be using 208 rows of greatness.
​
>[!note] **Time for a little challenge?**
>How many rows do you have in your data set? What is missing and why?

​
### :athletic_shoe: **About the Exercises**
Each exercise is made up of multiple use cases which will need individual steps to complete. We will give you a rough outline of where to start and leave it to the exercise steps you will find on the following pages to guide you through each use case and through the exercises. You will find red colored sheets in the workbooks which are named as each exercise, these are your playground. You will find blue colored sheets in the workbooks named similarly which do show you the solution. If you follow along the instructions, you will get to these solutions as well.
​
* [Get a copy of the file](https://drive.google.com/drive/folders/119mMz3h2HU8CMLrLAX76eaABu-bJkQKh?usp=share_link)

That's the end of the introduction section. You can navigate to subsequent sections by clicking the arrows below. The next section contains the first of two exercises we will be doing together today.

===
# **Parameters** (Exercise 1 of 3)
​
### :bulb: **Key Points**  
* **Parameters** are like a safe for a single value of the type float, integer, string, date, datetime or boolean.
* **Parameters** can be use in calculations, filters and reference lines (etc.)
* **Parameters** can be controlled by the end user and can accept any value, or given values by the creator, or values determined by a dimension or measure in the data set
​
### :orange_book: **Resource Quick Links** 
* [Tableau Documentation - Parameters](https://help.tableau.com/current/pro/desktop/en-us/parameters_create.htm)
​
### :memo: **Exercise 1 - Parameter in Calculated Field** 
Andre Agassi does not go to any Slam. He values his time in retirement and only puts on the tennis rack if the prize is right! We will give him an overview which Grand Slams would have been feasible as winner or runner-up to attend.
​
* Double click on **'OUR SESSION TWBX'** on your VM desktop to open the the workbook in Tableau Desktop. 
* We will create a new **Parameter** for an integer value. It will be formated as currency. 
* The new **Paramter** will be shown and made available for input.
* In a new calculated field we will check if the prize money for a Grand Slam tournament was less than the the value of our **Parameter**.
* This calculated field will be used on shape to indicate the Slams above or below our **Parameter**
​

Complete the following steps for **Exercise 1**:
​
- [ ] **Step 1 -** Right click on any white space in the data pane and click on **Create Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.00.58.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.00.58.png){300}


- [ ] **Step 2 -** Name your **Parameter**, change Data type to **Integer**, change  Display format to **Currency (Standard)** (English (United States)) and click **Ok**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.11.11.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.11.11.png){500}

- [ ] **Step 3 -** Right click on your new **Parameter** and select **Show Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.14.35.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.14.35.png){300}

- [ ] **Step 4 -** Right click any white space in the data pane and click on **Create Calculated Field**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.16.49.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.16.49.png){300}

- [ ] **Step 5 -** Give the new calculated field a Name. Write a calculation that gives back <span style="color:grey">"Let's play some tennis!"</span> when the **Parameter** is above or equal to <span style="color:orange">[Prize Money $ USD]</span> and else <span style="color:grey">"Watch Netflix instead"</span>. Hit **OK**.

>[+hint] Click here to show the step
> 
> ``` -nocolor
> IF [Prize Money $ USD] >= [Prize Money Threshold]
> THEN "Let's play some tennis!"
> ELSE "Watch Netflix instead"
> END
> ```

- [ ] **Step 6 -** Drag your new calculated field to the **Shapes** area and change the value in your **Parameter** to 1000000.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.44.45.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.44.45.png){500}
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.52.54.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.52.54.png)

- [ ] **Step 7 -** Click on the **Shapes** area, choose the **Game Set Match** shapes palette and hit **Assign Palette**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.46.27.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.46.27.png){500}

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint1A]

> [Hint1A]:
> !IMAGE[Parameter - Exercise 1.gif](instructions258611/Parameter - Exercise 1.gif)

### :rocket: **DONE** :rocket:
Now play around with it and put some values into the **Parameter**.

**Move to the next section when you are done!**
​
===
# **Parameters** (Exercise 2 of 3)
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
Is there a way to make the Slams we would have loved to attend even more visually stand out? As Andre Agassi I'm known for my skills on hard surfaces and I detest clay! 
​
* Move to the next red colored sheet named **Exercise 2 - Parameter in Reference Line - Start**
* We will add a reference line to our view and it's value will be the **Parameter** we created in the first exercise
* We will color the area above and below the reference line to indicate John McEnroe's preference of grass surface on a tennis court

>[!knowledge] **Andre Agassi a legend on hard?**
Andre Agassi won six Grand Slams on hard. Two times the US Open and four time the Australian Open. He also won once the French Open and Wimbledon which are played on clay and grass.

​
Complete the following steps for **Exercise 2**:

- [ ] **Step 1 -** Move to the next red colored sheet named **Exercise 2 - Parameter in Reference Line - Start** and switch to the **Analytics tab**. You could also use your view from **Exercise 1**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 23.10.47.png](instructions258611/Bildschirmfoto 2024-04-11 um 23.10.47.png){300}

- [ ] **Step 2 -** Drag the **Reference Line** into the view on **Table** and **SUM(Prize Money $ USD)**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 23.14.45.png](instructions258611/Bildschirmfoto 2024-04-11 um 23.14.45.png){700}

- [ ] **Step 3 -** Change the Value to your created **Parameter** from **Exercise 1** or the provided **Parameter: *Prize Money Threshold***. Set **Label** to **None**. Hit **OK**. Remember to **Show Parameter** that you selected.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 23.17.55.png](instructions258611/Bildschirmfoto 2024-04-11 um 23.17.55.png){500}
> !IMAGE[Bildschirmfoto 2024-04-11 um 23.24.56.png](instructions258611/Bildschirmfoto 2024-04-11 um 23.24.56.png){500}

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint1B]

> [Hint1B]:
> !IMAGE[Parameter - Exercise 2.gif](instructions258611/Parameter - Exercise 2.gif)
    
### :rocket: **AWESOME** :rocket:
Feel free to play around with it again. It does not add much to our use case, but as you progress in your Tableau journey you will find unexpected uses for reference lines and you just learned your first step of making them interactive!

**Move to the next section when you are done!**
​
===
# **Parameters** (Exercise 3 of 3)
​
### :bulb: **Key Points**
* **Parameters** can be used in filters to make the N in Top N filters user dependant or to filter out values using the formula option in Condition or Top filters.
* We have see that **Parameters** can be used in calculated fields. These calculated fields can be used as filters themselves.

### :orange_book: **Resource Quick Links**  
* [Tableau Documentation - Parameters](https://help.tableau.com/current/pro/desktop/en-us/parameters_create.htm)
​
### :memo: **Exercise 3 - Parameter in Filter**

Money is just one metric. Andre knows, he just can't hold up with the worlds elite in a fully fledged 5 set match. Ever so slightly 20 years in age seem to do make a difference! Therefore, lets look for finals where the fewest points were made. In retirement Andre loves the low effort win.

* Move to the next red colored sheet named **Exercise 3 - Parameter in Filter - Start**
* We will create a new **Parameter** based on a field. This allows end users to only input eligable values.
* We will add a formular to a conditioned filter. The formular needs to be aggregated and the result of it needs to be **TRUE** or **FALSE**.


Complete the following steps for **Exercise 3**:

- [ ] **Step 1 -** Move to the next red colored sheet named **Exercise 3 - Parameter in Filter - Start** and create a new **Parameter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-11 um 22.00.58.png](instructions258611/Bildschirmfoto 2024-04-11 um 22.00.58.png){300}
​

- [ ] **Step 2 -** Give the **Parameter** a proper name. Data type must be **Integer**. Click on **Range** in Allowable values. Click on **Add values from** and select **Point Number**. Check **When workbook opens**. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-13 um 22.00.39.png](instructions258611/Bildschirmfoto 2024-04-13 um 22.00.39.png){500}

>[!knowledge] **How update Parameters based on Dimensions or Measures?**
You can choose **Fixed** and the values of a **Parameter** won't change even if the values of the underlying dimension or measure change. This saves queries and therefore loading time when a dashboard is opened. Usually you want the **Parameter** to update and the option **When workbooks opens** does that. It will query the underlying data when the workbooks opens in Tableau Desktop or the dashboard is opened in Tableau Server or Tableau Cloud and change the respective values of the **Parameter**.

- [ ] **Step 3 -** Right click on the discrete field named **Combined Field: Player, Event, Year** in the filter shelf and **Edit Filter**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-13 um 22.13.39.png](instructions258611/Bildschirmfoto 2024-04-13 um 22.13.39.png){300}

- [ ] **Step 4 -** Change to **Condition**, check **By formula** and write <span style="color:#5DADE2">SUM</span>(<span style="color:orange">[Point Number]</span>) <= <span style="color:#9B59B6">[Points per Game]</span>. Hit **OK**.

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-13 um 22.27.51.png](instructions258611/Bildschirmfoto 2024-04-13 um 22.27.51.png){500}

- [ ] **Step 5 -** Show the controls for your **Parameter**

>[+hint] Click here to show the step
> 
> !IMAGE[Bildschirmfoto 2024-04-13 um 22.28.43.png](instructions258611/Bildschirmfoto 2024-04-13 um 22.28.43.png){300}

- [ ] **Step 6 -** Change the value of your **Paramter** to above **141** to see games for both events. Switch to the dashboard **Exercise 3 Result** for a more immersive experience.

>[!hint]
^[Click here to show the whole solution! (You can drag the instruction pane further to the right to enlarge the GIF.)][Hint1C]

> [Hint1C]:
> !IMAGE[Parameter - Exercise 3.gif](instructions258611/Parameter - Exercise 3.gif)


### :rocket: **YOU GOT THIS** :rocket:
Well done! This concludes our exercises introducing **Parameter**. If you are done before the timer runs out: look or us, our assistants or give yourself a high five! We will move on shortly, guide you through the exercises again and give you some tips along the way.
​
​
===
# **Sets** (Exercise 1 of 4)
​
### :bulb: **Key Points**

### :orange_book: **Resource Quick Links**  
​
### :memo: **Exercise 1 - XXX**



​
===
# **Sets** (Topic 2 of 4)
​
### :bulb: **Key Points**

​
### :orange_book: **Resource Quick Links**  
​
​
### :memo: **Exercise 2 - XXX**


===
# **Sets** (Topic 3 of 4)
​
### :bulb: **Key Points**

​
### :orange_book: **Resource Quick Links**  
​
​
### :memo: **Exercise 3 - XXX**


===
# **Sets** (Topic 4 of 4)
​
### :bulb: **Key Points**

​
### :orange_book: **Resource Quick Links**  
​
​
### :memo: **Exercise 4 - XXX**

​
===
# **Wrapping Up**
## Thanks again for joining us today!
​
That's it! We've covered a lot today:
​
1. We created Parameter indipendantly and dependant on a measure.
2. We used Parameter in a calcualated field, in a reference line and in a filter.
3. We learned how Andre Agassi can get the most money for the least effort.
4. d
5. d
6. d

We hope you've enjoyed today's session! Please feel free to chat with us, ask questions, and keep in touch!
​
Lastly, here are some resources as you continue along with your Prep Builder journey:
​
### **Exercise Resources**
* [Get a copy of the files and flows](https://drive.google.com/drive/folders/119mMz3h2HU8CMLrLAX76eaABu-bJkQKh?usp=share_link)
​
### **Parameter Examples**
* [Parameter Driven Forecasting](https://public.tableau.com/app/profile/daria5688/viz/ParameterDrivenForecasting/ParameterDrivenForecasting)
* [Great Example of Parameter Actions](https://public.tableau.com/app/profile/marc.reid/viz/ParameterActionsExample/DateZoom)
* [Dynamic Drill Down with Zone Visibility](https://public.tableau.com/app/profile/ellen4268/viz/Dynamiczoningdemo/Dashboard1)
​
### **Set Examples**
More details on how you can optimize your Tableau workbooks beyond moving cleaning and calculation into Prep Builder:
* [Optimize Workbook Performance](https://help.tableau.com/current/pro/desktop/en-us/performance_tips.htm)
* [Designing Efficient Workbooks Whitepaper](https://www.tableau.com/learn/whitepapers/designing-efficient-workbooks)
