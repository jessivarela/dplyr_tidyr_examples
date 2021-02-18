library(tidyverse)
library(untidydata)

# data from untidydata set 
pre_post


# separate into different columns 
pre_post %>%
  separate(., col = spec,
           into = c( "group", "cond"), 
           sep = "_")

#unite into one column 
pre_post %>% 
  unite(., col = "silly", 
        c("id", "spec"),
        sep = "_")

#pivot_longer
pre_post %>%
  pivot_longer(., 
               cols = "test1", "test2",
               names_to = "test",
               values_to = "score") %>%
  ggplot(., aes(x = test, y = score)) +
           geom_boxplot()

#pivot_wider 
language_diversity %>% glimpse

language_diversity %>%
  pivot_wider(
    id_cols = ,
    names_from = ,
    values_from = 
  )

or 

#pivot_wider other example
language_diversity %>% glimpse

language_diversity %>%
  pivot_wider(
    id_cols = c("Measurement", "Value") ,
    names_from = Measurement,
    values_from = Values
    ) %>%
  ggplot(., aes(x = log(Population, y= Langs)) +
  geom_point()


