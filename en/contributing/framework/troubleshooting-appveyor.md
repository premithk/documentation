# Troubleshooting AppVeyor

## Waiting for status to be reported
Ugh, isn't this annoying? Luckily it doesn't happen often. It happens when the Webhook payload from GitHub to AppVeyor failures for whatever reason. Luckily it's easy to fix.

![](/images/contributing/waiting-for-status-to-be-reported.png)

Navigate to Settings -> Webhooks and then click on the manage AppVeyor webhook button which will reveal this screen.

![](/images/contributing/manage-appveyor-webhook.png)

Scroll down and identify the failed payload and mash the "Redeliver" button exactly once.

![](/images/contributing/trigger-build-by-redelivering-failed-appveyor-webhook.png)

Visit AppVeyor to verify that the build has kicked off.