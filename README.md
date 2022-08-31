Please note that this problem is currently solved - but it would be nice to prevent this from happening again.

___

Some tia devs had git inconsistencies due to case-sensitivity problems. The remote repo uses a Linux logic and sees for instance F9111.fmb and f9111.fmb as two different items, while the local developer machine uses Windows logic and sees those items as identical. Consequently, one item is deleted, and the dev is blocked.

It would be nice if we could align our file naming practices and prevent this problem.

Potential solutions

·         align Git and Dimension by only using lower case letters

·         set up a control mechanism in our pipeline that blocks files with capital letters - like some kind of test

·         create a pre-commit git hook which verifies that items have lower case letters

·         enable case sensitivety on dev computers

·         document procedure for item naming in a shared dev handbook

See https://almbrand.atlassian.net/browse/TU-655 for more info

Please contact me if you need any clarifications. I need technical knowledge here, but my dev colleagues Lukas and Grzegorz can help