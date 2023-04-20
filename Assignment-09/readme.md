#Data Visualization II
---
Use the inbuilt dataset 'titanic' as used in the above problem. 

1.Draw scatterplot for distribution of survivors by gender

2.Calculate mean of survivors

3.Generate uniform distribution

4.Combine the scatter plot for survivals of male and female in the same figure. Show different colors and intensities to add more information to the plot. 


5.Bar + Scatter Plot (Stripplot)
A strip plot is a scatter plot where one of the variables is categorical.
---
fig, ax = plt.subplots(1, 1, figsize=(9, 7))
np.random.seed(42)

Male Stripplot
ax.scatter(np.random.uniform(-0.3, 0.3, len(male_pos)), male_pos, color='#004c70', edgecolor='lightgray', label='Male(Survived=1)')
ax.scatter(np.random.uniform(-0.3, 0.3, len(male_neg)), male_neg, color='#004c70', edgecolor='lightgray', alpha=0.2, label='Male(Survived=0)')

---

Female Stripplot
ax.scatter(1+np.random.uniform(-0.3, 0.3, len(female_pos)), female_pos, color='#990000', edgecolor='lightgray', label='Female(Survived=1)')
ax.scatter(1+np.random.uniform(-0.3, 0.3, len(female_neg)), female_neg, color='#990000', edgecolor='lightgray', alpha=0.2, label='Female(Survived=0)')

---

6.Add legend and titles
Use set_xlim()
set_ylim()
x_ticks()
y_ticks()
legend()
text()   methods
