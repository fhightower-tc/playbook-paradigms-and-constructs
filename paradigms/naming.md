# Names, Descriptions, and Labels

We want to be informative and consistent with our naming conventions and descriptions to maintain a clean and organized work environment. Here are a few guidelines to follow that will help you to accomplish this.

##Playbooks and Components

###Names
The first rule in naming your playbook is to make it as informative as possible. Short vague names don't serve your team justice and certainly not when your playbooks become large and complex.

We want to use proper capitalization and spaces while using descriptive names that give a little insight one _what_ the playbook does.

Some good examples:

* `Wayback Machine Query`
* `JOEs Sandbox Sample Submission`
* `Email and Indicator Extract`

Bad:

* `wayback_pb`
* `joes submit`
* `Email Indicators`

Ideally, we want to store as much info as to what the playbook does in the name while keeping it reasonably brief.

###Labels

Labels are a great tool offered to increase your productivity and make your playbook environment a little more organized.

For playbooks and components that are designed to fit into a larger overarching system, it is a good idea to add labels with their project/system names. This makes it easier to search for and browse playbooks by project.

If you have an owner specific playbook or component (only works or creates data in a owner), it is also a good idea to add the owner as a label.

If you work in the same ThreatConnect instance as other teams that are also building playbooks, adding labels with your team name is another good way to stay organized.

Labels should follow the same convention as naming (spaces, capitalization, and descriptive).

### Descriptions

This should be very straightforward. Write good descriptions that discusses not just _what_ a playbook or component does but also _how_ it fits in your team's goals or processes!

## Variables

When it comes to naming variables, **be consistent**. No matter what you decide to do, stick with it. The variable `badDomain` works just as well as `bad_domain` (although one of them requires an extra character). Just be consistent.

Concerning the names of playbook apps, if you do change the name from the default name, you need to find a balance between being too ambiguous and too descriptive. You don't want to be too ambiguous because this isn't helpful, but you also don't want to be too descriptive because then you will have to change the name of the app if the app's functionality every changes. For example, if you are designing a playbook that runs once a week, a good name for the "Timer" trigger (which kicks off the playbook on a schedule) would be "Run Playbook Weekly". A name like "Run Playbook on Monday at 12:34" is probably too descriptive; if you ever change the day and/or time at which the Timer runs, you will also have to change the name. Changing an app's name isn't hard, but it is easy to forget to do so which means that the names of the apps become obsolete and confusing over time.
