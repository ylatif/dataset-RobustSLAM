Dataset for Robust SLAM backend Evaluation
----


This dataset has been derived from the first 10 sequences of the Kitti Vision bechmark [1]. Visual odometry has been calculate using libviso2 [2] at 10Hz and Loop closures have been identified from the right image of each stereo pair at 2Hz (every fifth image) using DLoopDetector [3].

Each sequence is contained in a directory representing the sequence number (00,02,...). With each directory the following files can be found :
    
- kitii\_??\_odom.g2o : Extracted Odometry for Sequence ??
- kitti\_??\_GT.g2o   : Ground truth poses obtained from Ground Truth provided by [1].
- kitti\_??\_odom\_GT\_LC : Odometry along with Ground truth loop closures
- kitti\_??\_alpha\_f.ff.g2o : Odometry along with loop closures at the alpha value of f.ff (0.00 to 1.00)
- kitti\_??\_alpha\_F.FF\_GT\_LC.txt : Ground truth loop closures for the sequence ?? at f.ff value of alpha



- [1]: [http://www.cvlibs.net/datasets/kitti/eval_odometry.php](http://www.cvlibs.net/datasets/kitti/eval_odometry.php)
- [2]: [http://www.cvlibs.net/software/libviso/](http://www.cvlibs.net/software/libviso/)
- [3]: [http://webdiis.unizar.es/~dorian/index.php?p=33](http://webdiis.unizar.es/~dorian/index.php?p=33)


For any queries and/or suggestions please email me : ylatif [AT] unizar dot es