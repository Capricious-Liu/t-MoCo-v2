We only provide code for t-MoCo, since our modification is very straightforward. 
The t-MoCo only changes the loss function, and the corresponding modifications can be found in line 318 to 345 in moco/builder.py.
The same change can be directly made to SimCLR to produce t-SimCLR.

The simulation can be run through script/moco_tsne_pena0_tdf10_t5.sh