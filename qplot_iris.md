#install ggplot2
install.packages("ggplot2")
library(ggplot2)

#plot scatter plot of sepal length vs petal length
qplot(Sepal.Length, Petal.Length, data = iris)
#identify by species
qplot(Sepal.Length, Petal.Length, data = iris, color = Species)
#size of each point denotes petal width
qplot(Sepal.Length, Petal.Length, data = iris, color = Species, size = Petal.Width)
#make the plot little trasparent
qplot(Sepal.Length, Petal.Length, data = iris, color = Species, size = Petal.Width,
      alpha=I(0.7))
#add axis labels and title
qplot(Sepal.Length, Petal.Length, data = iris, color = Species, size = Petal.Width,
      xlab = "Sepal Length", ylab = "Petal Length", main = "Sepal vs Petal Length")
