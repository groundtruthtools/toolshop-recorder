# toolshop-recorder

The nightly scheduler for the hiring history behind companyfacts.dev and the
groundtruth Apify Actors.

Once a day it reads the public job boards of about 7,500 companies on
Greenhouse, Ashby, Workable and Lever (one request every 2 seconds per
system), records which jobs appeared, changed or closed, and publishes the
day's job feeds. The code is in a private repository; this one holds the
schedule and `status/last-run.json`, a summary of the latest run (boards read,
boards failed, jobs new, removed and changed).

Questions about the data: see https://companyfacts.dev.
