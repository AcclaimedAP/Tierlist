# Tier list w/ links template incl. example
This is a Vue.js project that creates a tier list from an input(so far not decided, but probably JSON or an object.) It will format it in a pretty manner and then allow you to create links to these.

The example I will create this for is Genshin, but it can also be adjusted for any sort of tierlist you want. It will in this scenario rank them from S+ tier to D.

## Todo
- Dynmamically sort a list of characters into the tiers based on predetermined input
 * This should theoretically most likely be better to have been hardcoded previously, but we want it to be dynamic and easy to adjust.
 The idea is that it should very easily take an object that involves name and a tier, and then place it based on that into individual lists, or a big list of objects that is split into the tiers?
- link to pages for information about character.
 * Probably massive work to make it not feel bad, issue with a OPA is that you can't directly link to relevant information on it, look into solutions?
- Styling, lots of it...