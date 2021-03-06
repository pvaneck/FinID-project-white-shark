# Shark Fin Image Dataset for Great White Shark Research

## Dataset
The shark Fin ID dataset currently has 47,092 images in 243 categories (i.e. 243 shark individuals). The data are hosted in a publuc AWS S3 bucket: `finid-public`.

## Summary of Numbers of Images for Fin ID
See `FinID_num_images_summary_02_17_2020.csv` for details.

## Download
AWS CLI (Command Line Interface) is recommended to download the dataset from S3 bucket. The installation instruction can be found [here](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html). To confirm the successful installation, type command `aws --version`. If you get error message: `ImportError: No module named 'awscli'`, this [resource](https://stackoverflow.com/questions/43873663/awscli-fails-to-work-no-module-named-awscli) might solve the issue.

To download, `cd` into your directory, for example `finid_dataset`, type command `aws s3 sync s3://finid-public/dataset/ .` The dataset will be downloaded to the folder `finid_dataset`. To list all objects and folders in S3 bucket, use the command `aws s3 ls s3://finid-public/`.

You can also utilize [boto3](https://github.com/boto/boto3) to download the dataset.

## Data Sharing License
The data sharing license associated with this project is CDLA-Permissive (Community Data License Agreement – Permissive – Version 1.0). The details of the license agreement can be found [here](https://cdla.io/permissive-1-0/) ([PDF version](https://cdla.io/permissive-1-0/wp-content/uploads/sites/52/2017/10/CDLA-Permissive-v1.0.pdf)). The CDLA-Permissive agreement is similar to permissive open source licenses in that the publisher of data allows anyone to use, modify and do what they want with the data with no obligations to share any of their changes or modifications.

## Contact
zacycliu@stanford.edu

## Last updated
Feb 19, 2020
