Find-Who-to-Look-at
=====================
The video eye-tracking database containing the fixation data of 65 multiple-face videos from YouTube and Youku, established by Yufan Liu, Mai Xu in Beihang University (2016).

## Usage of Database
See 'our_database' for the database and eye tracking data. All fixation data are recorded in **'video_database.mat'**, where you can find

* videos_info: the information of 65 videos 

* video_names_list: the index for 65 videos

* subj_info: the information of 39 participants 

* subj_names_list: the index for 39 participants

* fixdata: contains fixation data of all videos from all participants, each row refers to a single fixation.

* fixdata_fields: 
    '1: SubjectIndex (see subj_names_list)'
    '2: VideoIndex (see video_names_list)'
    '3: Timestamp (milliseconds after image display)'
    '4: GazeDuration'
    '5-6: fixation position (take upper-lift corner as origin )'
   
e.g. If a row in fixdata is '6 29 4084 183 467 319', that means this fixation is in '029.avi' recorded from 'ZMX'. The start time and the duration of this fixation is 4084ms and 183ms, respectively, with the location (467,391).

As a test, you can run **'demo.m'** to view the heatmaps of the target video.  

## Annotaion Results
**'annotated_facial_landmarks'**: The annotation of facial landmarks, for 65 videos. 'final**i**.mat' is the landmark annotation of the i-th video.

**'annotated_speaking_feature'**: The annotation of speaking feature, for 65 videos. 'mouthMotion**i**.mat' is the speaking feature annotation of the i-th video.


## Contact
Should you have any queries, please contact fannie_lyf@buaa.edu.cn / yufan.liu@ia.ac.cn

Have fun!
