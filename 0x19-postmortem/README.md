
# Postmortem Report: AWS S3 Outage

## Issue Summary

- **Outage Duration:**  
  **Start:** 9:37 AM PST, February 28, 2017  
  **End:** 1:54 PM PST, February 28, 2017

- **Impact:**  
  AWS S3 in the US-EAST-1 region decided to take a surprise vacation, leaving 54% of the internet scrambling for their files. Major websites were left saying, “Sorry, we’re on a break,” as users encountered errors. Even the internet giants had to play the waiting game.

- **Root Cause:**  
  A classic case of “Oops, wrong server!” An innocent debugging exercise turned into a full-blown disaster movie when too many servers were taken down, including the ones holding S3’s vital information.

![Click here to visualize the domino effect.](#)

## Timeline

- **9:37 AM PST:** S3 starts acting up, and AWS monitoring tools scream, “Mayday!”
- **9:40 AM PST:** Engineers jump in, initially convinced that a rogue network cable might be to blame.
- **10:05 AM PST:** The wild goose chase begins with engineers checking every network setting they can find.
- **10:30 AM PST:** The S3 team gets the call, and suddenly, things get serious.
- **1:54 PM PST:** The lost servers are found, and S3 slowly wakes up from its unplanned nap.

## Root Cause and Resolution

- **Root Cause:**  
  It all started with a tiny human error—a command intended to debug the system ended up sending too many servers into early retirement. This took down a key part of S3 that manages where your files live, and when that went down, so did everything else.

- **Resolution:**  
  After some frantic server wrangling, the AWS team managed to bring everything back online. They also added some extra safeguards to make sure no one can accidentally send half the internet into chaos again.

## Corrective and Preventative Measures

- **Improvements:**  
  If there’s one thing we learned, it’s that commands are like lightsabers—handle with care. We’ve tightened up the process to make sure no one can swing one around without proper checks.

- **Tasks:**
  1. Add extra guardrails around server commands to prevent unintended mass retirements.
  2. Introduce a new policy: "Think twice, click once."
  3. Set up a buddy system for critical operations—because two heads are better than one!
