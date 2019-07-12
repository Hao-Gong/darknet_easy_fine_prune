# darknet_project_privat

I set a accumulational prune step. You can only prune it on a trained model. Using the same .cfg file and some prune params like:

[convolutional]

prune=1  //enable prune

prune_threshold_min=0.0001  //start prune threshold

prune_threshold_max=0.0005  //end prune threshold

prune_add_step=5000 // each epoch add (prune_threshold_max-prune_threshold_min)/prune_add_step

batch_normalize=1

filters=16

size=3

stride=1

pad=1

activation=leaky

