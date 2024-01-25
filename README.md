# Medusa's Uglier Sisters

code is built off from [Andrej Karpathy's famous guide on how to make a GPT](https://github.com/karpathy/ng-video-lecture)
ideas are based on [Medusa](https://github.com/FasterDecoding/Medusa)
by based on i mean the models & inference schemes you'll find here are just worse dumbed down versions of the Medusa method, hence "uglier" sisters rather than just sisters

My goals with this are to
1) be a silly goose
2) test out my newfound confidence with coding
3) learn about how Medusa works
4) experiment with some ideas that you might consider dumber (and therefore likely slower) 
5) i'll likely post a video about this along with my general breakdown of how actual medusa works over on [my YT channel](https://www.youtube.com/channel/UCeQhm8DwHBg_YEYY0KGM1GQ) after i've either finished or given up on Euryale

## Stheno

the one working right now. basically a greedy decoding oversimplified version of one of Medusa's basic ideas
Rn i've seen a 1.33x speed increase over regular next-token prediction decoding. I think this could easily be a lot faster if I remove all the print statements, generally optimize my code, and use a bigger model with more snake heads. Thinking if I do that it'll be in a separate jupyter notebook just so i can keep the main one working for teaching purposes

## Euryale

haven't yet started, but basically I think i have a clever way to take advantage of batch decoding. Small chance this is actually quicker than actual Medusa, although it'll definitely be more memory intensive. 