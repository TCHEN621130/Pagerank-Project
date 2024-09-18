# Pagerank-Project
In this project, I am creating a search engine for the website (https://www.lawfaremedia.org/) that provides legal analysis on US national security issues. I will use Pagerank to return only the most important results from this website in my search engine.

# Submission
Task 1, part 1:

``` 
    $ python3 pagerank.py --data=data/small.csv.gz --verbose
    INFO:root:rank=0 pagerank=8.5429e-01 url=4
    INFO:root:rank=1 pagerank=6.7512e-01 url=6
    INFO:root:rank=2 pagerank=5.4108e-01 url=5
    INFO:root:rank=3 pagerank=3.1644e-01 url=2
    INFO:root:rank=4 pagerank=2.5502e-01 url=3
    INFO:root:rank=5 pagerank=2.3246e-01 url=1
```

Task 1, part 2:

```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='corona'
    INFO:root:rank=0 pagerank=3.9236e-03 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
    INFO:root:rank=1 pagerank=3.4359e-03 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
    INFO:root:rank=2 pagerank=2.3217e-03 url=www.lawfareblog.com/britains-coronavirus-response
    INFO:root:rank=3 pagerank=2.2610e-03 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
    INFO:root:rank=4 pagerank=2.1226e-03 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
    INFO:root:rank=5 pagerank=2.0721e-03 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
    INFO:root:rank=6 pagerank=2.0332e-03 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
    INFO:root:rank=7 pagerank=1.9729e-03 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
    INFO:root:rank=8 pagerank=1.9693e-03 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response
    INFO:root:rank=9 pagerank=1.8279e-03 url=www.lawfareblog.com/house-subcommittee-voices-concerns-over-us-management-coronavirus

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='trump'
    INFO:root:rank=0 pagerank=4.2801e-02 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
    INFO:root:rank=1 pagerank=3.4683e-02 url=www.lawfareblog.com/donald-trump-and-politically-weaponized-executive-branch
    INFO:root:rank=2 pagerank=2.7849e-02 url=www.lawfareblog.com/trump-administrations-worrying-new-policy-israeli-settlements
    INFO:root:rank=3 pagerank=2.6351e-02 url=www.lawfareblog.com/document-trump-revokes-obama-executive-order-counterterrorism-strike-casualty-reporting
    INFO:root:rank=4 pagerank=2.4786e-02 url=www.lawfareblog.com/dc-circuit-overrules-district-courts-due-process-ruling-qasim-v-trump
    INFO:root:rank=5 pagerank=2.2742e-02 url=www.lawfareblog.com/how-trumps-approach-middle-east-ignores-past-future-and-human-condition
    INFO:root:rank=6 pagerank=2.0582e-02 url=www.lawfareblog.com/why-trump-cant-buy-greenland
    INFO:root:rank=7 pagerank=1.8467e-02 url=www.lawfareblog.com/oral-argument-summary-qassim-v-trump
    INFO:root:rank=8 pagerank=1.7373e-02 url=www.lawfareblog.com/dc-circuit-court-denies-trump-rehearing-mazars-case
    INFO:root:rank=9 pagerank=1.7181e-02 url=www.lawfareblog.com/second-circuit-rules-mazars-must-hand-over-trump-tax-returns-new-york-prosecutors

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='iran'
    INFO:root:rank=0 pagerank=3.4590e-02 url=www.lawfareblog.com/praise-presidents-iran-tweets
    INFO:root:rank=1 pagerank=2.3338e-02 url=www.lawfareblog.com/how-us-iran-tensions-could-disrupt-iraqs-fragile-peace
    INFO:root:rank=2 pagerank=1.4032e-02 url=www.lawfareblog.com/cyber-command-operational-update-clarifying-june-2019-iran-operation
    INFO:root:rank=3 pagerank=1.1128e-02 url=www.lawfareblog.com/aborted-iran-strike-fine-line-between-necessity-and-revenge
    INFO:root:rank=4 pagerank=6.9530e-03 url=www.lawfareblog.com/iranian-hostage-crisis-and-its-effect-american-politics
    INFO:root:rank=5 pagerank=6.9320e-03 url=www.lawfareblog.com/parsing-state-departments-letter-use-force-against-iran
    INFO:root:rank=6 pagerank=6.8211e-03 url=www.lawfareblog.com/announcing-united-states-and-use-force-against-iran-new-lawfare-e-book
    INFO:root:rank=7 pagerank=6.0697e-03 url=www.lawfareblog.com/us-names-iranian-revolutionary-guard-terrorist-organization-and-sanctions-international-criminal
    INFO:root:rank=8 pagerank=5.8303e-03 url=www.lawfareblog.com/trump-moves-cut-irans-oil-revenues-whats-his-endgame
    INFO:root:rank=9 pagerank=4.9612e-03 url=www.lawfareblog.com/iran-shoots-down-us-drone-domestic-and-international-legal-implications
```

Task 1, part 3:

```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz
    INFO:root:rank=0 pagerank=3.6346e+00 url=www.lawfareblog.com/our-comments-policy
    INFO:root:rank=1 pagerank=3.6346e+00 url=www.lawfareblog.com/lawfare-job-board
    INFO:root:rank=2 pagerank=3.6346e+00 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
    INFO:root:rank=3 pagerank=3.6346e+00 url=www.lawfareblog.com/subscribe-lawfare
    INFO:root:rank=4 pagerank=3.6346e+00 url=www.lawfareblog.com/support-lawfare
    INFO:root:rank=5 pagerank=3.6346e+00 url=www.lawfareblog.com/upcoming-events
    INFO:root:rank=6 pagerank=3.6346e+00 url=www.lawfareblog.com/snowden-revelations
    INFO:root:rank=7 pagerank=3.6346e+00 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
    INFO:root:rank=8 pagerank=3.6346e+00 url=www.lawfareblog.com/topics
    INFO:root:rank=9 pagerank=3.6346e+00 url=www.lawfareblog.com/documents-related-mueller-investigation

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2
    INFO:root:rank=0 pagerank=1.5650e+00 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
    INFO:root:rank=1 pagerank=1.1968e+00 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
    INFO:root:rank=2 pagerank=1.1837e+00 url=www.lawfareblog.com/opening-statement-david-holmes
    INFO:root:rank=3 pagerank=5.6602e-01 url=www.lawfareblog.com/summary-david-holmess-deposition-testimony
    INFO:root:rank=4 pagerank=5.6297e-01 url=www.lawfareblog.com/senate-examines-threats-homeland
    INFO:root:rank=5 pagerank=4.8742e-01 url=www.lawfareblog.com/what-make-first-day-impeachment-hearings
    INFO:root:rank=6 pagerank=4.8691e-01 url=www.lawfareblog.com/livestream-house-armed-services-committee-hearing-f-35-program
    INFO:root:rank=7 pagerank=4.8294e-01 url=www.lawfareblog.com/whats-house-resolution-impeachment
    INFO:root:rank=8 pagerank=4.4849e-01 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
    INFO:root:rank=9 pagerank=4.4788e-01 url=www.lawfareblog.com/congress-us-policy-toward-syria-and-turkey-overview-recent-hearings
```

Task 1, part 4:

```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose 
    INFO:root:rank=0 pagerank=3.6346e+00 url=www.lawfareblog.com/our-comments-policy
    INFO:root:rank=1 pagerank=3.6346e+00 url=www.lawfareblog.com/lawfare-job-board
    INFO:root:rank=2 pagerank=3.6346e+00 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
    INFO:root:rank=3 pagerank=3.6346e+00 url=www.lawfareblog.com/subscribe-lawfare
    INFO:root:rank=4 pagerank=3.6346e+00 url=www.lawfareblog.com/support-lawfare
    INFO:root:rank=5 pagerank=3.6346e+00 url=www.lawfareblog.com/upcoming-events
    INFO:root:rank=6 pagerank=3.6346e+00 url=www.lawfareblog.com/snowden-revelations
    INFO:root:rank=7 pagerank=3.6346e+00 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
    INFO:root:rank=8 pagerank=3.6346e+00 url=www.lawfareblog.com/topics
    INFO:root:rank=9 pagerank=3.6346e+00 url=www.lawfareblog.com/documents-related-mueller-investigation

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --alpha=0.99999
    INFO:root:rank=0 pagerank=1.0519e+01 url=www.lawfareblog.com/masthead
    INFO:root:rank=1 pagerank=1.0519e+01 url=www.lawfareblog.com/lawfare-job-board
    INFO:root:rank=2 pagerank=1.0519e+01 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
    INFO:root:rank=3 pagerank=1.0519e+01 url=www.lawfareblog.com/subscribe-lawfare
    INFO:root:rank=4 pagerank=1.0519e+01 url=www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
    INFO:root:rank=5 pagerank=1.0519e+01 url=www.lawfareblog.com/our-comments-policy
    INFO:root:rank=6 pagerank=1.0519e+01 url=www.lawfareblog.com/upcoming-events
    INFO:root:rank=7 pagerank=1.0519e+01 url=www.lawfareblog.com/support-lawfare
    INFO:root:rank=8 pagerank=1.0519e+01 url=www.lawfareblog.com/snowden-revelations
    INFO:root:rank=9 pagerank=1.0519e+01 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2
    INFO:root:rank=0 pagerank=1.5650e+00 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
    INFO:root:rank=1 pagerank=1.1968e+00 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
    INFO:root:rank=2 pagerank=1.1837e+00 url=www.lawfareblog.com/opening-statement-david-holmes
    INFO:root:rank=3 pagerank=5.6602e-01 url=www.lawfareblog.com/summary-david-holmess-deposition-testimony
    INFO:root:rank=4 pagerank=5.6297e-01 url=www.lawfareblog.com/senate-examines-threats-homeland
    INFO:root:rank=5 pagerank=4.8742e-01 url=www.lawfareblog.com/what-make-first-day-impeachment-hearings
    INFO:root:rank=6 pagerank=4.8691e-01 url=www.lawfareblog.com/livestream-house-armed-services-committee-hearing-f-35-program
    INFO:root:rank=7 pagerank=4.8294e-01 url=www.lawfareblog.com/whats-house-resolution-impeachment
    INFO:root:rank=8 pagerank=4.4849e-01 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
    INFO:root:rank=9 pagerank=4.4788e-01 url=www.lawfareblog.com/congress-us-policy-toward-syria-and-turkey-overview-recent-hearings

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
    INFO:root:rank=0 pagerank=5.1867e+01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
    INFO:root:rank=1 pagerank=5.1867e+01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
    INFO:root:rank=2 pagerank=7.8653e+00 url=www.lawfareblog.com/cost-using-zero-days
    INFO:root:rank=3 pagerank=2.3464e+00 url=www.lawfareblog.com/lawfare-podcast-former-congressman-brian-baird-and-daniel-schuman-how-congress-can-continue-function
    INFO:root:rank=4 pagerank=1.5375e+00 url=www.lawfareblog.com/events
    INFO:root:rank=5 pagerank=1.1749e+00 url=www.lawfareblog.com/water-wars-increased-us-focus-indo-pacific
    INFO:root:rank=6 pagerank=1.1749e+00 url=www.lawfareblog.com/water-wars-drill-maybe-drill
    INFO:root:rank=7 pagerank=1.1749e+00 url=www.lawfareblog.com/water-wars-disjointed-operations-south-china-sea
    INFO:root:rank=8 pagerank=1.1749e+00 url=www.lawfareblog.com/water-wars-us-china-divide-shangri-la
    INFO:root:rank=9 pagerank=1.1749e+00 url=www.lawfareblog.com/water-wars-sinking-feeling-philippine-china-relations
```
