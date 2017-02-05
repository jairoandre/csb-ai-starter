# Introduction

Aim of this project is to serve as a starter code for search based AI solutions to the [Coders Strike Back](https://www.codingame.com/multiplayer/bot-programming/coders-strike-back) bot programming challenge. 

It provides a fully working and tested simulation engine, simple mutation-based search algorithm, basic reflex AI and generic API with which the user can extend the bot. It is written with performance in mind and can achieve an average of 200k-250k simulations per turn.

Without any modifications this bot is ranked at 30 out of 19000. With a GA-based search it can get to top 10. A heavily modified version of it currently holds rank 4.

# Usage

Assuming you are in Legend league, all you need to do is copy/paste and hit submit. If you are in Gold league, you'll need to change `MAX_THRUST` const to `100`. Code assumes input format provided in Gold league and above and will not work for lower leagues.

# Next steps

If you want to get further in the ranking, you'll need to start adding improvements to it. Here are some ideas in order of difficulty to implement:

* Add more parameters to evaluation function
* Add different coefficients to evaluation parameters
* Add bots with alternative coefficients as opponents for your main bot
* Replace solver with Genetic Algorithm based (**most impact**)
* Replace computationally heavy math functions with cache or approximations
* Rewrite reflex bot implementation

# Additional resources

* [Magus post-mortem](http://files.magusgeek.com/csb/csb_en.html) (bulk of API and collision code is based on this)
* [pb4 post-mortem](https://www.codingame.com/blog/coders-strike-back-pb4608s-ai-rank-3rd/)
* [Jeff06 post-mortem](https://www.codingame.com/blog/genetic-algorithms-coders-strike-back-game/)
* [sethorizer's sim engine tester](https://github.com/sethorizer/csb)