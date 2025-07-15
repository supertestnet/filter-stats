# Filter stats
Documenting the statistical effect of filters over time

# What is this?
When arguing with bitcoiners about the effect of mempool filters, I often point out that their statistical effect is observable in the statistics revealed by blockchain analytics. For example, there is a mempool filter in bitcoin whereby most nodes block transactions that pay less than 1 sat per vbyte. When I point out this filter, many people who deny the effect of filters say that filter *has* no effect because some miners ignore it. But I say it is empircally observable via blockchain analytics, so I made this website to demonstrate the effect of filters.

# How to try it
Just go here: https://supertestnet.github.io/filter-stats

# What is it doing?
The website downloads the last 144 blocks and analyzes their transactions. If any transaction pays less than 1 sat per byte, it adds it to a list and updates a percentage counter. The percentage counter shows how the percentage of transactions that pay less than 1 sat per byte. When this percentage is low, it indicates that the filters are working: few people are getting transactions mined that pay a low feerate.
