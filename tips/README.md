# Helpful Tips and Tricks

- To get a date in **ISO format**, use the following format string: `yyyy-MM-dd'T'HH:mm:ss'Z'` in the "Date Format" app.
- If you are working with the **Datastore**, there is an introduction to it [here](https://pb-constructs.hightower.space/playbooks/introductions/datastore). There are gotchas [here](https://pb-constructs.hightower.space/playbooks/gotchas#datastore-gotchas).
- When using a **regex** in the "**Find and Replace**" playbook app, you can use `$1`, `$2`, etc. in the replace value to insert matched groups. For example, if you find the regex `(\S)\.(\S)`, this will find a non-whitespace character, followed by a period, followed by a non-whitespace character. Let's say you wanted replace the period with `[.]` (perhaps you are [defanging](https://ioc-fang.github.io/) indicators). To do this, you can use `$1[.]$2` as the replace value. The `$1` will be replaced with the non-whitespace character before the period and `$2` will be replaced with the non-whitespace character after the period.
- There is a website with some helpful resources at [http://playbooks.hightower.space/](http://playbooks.hightower.space/).
- There is a website listing open-source, ThreatConnect resources at [https://tc.hightower.space/](https://tc.hightower.space/).
