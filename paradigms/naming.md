# Naming

Here are a few thoughts on naming conventions:

When it comes to naming variables, **be consistent**. No matter what you decide to do, stick with it. The variable `badDomain` works just as well as `bad_domain` (although one of them requires an extra character). Just be consistent.

Concerning the names of playbook apps, if you do change the name from the default name, you need to find a balance between being too ambiguous and too descriptive. You don't want to be too ambiguous because this isn't helpful, but you also don't want to be too descriptive because then you will have to change the name of the app if the app's functionality every changes. For example, if you are designing a playbook that runs once a week, a good name for the "Timer" trigger (which kicks off the playbook on a schedule) would be "Run Playbook Weekly". A name like "Run Playbook on Monday at 12:34" is probably too descriptive; if you ever change the day and/or time at which the Timer runs, you will also have to change the name. Changing an app's name isn't hard, but it is easy to forget to do so which means that the names of the apps become obsolete and confusing over time.
