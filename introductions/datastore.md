# Introduction to the Datastore

## Datastore Structure

When working with the datastore, I think of it like a file system with three levels:

`/{domain}/{store name}/{path}`

The datastore Playbook app provides a field for each of these levels:

![datastore structure](_images/datastore_app.png)

If you are trying to retrieve content from the datastore, you can leave the `entity` field empty; if you are trying to write/update content, put the new data in the `entity` field as valid json. For example, if you wanted to record the value of the [ETag](https://en.wikipedia.org/wiki/HTTP_ETag) of a domain, the datastore app would look something like:

![datastore example storing the etag for a domain](_images/example_datastore.png)

## Developer Tokens

In order to access the datastore outside of playbooks, you will need a developer token. You can get one in the ThreatConnect UI by hovering over the *gear icon in the upper right corner > Org Settings > Apps*. Then click the menu with three vertical dots on the right side of the screen and select *Get Developer Token*. This is necessary if you are trying to access the datastore via a REST client or a script outside of playbooks (which is helpful when testing/designing playbooks).
