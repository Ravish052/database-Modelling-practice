# School-mgmt DB design

step by step design of a school database 

students can move to a different year levels

grade1 -> gradw2 -> grade3 ....



requirements >>>

1. school stores info about students, name, gender, DOB, date of enrollment
2. store info about parents, grand parents and other guardians, along with their contacts and addresses
3. schools operate based on school years. an year has a start date and an end date, and can be in a single calendar yrar or multiple
4. a year has multi[le semesters. theres no fixed number of terms per year
5. studenst are enrolled in one year level at a time, and can move up to the next level  in the future
6.  students are part of classes and can be in more than one class at a time
7. classes have subjects such as sports, physiics, a class subject may be a more generalname for the junior years.
8. subjects belong to departments
9. a class is taught by a teacher
10. teachers have name, genders and contact info.
11. a class exists for a term, there can be multiple classes in a year, and multiple classes within the same term. a class can have a name to help describe it
12. classes are held in classroom. there are types of classromms and have names
13. the time a class occurs is called a period, there are certain number of periods per day, and the periods are set for the enntire school each year
14. a class can occur over multiple periods, which could be two periods or up to the entire day
15. students are scored between 0 -100 for each class, and calculation is done to determine their overall score for the year
16. the scores can be matched to a letter grade 


