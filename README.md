# R-lauguage

norrow <- nrow(iris)
mylabel <- c()
for(i in 1:norow) {
  if (iris$Petal.Length[i] <= 1.6) {
    mylabel[i] <- 'L'
  } else if (iris$Petal.Length[i] <= 5.1) {
    mylabel[i] <- 'H'
  } else {
    mylabel[i] <- 'M'
  }
}



sum <- 0
i <- 1
while(i <=100) {
  sum <- sum + i
  i <- i + 1
}
print(sum)


apply(iris[,1:4], 1, mean)
apply(iris[,1:4], 2, mean)


mymax <- function(x,y) {
  num.max <- x
  if(y>x) {
    num.max <- y
  }
  return(num.max)
}

mymax(10,15)
a <- mymax(20,15)
b <- mymax(31,45)
print(a+b)



mydiv <- function(x,y=2) {
  result <- x/y
  return(result)
}

mydiv(x=10,y=3)
mydiv(10,3)
mydiv(10)



score <- c(76, 84, 69, 50, 95, 60, 82, 71, 88, 84)
idx <- which(score<=60)
score[idx] <- 61
score

idx <- which(score>=80)
score.high <- score[idx]
score.high



favorite <- c('winter', 'summer', 'spring', 'summer', 'summer', 'fall', 'fall', 'summer', 'spring', 'spring')
favorite
table(favorite)

ds <- table(favorite)
ds
barplot(ds, main= 'favorite season',
        col=rainbow(4),
        las=2)



blood <- 
ds <- table(blood)
barplot(ds, main = 'blood distribution',
        xlab = 'frequency',
        ylab = 'type',
        col = 'purple',
        names= c('AB','A','B','O')
        horiz = TRUE,
        las=1)







 
