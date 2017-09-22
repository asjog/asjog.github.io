---
layout: page
title: Learnings
---
## Using tksurfer for visualizing cortical thicknesses </h2>
I have just started exploring effects of scanner on surfaces and surface thicknesses produced by Freesurfer.
To that end, I needed to learn how to produce surface renderings using tksurfer on an industrial scale.
To do that using tksurfer needed me to write a Tcl script (a language that I did not existed until yesterday).
It is quite a fun language but using it I can generate figures for multiple datasets by the following command:

```
tksurfer fsaverage lh inflated -tcl tksurfer_save_abs_rel_thickness_figs.tcl -curv lh.sulc -colscalebarflag 1
```


