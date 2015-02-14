# WEEK-4
HOMEWORKS 7 , 8 ,9 &amp; 10

hw7:

1.1   9

2.1  hist(dat[,4])

2.2 hist(dat[,9])

3.1  boxplot(InsectSprays$count ~ InsectSprays$spray)
     # C

hw8:

1.1  mean(scale(x) * scale(y))

2.1 min(time) / median(time)

2.2 max(time) / median(time)

3.1 # NEVER

3.2 # CONFUSION

3.3 # To compare percentages that add up to 100%

hW9:

1.1 

library(dplyr)

msleep %>%

mutate(rem_proportion = sleep_rem / sleep_total) %>%

group_by(order) %>%

summarise(medremprop = median(rem_proportion)) %>%

arrange(medremprop) %>%

head(3)

HW10:

1. mean(c(chick$weight.4, 3000))/mean(chick$weight.4)

2. median(c(chick$weight.4, 3000))/median(chick$weight.4)

3. sd(c(chick$weight.4, 3000))/sd(chick$weight.4)

4. cor(c(chick$weight.4, 3000), c(chick$weight.21,3000))/cor(chick$weight.4, chick$weight.21)

5.  x = chick$weight.4[chick$Diet == 1]

    y = chick$weight.4[chick$Diet == 4]

    t.test(c(x, 200), y)$p.value

6.  t.test(x,y + 10)$statistic - t.test(x,y + 100)$statistic
    # bear in mind the codes from question 5 
