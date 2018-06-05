# Helpful Tips and Tricks

- To get a date in **ISO format**, use the following format string: `yyyy-MM-dd'T'HH:mm:ss'Z'` in the "Date Format" app.
- If you are working with the **Datastore**, there are helpful tips [here](../introductions/datastore).
- When using a regex in the "Find and Replace" playbook app, you can use `$1`, `$2`, etc. in the replace value to insert matched groups. For example, if you find the regex `(\S)\.(\S)`, this will find a non-whitespace character, followed by a period, followed by a non-whitespace character. Let's say you wanted replace the period with `[.]` (perhaps you are [defanging](https://ioc-fang.github.io/) indicators). To do this, you can use `$1[.]$2` as the replace value. The `$1` will be replaced with the non-whitespace character before the period and `$2` will be replaced with the non-whitespace character after the period. 
