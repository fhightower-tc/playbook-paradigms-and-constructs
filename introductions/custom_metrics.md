# Introduction to Custom Metrics

Custom metrics are extremely powerful and can solve a variety of use-cases. This is a brief introduction to the what they are and how one might use them.

## What are Custom Metrics?

Custom metrics is a feature built into ThreatConnect that allows you to store and process basic information.

## How do Custom Metrics Work?

There are three important aspects of a custom metric:

1. **Data type:** this aspect determines what operation will be performed on incoming data. Some of the available options are: Sum, Count, and Average.
2. **Interval:** this determines how often the data in the custom metric will zeroed. Custom metrics can be reset at many intervals from hourly to yearly.
3. **Keyed/Non-keyed:** this setting allows you to 'group' metrics based on a key. Data within a keyed metric will be stored as key-value pairs. For example, if you wanted to keep a count of the malware sandboxes you have used in a month, you may want to use a keyed metric with the key being the name of the sandbox. You can think of the data in a keyed metric like data in a table with the key as the first column and the value as the second:

| Key | Value |
|---|---|
| VirusTotal | 5 |
| HybridAnalysis | 7 |
| JoeSandbox | 2 |

The beauty of custom metrics is that they can be easily displayed in visual form on the dashboard.

## Example use-cases

Use-cases for custom metrics are almost limitless, but here are few examples.

### Tracking App Usage

If you are using spaces apps in ThreatConnect, you may want to keep track of which apps your team is using. To do this, you can setup a keyed metric that will keep a count of how many times each spaces app is used.

### Validating Investments

Custom metrics can be used to validate investments in a variety of ways. For example, one could keep a running count of all data created by a firewall or defensive device. This would allow you to track activity and even compare different devices.

### Tracking Quotas

Many systems, like malware analysis engines and scanners, have a daily and/or monthly quota. Custom metrics can help you keep track of quotas. For example, if you have a daily quota of 10 submissions to a system, you could increment a custom metric every time you use a submission. This way if you want to know how many submissions you have used, you can simply [check the value of the metric](https://pb-constructs.hightower.space/playbooks/constructs/get_metric_value).

## Resources

API documentation for custom metrics can be found [here](https://docs.threatconnect.com/en/latest/rest_api/custom_metrics/custom_metrics.html#custom-metrics).
