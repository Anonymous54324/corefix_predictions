# CoReFix Prediction Samples

This repository contains generated patches by CoReFix. All the samples are taken from the test dataset. Also, note that we published two detailed patch in Appendix.
The pathes are code reduced versions of the files to provide better visibility.
In case you want to see the full version of the files, we also included github urls. 
Each patch has a .html file highlighting the pre and post versions and .txt file containing github links

Files are named after repo and file names.
File url links should take you directly to the file and also highlight the line where the rule was reported by static analyzer.
The other url is the link to the commit.

We have all the predictions for all our experiments and models saved and would be happy to publish them.

# Structure of the repo for a single rule

├── AmbiguousConditional \
│   ├── *.html // delta for pre_code and model prediction \
│   ├── *.txt// contains github urls \
│   ├── ...
└── README.md 


# How to view the samples?

1. Clone this repo
2. You can now open the html files in your local browser. Simply click and go thorught the files in your favorite file explorer app as you wish

# Note about GitHub URLs

In rare cases github urls will not lead you to the correct place. This is not a bug in our code but it is related to how libgit library works. We do not store the full files in our dataset to save memory but fetch them on the fly via libgit. Those commit hashes work for file fetching process because libgit also has some internal logic to handle rebases, merge commits and other things. Therefore, the commit hashes we save are meant to be used for file fetching via libgit not for url creation. That's why, when used as urls, the commit shas might not lead to the right place.

In such cases, you can open the github repo, find the file (filename is provided in html files) and search the history of that file. Some of the commits close to the given commit hash must contain the presented changes.



# Rules

