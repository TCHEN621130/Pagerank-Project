# Pagerank-Project
In this project, I am creating a search engine for the website (https://www.lawfaremedia.org/) that provides legal analysis on US national security issues. I will use Pagerank to return only the most important results from this website in my search engine.

# Submission
Task 1, part 1:

``` 
    $ python3 pagerank.py --data=data/small.csv.gz --verbose

    DEBUG:root:computing indices
    DEBUG:root:computing values
    C:\Users\teren\OneDrive\Desktop\HMC\3) Junior\Data Mining\Pagerank-Project\pagerank.py:73: UserWarning: torch.sparse.SparseTensor(indices, values, shape, *, device=) is deprecated.  Please use torch.sparse_coo_tensor(indices, values, shape, dtype=, device=). (Triggered internally at C:\actions-runner\_work\pytorch\pytorch\builder\windows\pytorch\torch\csrc\utils\tensor_new.cpp:643.)
    self.P = torch.sparse.FloatTensor(i, v, torch.Size([n,n]))
    DEBUG:root:i=0 residual=0.2869156002998352
    DEBUG:root:i=1 residual=0.17673587799072266
    DEBUG:root:i=2 residual=0.11748470366001129
    DEBUG:root:i=3 residual=0.061109527945518494
    DEBUG:root:i=4 residual=0.038023941218853
    DEBUG:root:i=5 residual=0.018694842234253883
    DEBUG:root:i=6 residual=0.011767178773880005
    DEBUG:root:i=7 residual=0.009790820069611073
    DEBUG:root:i=8 residual=0.01014517992734909
    DEBUG:root:i=9 residual=0.010316635482013226
    DEBUG:root:i=10 residual=0.00993178877979517
    DEBUG:root:i=11 residual=0.009173526428639889
    DEBUG:root:i=12 residual=0.008200429379940033
    DEBUG:root:i=13 residual=0.007159791421145201
    DEBUG:root:i=14 residual=0.006137470249086618
    DEBUG:root:i=15 residual=0.005187023431062698
    DEBUG:root:i=16 residual=0.004333975724875927
    DEBUG:root:i=17 residual=0.0035879577044397593
    DEBUG:root:i=18 residual=0.0029477779753506184
    DEBUG:root:i=19 residual=0.0024063601158559322
    DEBUG:root:i=20 residual=0.001953764818608761
    DEBUG:root:i=21 residual=0.0015790157485753298
    DEBUG:root:i=22 residual=0.0012710248120129108
    DEBUG:root:i=23 residual=0.0010196113726124167
    DEBUG:root:i=24 residual=0.0008153740200214088
    DEBUG:root:i=25 residual=0.000650388712529093
    DEBUG:root:i=26 residual=0.0005175543483346701
    DEBUG:root:i=27 residual=0.0004110064182896167
    DEBUG:root:i=28 residual=0.00032570521580055356
    DEBUG:root:i=29 residual=0.0002577237319201231
    DEBUG:root:i=30 residual=0.00020367132674437016
    DEBUG:root:i=31 residual=0.00016063386283349246
    DEBUG:root:i=32 residual=0.0001265958562726155
    DEBUG:root:i=33 residual=9.965635399566963e-05
    DEBUG:root:i=34 residual=7.833473500795662e-05
    DEBUG:root:i=35 residual=6.153235153760761e-05
    DEBUG:root:i=36 residual=4.832382910535671e-05
    DEBUG:root:i=37 residual=3.799118348979391e-05
    DEBUG:root:i=38 residual=2.9711076422245242e-05
    DEBUG:root:i=39 residual=2.3324044377659447e-05
    DEBUG:root:i=40 residual=1.8230430214316584e-05
    DEBUG:root:i=41 residual=1.4268070117395837e-05
    DEBUG:root:i=42 residual=1.1168278433615342e-05
    DEBUG:root:i=43 residual=8.670030183566269e-06
    DEBUG:root:i=44 residual=6.788734026486054e-06
    DEBUG:root:i=45 residual=5.372772648115642e-06
    DEBUG:root:i=46 residual=4.164867732470157e-06
    DEBUG:root:i=47 residual=3.2266434573102742e-06
    DEBUG:root:i=48 residual=2.5501456093479646e-06
    DEBUG:root:i=49 residual=1.9844856069539674e-06
    DEBUG:root:i=50 residual=1.537638127047103e-06
    DEBUG:root:i=51 residual=1.2043236665704171e-06
    DEBUG:root:i=52 residual=8.70921553541848e-07
    INFO:root:rank=0 pagerank=8.5429e-01 url=4
    INFO:root:rank=1 pagerank=6.7512e-01 url=6
    INFO:root:rank=2 pagerank=5.4108e-01 url=5
    INFO:root:rank=3 pagerank=3.1644e-01 url=2
    INFO:root:rank=4 pagerank=2.5502e-01 url=3
    INFO:root:rank=5 pagerank=2.3246e-01 url=1
```

