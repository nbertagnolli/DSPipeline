# DSPipeline
This is a prototype repository.  It holds some example code for a prototype of an automated
Data Science Pipeline.  The idea is two fold. And entirely based off of what Damien Patton
described to me during an interview.  This is my meger attempt at replicating the idea.

1. Have a model staging area
2. Have a system which automatically adjusts train test sets with new data.

The workflow for a datascientist should be to create models.  Models go into an "arena"
where they are all trained on the entire data set and tested on the most recent data.
The best model is then automatically selected and put into production.  As new data comes
in the old test set is added to the training set for all models in the staging area to retrain
on and the new data is used as the test set. 
