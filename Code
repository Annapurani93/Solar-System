library(aRtsy)
library(tidyverse)
set.seed(1)
library(patchwork)

colors <- list(c("Orange", "red"),c("brown","beige"), c("beige","white"), 
               c("blue","green"), c("red"),c("yellow","white","brown"),c("lightgoldenrod1"), c("lightblue"),c("steelblue"))

canvas_planet(colors, radius = c(250, 25, 50, 50, 35, 100, 75, 75, 70), 
              center.x = c(100, 320, 400, 500, 585, 705, 855, 990, 1120),
              center.y = c(100, 320, 400, 500, 585, 705, 855, 990, 1120), 
              starprob = 0.005)->solarsystem

ggsave("solarsystem.png", solarsystem, width = 18, height = 18)

solarsystem & plot_annotation(
  title = 'Solar System',
  caption = "Art by @annapurani93")->solarsystem
