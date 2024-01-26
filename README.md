# Medusa's Uglier Sisters

code is built off from [Andrej Karpathy's famous guide on how to make a GPT](https://github.com/karpathy/ng-video-lecture)

ideas are based on [Medusa](https://github.com/FasterDecoding/Medusa)

by based on i mean the models & inference schemes you'll find here are just worse dumbed down versions of the Medusa method, hence "uglier" sisters rather than just sisters

My goals with this are to
1) be a silly goose
2) test out my newfound confidence with coding
3) learn about how Medusa works
4) experiment with some ideas that you might consider dumber (and therefore likely slower) than medusa
5) i'll likely post a video about this along with my general breakdown of how actual medusa works over on [my YT channel](https://www.youtube.com/channel/UCeQhm8DwHBg_YEYY0KGM1GQ) after i've either finished or given up on Euryale

## Stheno

basically a greedy decoding oversimplified version of the basic idea of speculative decoding with medusa heads

There is a speed increase over regular next-token prediction decoding. However the greedy decoding aspect is a huge bummer bc it makes the text too repetitive. 

## Euryale

basically a clever way to take advantage of batch decoding to do something akin to medusa but not using an attention mechanism. This is definitely an uglier sister tho, it's nowhere near as fast as medusa bc it's an absolute memory hog with the batch decoding. it was fun to make tho