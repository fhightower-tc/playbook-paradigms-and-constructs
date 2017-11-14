# ThreatConnect Playbook Constructs

Helpful constructs and paradigms for building [playbooks](http://kb.threatconnect.com/customer/en/portal/articles/2744775-playbooks) in [ThreatConnect](https://app.threatconnect.com).

## If-Merge

This construct consolidates the output of an *if* operator so that a value is available to a down-stream playbook regardless of the value returned by the *if* operator.

![if_merge](_images/if_merge.png)

## Trigger Pass-back

Values can be passed from a playbook back to the response. This is especially helpful for user-action triggers and http link triggers.

![trigger passback 1](_images/trigger_passback_1.png)

![trigger passback 2](_images/trigger_passback_2.png)
