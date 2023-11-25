# pandas-challenge


I used two methods to find the percentage of schools that passed both reading and math.

Method 1: passed reading * passed math = passed both - more stats 
Method 2 
- work1 = work.loc[(work['reading_score'] >= 70) & (work['math_score'] >= 70)] #method2
- total_passboth = work1.groupby('school_name')["School ID"].count()  # work1 is only the schools that passed both
- work = all schools
- total_schools = work.groupby('school_name')["School ID"].count()
- overallpassing = (total_passboth/total_schools)*100

The results were slightly differernet, so I made columns and top/bottom schools for both.
