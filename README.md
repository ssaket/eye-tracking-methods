# Course: Introduction to eye-tracking methods

## About this repository
In this repository we develop materials for a graduate-level course introducing students to some of the eye-tracking methods used in cognitive psychology, psycholinguistics, and related fields.  Materials are published under the CC BY-NC license.  Feel free to use and adapt this material for your own courses.  Also feel free to use our [issue tracker](https://github.com/tmalsburg/eye-tracking-methods/issues) to make suggestions for improvements.  Contributions in the form of actual content are welcome, as well, and can be submitted via pull requests or e-mail.

See [here](https://github.com/tmalsburg/eye-tracking-methods/graphs/contributors) for a list of contributors.

## Course description
The goal of this course is to put participants in the position to plan and conduct their own eye-tracking experiments.  Our aim will be to understand each step in the acquisition, preprocessing, analysis pipeline up to the statistical analysis.  Time permitting we will also look into some prominent computational models of eye movement behavior.

Specific topics: Eye physiology, visual perception, oculo-motor control and types of eye movements, eye-tracking technologies, design and implementation of eye-tracking experiments, acquisition of eye movement data, quality control, algorithms for the detection of eye movements and gaze fixations, conventional eye-tracking measures, scanpath analysis, computational models of eye movement behavior.

## Course format
The course consists of lectures, discussion, supervised practical exercises, and self-organized project work.  Lectures on each week’s topic will be online and prerecorded (asynchronous).  In addition, we will meet once per week to discuss the material.  This synchronous meeting will be in person (pandemic permitting) or online.  Supervised exercises will take place at a fixed time each week in the eye-tracking lab in Keplerstraße 17 (K2, R10.012).  Project work will be conducted in small groups which will also have access to the lab.

## Eye-trackers
For practical exercises and project work we will use two GazePoint GP3HD and one GP3 eye-tracker.  A research-grade SMI IView X eye-tracker may also be available for those who are interested.  Beyond that we will introduce SR Research’s popular EyeLink 1000 system and PupilLabs’ Core system.  However, those may not be available for exercises and project work.

## Prerequisites
- Basic background in programming in a language such as Python, R, Julia, Matlab, or similar (or willingness to acquire it on your own initiative).
- High school math (or willingness to refresh it on your own initiative).
- Problem solving skills and ability to work independently.

## Organizational details
Discussion session:
- Time: Wed, 9:45-11:15
- Room: Keplerstraße 17 (K2), lecture room M 17.72 (7th floor).

Lab exercises:
- Time: t.b.d.
- Room: Keplerstraße 17 (K2), R10.012 (10th floor).

## Syllabus
### Week 01 (Oct 20): Eye physiology and visual perception
=> Demo with Pupil Labs?

  - Retina
  - peripheral/foveal
  - Optics (lense, light)
  - pupil
  - eye muscles
  
### Week 02 (Oct 27): Topics for group projects
  ? Should we give them explicit ideas like
    - Visual Search
    - Region of Interest
    - Reading task, Music sheets?
  ? Or should we give them a question, or should they come up with one themselves?

### Week 03 (Nov 03): Oculo-motor control and types of eye movements
  - FEF, PPC, superior colliculus
  - Saccades
  - Fixations
    - Smooth Pursuit
    - VOR, OK
  - vergence
  - rotation
 
### Week 04 (Nov 10): Eye-tracking technologies / types of eye-trackers
  - Trackable features 
    - Pupil
      - Dark/Light Pupil
    -  Cornea-Reflection
    -  Iris => rotation 
    -  Photoreceptors
    -  Eye-Ball
  - Historical measures
    -  looking at eyes
    -  mirrors on eyes
    -  coils
    -  EOG

  - Videobased ET
    - remote
    - headmounted
      - mobile ET
        - parallax problem
    
  - Dual-Purkinje, 
  - laser scanning
  - bubble/mouse-click technique


### Week 05 (Nov 17): Design and implementation of a simple eye-tracking experiment with OpenSesame
  ? Doesnt this require basic knowledge given earliest in Week 10 / 11 the eye-tracking measures?
  ? I.e. fixation duration, AOI etc. Or should we preview them here as well?

### Week 06 (Nov 24): Design and implementation of a simple gaze-contingent experiment with OpenSesame
### Week 07 (Dec 01): Acquisition of eye-tracking data and quality control 1
  - ? Calibration methods

### Week 08 (Dec 08): Detection of eye movements in raw eye-tracking data: Box- and velocity-based algorithms
  -> Maybe broaden this up to blackbox algorithms as well? Cluster, HMMs, Deepnets
  - Automated correction of fixation locations:
    - Carr, J. W., Pescuma, V. N., Furlan, M., Ktori, M., & Crepaldi, D. (2021). Algorithms for the automated correction of vertical drift in eye-tracking data. Behavior Research Methods. http://dx.doi.org/10.3758/s13428-021-01554-0

### Week 09 (Dec 15): Conventional eye-tracking measures and analysis approaches in scene perception research

### Week 10 (Dec 22): Conventional eye-tracking measures and analysis approaches in reading research
  !! No slot in this week, BaWü has long christmas break

### Week 11 (Jan 12): Scanpath analysis
### Week 12 (Jan 19): A computational model of eye movements in scene viewing
  - SceneWalk
  - Deepgaze

### Week 13 (Jan 26): A computational model of eye movements in reading
### Week 14 (Feb 02): Presentation of group projects
### Week 15 (Feb 09): Presentation of group projects

