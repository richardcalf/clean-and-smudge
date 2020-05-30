# clean-and-smudge
A step by step guide to clean and smudge

To clean and smudge is to have a secret on you local repo that gets replaced with a placeholder when committing, and then replaced with the secret when checking out to your local repo again.

Here is the synosis:

You have a javascript file that contains a secret, but you don't want that secret to be committed for security reasons.

You'll need to setup a configuration section that runs on the commit event, that replaces your secret with a placeholder.

You'll need a setup configuration section that runs on the merge event, that replaces the placeholder with your secret.
