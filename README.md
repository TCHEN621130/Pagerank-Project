# Pagerank-Project
In this project, I am creating a search engine for the website (https://www.lawfaremedia.org/) that provides legal analysis on US national security issues. I will use Pagerank to return only the most important results from this website in my search engine.

# Submission
Task 1, part 1:

``` 
    $ python3 pagerank.py --data=data/small.csv.gz --verbose
    INFO:root:rank=0 pagerank=2.1634e+00 url=4
    INFO:root:rank=1 pagerank=1.6664e+00 url=6
    INFO:root:rank=2 pagerank=1.2402e+00 url=5
    INFO:root:rank=3 pagerank=4.5712e-01 url=2
    INFO:root:rank=4 pagerank=3.5620e-01 url=3
    INFO:root:rank=5 pagerank=3.2078e-01 url=1
```

Task 1, part 2:

```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='corona'
    INFO:root:rank=0 pagerank=4.5865e-03 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
    INFO:root:rank=1 pagerank=4.0464e-03 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
    INFO:root:rank=2 pagerank=2.6118e-03 url=www.lawfareblog.com/britains-coronavirus-response
    INFO:root:rank=3 pagerank=2.5392e-03 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
    INFO:root:rank=4 pagerank=2.3560e-03 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
    INFO:root:rank=5 pagerank=2.2897e-03 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
    INFO:root:rank=6 pagerank=2.2729e-03 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response
    INFO:root:rank=7 pagerank=2.2522e-03 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
    INFO:root:rank=8 pagerank=2.1880e-03 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
    INFO:root:rank=9 pagerank=2.0341e-03 url=www.lawfareblog.com/cyberlaw-podcast-how-israel-fighting-coronavirus

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='trump'
    INFO:root:rank=0 pagerank=6.6250e-02 url=www.lawfareblog.com/donald-trump-and-politically-weaponized-executive-branch
    INFO:root:rank=1 pagerank=6.0200e-02 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
    INFO:root:rank=2 pagerank=3.4972e-02 url=www.lawfareblog.com/trump-administrations-worrying-new-policy-israeli-settlements
    INFO:root:rank=3 pagerank=3.2196e-02 url=www.lawfareblog.com/document-trump-revokes-obama-executive-order-counterterrorism-strike-casualty-reporting
    INFO:root:rank=4 pagerank=3.0974e-02 url=www.lawfareblog.com/dc-circuit-overrules-district-courts-due-process-ruling-qasim-v-trump
    INFO:root:rank=5 pagerank=2.8463e-02 url=www.lawfareblog.com/how-trumps-approach-middle-east-ignores-past-future-and-human-condition
    INFO:root:rank=6 pagerank=2.5255e-02 url=www.lawfareblog.com/why-trump-cant-buy-greenland
    INFO:root:rank=7 pagerank=2.2459e-02 url=www.lawfareblog.com/oral-argument-summary-qassim-v-trump
    INFO:root:rank=8 pagerank=2.1464e-02 url=www.lawfareblog.com/dc-circuit-court-denies-trump-rehearing-mazars-case
    INFO:root:rank=9 pagerank=2.1105e-02 url=www.lawfareblog.com/second-circuit-rules-mazars-must-hand-over-trump-tax-returns-new-york-prosecutors

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='iran'
    INFO:root:rank=0 pagerank=6.6138e-02 url=www.lawfareblog.com/praise-presidents-iran-tweets
    INFO:root:rank=1 pagerank=2.9202e-02 url=www.lawfareblog.com/how-us-iran-tensions-could-disrupt-iraqs-fragile-peace
    INFO:root:rank=2 pagerank=1.7711e-02 url=www.lawfareblog.com/cyber-command-operational-update-clarifying-june-2019-iran-operation
    INFO:root:rank=3 pagerank=1.4606e-02 url=www.lawfareblog.com/aborted-iran-strike-fine-line-between-necessity-and-revenge
    INFO:root:rank=4 pagerank=8.4519e-03 url=www.lawfareblog.com/iranian-hostage-crisis-and-its-effect-american-politics
    INFO:root:rank=5 pagerank=8.3997e-03 url=www.lawfareblog.com/parsing-state-departments-letter-use-force-against-iran
    INFO:root:rank=6 pagerank=8.2589e-03 url=www.lawfareblog.com/announcing-united-states-and-use-force-against-iran-new-lawfare-e-book
    INFO:root:rank=7 pagerank=8.0568e-03 url=www.lawfareblog.com/trump-moves-cut-irans-oil-revenues-whats-his-endgame
    INFO:root:rank=8 pagerank=7.1946e-03 url=www.lawfareblog.com/us-names-iranian-revolutionary-guard-terrorist-organization-and-sanctions-international-criminal
    INFO:root:rank=9 pagerank=5.9410e-03 url=www.lawfareblog.com/iran-shoots-down-us-drone-domestic-and-international-legal-implications
```

Task 1, part 3:

```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz
    INFO:root:rank=0 pagerank=8.4165e+00 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
    INFO:root:rank=1 pagerank=8.4165e+00 url=www.lawfareblog.com/lawfare-job-board
    INFO:root:rank=2 pagerank=8.4165e+00 url=www.lawfareblog.com/masthead
    INFO:root:rank=3 pagerank=8.4165e+00 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
    INFO:root:rank=4 pagerank=8.4165e+00 url=www.lawfareblog.com/subscribe-lawfare
    INFO:root:rank=5 pagerank=8.4165e+00 url=www.lawfareblog.com/our-comments-policy
    INFO:root:rank=6 pagerank=8.4165e+00 url=www.lawfareblog.com/upcoming-events
    INFO:root:rank=7 pagerank=8.4165e+00 url=www.lawfareblog.com/support-lawfare
    INFO:root:rank=8 pagerank=8.4165e+00 url=www.lawfareblog.com/snowden-revelations
    INFO:root:rank=9 pagerank=8.4165e+00 url=www.lawfareblog.com/topics

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2
    INFO:root:rank=0 pagerank=4.6096e+00 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
    INFO:root:rank=1 pagerank=2.9870e+00 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
    INFO:root:rank=2 pagerank=2.9672e+00 url=www.lawfareblog.com/opening-statement-david-holmes
    INFO:root:rank=3 pagerank=2.0175e+00 url=www.lawfareblog.com/senate-examines-threats-homeland
    INFO:root:rank=4 pagerank=1.8771e+00 url=www.lawfareblog.com/what-make-first-day-impeachment-hearings
    INFO:root:rank=5 pagerank=1.8764e+00 url=www.lawfareblog.com/livestream-house-armed-services-committee-hearing-f-35-program
    INFO:root:rank=6 pagerank=1.8695e+00 url=www.lawfareblog.com/whats-house-resolution-impeachment
    INFO:root:rank=7 pagerank=1.7657e+00 url=www.lawfareblog.com/congress-us-policy-toward-syria-and-turkey-overview-recent-hearings
    INFO:root:rank=8 pagerank=1.6809e+00 url=www.lawfareblog.com/summary-david-holmess-deposition-testimony
    INFO:root:rank=9 pagerank=9.8355e-01 url=www.lawfareblog.com/events
```

Task 1, part 4:

```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose 
    INFO:root:rank=0 pagerank=8.4165e+00 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
    INFO:root:rank=1 pagerank=8.4165e+00 url=www.lawfareblog.com/lawfare-job-board
    INFO:root:rank=2 pagerank=8.4165e+00 url=www.lawfareblog.com/masthead
    INFO:root:rank=3 pagerank=8.4165e+00 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
    INFO:root:rank=4 pagerank=8.4165e+00 url=www.lawfareblog.com/subscribe-lawfare
    INFO:root:rank=5 pagerank=8.4165e+00 url=www.lawfareblog.com/our-comments-policy
    INFO:root:rank=6 pagerank=8.4165e+00 url=www.lawfareblog.com/upcoming-events
    INFO:root:rank=7 pagerank=8.4165e+00 url=www.lawfareblog.com/support-lawfare
    INFO:root:rank=8 pagerank=8.4165e+00 url=www.lawfareblog.com/snowden-revelations
    INFO:root:rank=9 pagerank=8.4165e+00 url=www.lawfareblog.com/topics

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --alpha=0.99999
    INFO:root:rank=0 pagerank=1.0624e+01 url=www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
    INFO:root:rank=1 pagerank=1.0624e+01 url=www.lawfareblog.com/lawfare-job-board
    INFO:root:rank=2 pagerank=1.0624e+01 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
    INFO:root:rank=3 pagerank=1.0624e+01 url=www.lawfareblog.com/subscribe-lawfare
    INFO:root:rank=4 pagerank=1.0624e+01 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
    INFO:root:rank=5 pagerank=1.0624e+01 url=www.lawfareblog.com/our-comments-policy
    INFO:root:rank=6 pagerank=1.0624e+01 url=www.lawfareblog.com/upcoming-events
    INFO:root:rank=7 pagerank=1.0624e+01 url=www.lawfareblog.com/support-lawfare
    INFO:root:rank=8 pagerank=1.0624e+01 url=www.lawfareblog.com/snowden-revelations
    INFO:root:rank=9 pagerank=1.0624e+01 url=www.lawfareblog.com/topics

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2
    INFO:root:rank=0 pagerank=4.6096e+00 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
    INFO:root:rank=1 pagerank=2.9870e+00 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
    INFO:root:rank=2 pagerank=2.9672e+00 url=www.lawfareblog.com/opening-statement-david-holmes
    INFO:root:rank=3 pagerank=2.0175e+00 url=www.lawfareblog.com/senate-examines-threats-homeland
    INFO:root:rank=4 pagerank=1.8771e+00 url=www.lawfareblog.com/what-make-first-day-impeachment-hearings
    INFO:root:rank=5 pagerank=1.8764e+00 url=www.lawfareblog.com/livestream-house-armed-services-committee-hearing-f-35-program
    INFO:root:rank=6 pagerank=1.8695e+00 url=www.lawfareblog.com/whats-house-resolution-impeachment
    INFO:root:rank=7 pagerank=1.7657e+00 url=www.lawfareblog.com/congress-us-policy-toward-syria-and-turkey-overview-recent-hearings
    INFO:root:rank=8 pagerank=1.6809e+00 url=www.lawfareblog.com/summary-david-holmess-deposition-testimony
    INFO:root:rank=9 pagerank=9.8355e-01 url=www.lawfareblog.com/events

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
    INFO:root:rank=0 pagerank=5.2386e+01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
    INFO:root:rank=1 pagerank=5.2386e+01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
    INFO:root:rank=2 pagerank=7.9439e+00 url=www.lawfareblog.com/cost-using-zero-days
    INFO:root:rank=3 pagerank=2.3700e+00 url=www.lawfareblog.com/lawfare-podcast-former-congressman-brian-baird-and-daniel-schuman-how-congress-can-continue-function
    INFO:root:rank=4 pagerank=1.5530e+00 url=www.lawfareblog.com/events
    INFO:root:rank=5 pagerank=1.1867e+00 url=www.lawfareblog.com/water-wars-increased-us-focus-indo-pacific
    INFO:root:rank=6 pagerank=1.1867e+00 url=www.lawfareblog.com/water-wars-drill-maybe-drill
    INFO:root:rank=7 pagerank=1.1867e+00 url=www.lawfareblog.com/water-wars-disjointed-operations-south-china-sea
    INFO:root:rank=8 pagerank=1.1867e+00 url=www.lawfareblog.com/water-wars-sinking-feeling-philippine-china-relations
    INFO:root:rank=9 pagerank=1.1867e+00 url=www.lawfareblog.com/water-wars-us-china-divide-shangri-la
```

Task 2, part 1:
```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona' --search_query='-corona'
    INFO:root:rank=0 pagerank=8.8870e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
    INFO:root:rank=1 pagerank=8.8867e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
    INFO:root:rank=2 pagerank=1.8256e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
    INFO:root:rank=3 pagerank=1.4907e-01 url=www.lawfareblog.com/rational-security-my-corona-edition
    INFO:root:rank=4 pagerank=1.4907e-01 url=www.lawfareblog.com/brexit-not-immune-coronavirus
    INFO:root:rank=5 pagerank=1.0729e-01 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
    INFO:root:rank=6 pagerank=1.0199e-01 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
    INFO:root:rank=7 pagerank=1.0199e-01 url=www.lawfareblog.com/britains-coronavirus-response
    INFO:root:rank=8 pagerank=9.4298e-02 url=www.lawfareblog.com/lawfare-podcast-mom-and-dad-talk-clinical-trials-pandemic
    INFO:root:rank=9 pagerank=8.7207e-02 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response 

    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --search_query='corona'
    INFO:root:rank=0 pagerank=1.2503e-01 url=www.lawfareblog.com/congress-needs-coronavirus-failsafe-its-too-late
    INFO:root:rank=1 pagerank=6.0753e-02 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response        
    INFO:root:rank=2 pagerank=5.4779e-02 url=www.lawfareblog.com/britains-coronavirus-response
    INFO:root:rank=3 pagerank=5.4402e-02 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
    INFO:root:rank=4 pagerank=5.1763e-02 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response     
    INFO:root:rank=5 pagerank=5.1451e-02 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns  
    INFO:root:rank=6 pagerank=4.7124e-02 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
    INFO:root:rank=7 pagerank=2.7823e-02 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
    INFO:root:rank=8 pagerank=2.7441e-02 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
    INFO:root:rank=9 pagerank=2.0547e-02 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
```

Task 2, part 2:
```
    $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona' --search_query='-corona'
    INFO:root:rank=0 pagerank=8.8870e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
    INFO:root:rank=1 pagerank=8.8867e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
    INFO:root:rank=2 pagerank=1.8256e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
    INFO:root:rank=3 pagerank=1.0729e-01 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
    INFO:root:rank=4 pagerank=9.4298e-02 url=www.lawfareblog.com/lawfare-podcast-mom-and-dad-talk-clinical-trials-pandemic
    INFO:root:rank=5 pagerank=7.9633e-02 url=www.lawfareblog.com/fault-lines-foreign-policy-quarantined
    INFO:root:rank=6 pagerank=7.5307e-02 url=www.lawfareblog.com/limits-world-health-organization
    INFO:root:rank=7 pagerank=6.8115e-02 url=www.lawfareblog.com/chinatalk-dispatches-shanghai-beijing-and-hong-kong
    INFO:root:rank=8 pagerank=6.4847e-02 url=www.lawfareblog.com/us-moves-dismiss-case-against-company-linked-ira-troll-farm
    INFO:root:rank=9 pagerank=6.4847e-02 url=www.lawfareblog.com/livestream-house-armed-services-holds-hearing-national-security-challenges-north-and-south-america
```
