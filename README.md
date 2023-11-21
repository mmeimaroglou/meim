# Example of README.md
?mtcars
dat=mtcars
pmatrix=scale(dat)
totwinss=c()
for (k in 1:4){
  k_cl=kmeans(pmatrix,k)
  totwinss[k] <- k_cl$tot.withinss
}
plot(1:4,totwinss,
     xlab='metablhtes',
     ylab='aytokihta')
lines(1:4,totwinss)
k_cl=kmeans(pmatrix,4)
table(mtcars$Specie,k_cl$cluster)
