# cisecurity-aws-templates
Scripts and Cloudformation templates for the CISecurity Amazon Web Services Benchmark

This repository is not reviewed, authorized, or endorsed by CISecurity. Use at your own risk.

Two CloudFormation stacks are included.
* `2.xCloudtrail.json` Creates the Section 2 Cloudtrail configuration including S3 bucket, Cloudwatch Log Group and KMS keys.
* `3.xCloudTrailMetrics.json` Depends on the above Cloudtrail configuation.  Creates Cloudwatch metrics, alarms, and a SNS topic to receive the alarms.

It is up to the user to add an appropriate subscriptio to the SNS topic, such as the related security team's email address.
