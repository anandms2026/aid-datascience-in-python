Correct ones: 
obj2['California'] == None
S.iloc[0:3]
all of these work
df.drop('two')
s2.loc[1]
loc and iloc are methods
df.T

failed onces

df = df.rename(mapper = lambda x: x.upper(), axis = 'columns') --fail
df.rename(mapper = lambda x: x.upper(), axis = 1)
df = df.rename(mapper = lambda x: x.upper(), axis = 1) Fail-- 
df.rename(mapper = lambda x: x.upper(), axis = 1, inplace = True)



df.where(df['toefl score'] > 105)
df[df['toefl score'] > 105]
All of these will work
df.where(df['toefl score'] > 105).dropna() Fail


(df['toefl score'] > 105) & (df['toefl score'] < 115)
df[df['toefl score'].gt(105) & df['toefl score'].lt(115)]--fail
df[(df['toefl score'].isin(range(106, 115)))] --fail
df[(df['toefl score'] > 105) & (df['toefl score'] < 115)]


my_categories = pd.CategoricalDtype(categories=['D', 'D+', 'C-', 'C', 'C+', 'B-', 'B', 'B+', 'A-', 'A', 'A+'])



my_categories = pd.CategoricalDtype(categories=['D', 'D+', 'C-', 'C', 'C+', 'B-', 'B', 'B+', 'A-', 'A', 'A+'], ordered=True)



my_categories = pd.CategoricalDtype(categories=['A+', 'A', 'A-', 'B+', 'B', 'B-', 'C+', 'C', 'C-', 'D+', 'D'])



(my_categories=['A+', 'A', 'A-', 'B+', 'B', 'B-', 'C+', 'C', 'C-', 'D+', 'D'], ordered=True)


1 point
4.
Question 4


