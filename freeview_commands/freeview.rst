freeview -v \
011_S_4075_tp0/mri/T1.mgz \
011_S_4075_tp0/mri/wm.mgz \
011_S_4075_tp0/mri/brainmask.mgz \
011_S_4075_tp0/mri/aseg.mgz:colormap=lut:opacity=0.2 \
-f 011_S_4075_tp0/surf/lh.white:edgecolor=blue \
011_S_4075_tp0/surf/lh.pial:edgecolor=red \
011_S_4075_tp0/surf/rh.white:edgecolor=blue \
011_S_4075_tp0/surf/rh.pial:edgecolor=red


freeview -f 011_S_4075_tp0/surf/lh.pial:annot=aparc.annot:name=pial_aparc:visible=0 \
011_S_4075_tp0/surf/lh.pial:annot=aparc.a2009s.annot:name=pial_aparc_des:visible=0 \
011_S_4075_tp0/surf/lh.inflated:overlay=lh.thickness:overlay_threshold=0.1,3::name=inflated_thickness:visible=0 \
011_S_4075_tp0/surf/lh.inflated:visible=0 \
011_S_4075_tp0/surf/lh.white:visible=0 \
011_S_4075_tp0/surf/lh.pial \
--viewport 3d
