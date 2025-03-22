Hi, Dr. Wilkerson!

Initially, I wanted to use Tableau to create an interactive data visualization for this assignment.
However, I became frustrated by the lack of control offered. So, I created a website using GitHub Pages
and implemented a data visualization with the D3 JavaScript library. Please view my final deliverable
at kiron-ang.github.io/LoneStarImmunity.

The dataset, available at www.dshs.texas.gov/immunizations/data/school/coverage, contains data for 1,549
school districts in the state of Texas, encompassing public and private schools. Some of the columns
contain numerical information regarding the percentage of seventh graders in the school district that have
a particular vaccine. I originally wanted to display this data in a map of Texas, so users can quickly
identify geographical areas of interest.

However, I realized that the majority of users will only care about schools in their immediate vicinity.
If I am a parent in Houston, I will only care about schools in Harris County, since it is unlikely for me
to transfer my child to a school in Hidalgo county, even if I am greatly motivated by seventh grade
vaccination rates. This realization led me to choose a bar chart as the appropriate method of communication:
Instead of focusing on Texas as a whole, I can allow users to hone in on their county of residence in a
simple manner that allows for easy comparison of schools. Additionally, bar charts are easier to format and
display properly on a wide range of screens.

Concerning the colors of the app, I selected my palette from the visual identity of the Texas
Department of Transportation: www.txdot.gov/about/brand-guidelines/visual-identity/colors.html. I wanted
something that would be accessible, high-constrast, and representative of Texas. As a result, upon
first opening the page, users are greeted with elegant white Monsterrat text and three buttons on a minimal
blue background. After selecting a county and a vaccine, the user can generate a bar chart, where each bar
represents a school district, and the height of the bar is proportional to its vaccination rate. I 
intentionally removed the axes to both reduce visual noise and to force users to interact with the chart to
derive meaning. The only grounding point as users create different bar charts is an unobtrusive, dotted red
line that represents a vaccination rate of 85%.

This line, combined with the lack of margins between the bars and the ordering of the bars from highest
vaccination rate to lowest, optimizes the visual real estate so the bars themselves can take up the most
space on the screen. This was also intentional, again to encourage users to move their mouse over the bars
to reveal the name of the school district, whether or not the school is public or private, and the actual
numeric value for the vaccination rate. These details-on-demand are critical for respecting the time and goals
of users; instead of being bombarded with a hard-to-decipher table and unwieldly parameter controls, a user
can simply look at the lowest and highest schools, and then quickly locate their own school district. For
a busy parent trying to figure out if their child is in a well-vaccinated school district, my web application
allows them to compare their district's performance both in a relative and absolute fashion.

I spent approximately 20 hours on this project, including time spent exploring Tableau and D3. The aspects that
took the most time were the web design and fixing a bug where pressing the button consecutively without changing
the dropdown selections shrank the bars until they could no longer be seen. My code for this assignment is
available at github.com/kiron-ang/LoneStarImmunity. Thank you for your time and evaluation.

Sincerely,

Kiron Ang