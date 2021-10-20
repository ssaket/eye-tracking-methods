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
### Week 00 (Oct 20): No class
The university requested that we leave the first three days of the lecture period free for [introductory events](https://www.student.uni-stuttgart.de/en/startingout/introduction/study-program/).

### Week 01 (Oct 27): Eye physiology and visual perception
Presenter: Bene
=> Demo with Pupil Labs?

  - Retina
  - peripheral/foveal
  - Optics (lense, light)
  - pupil
  - eye muscles

**Homework:**
  - Work through some Python tutorial.  Needs to cover basic math needed for the course.
  - Some basic programming exercises.
    1. Read some from a `.csv` file.
    2. Make a simple plot of the data and save it in a file.
    3. Calculate some basic summary statistics (mean, standard deviation, median, median absolute deviation, …).
    4. Write data to a `.csv` file.
  - Read relevant chapter in Holmqvist et al.
  
### Week 02 (Nov 03): Topics for group projects
Presenter: Bene, Titus
  - Should we give them explicit ideas like
    - Visual Search
    - Region of Interest
    - Reading task, Music sheets?
  - Or should we give them a question, or should they come up with one themselves?

**Homework:**
  - Read some chapter in Holmqvist et al.
  - Choose a project or propose your own.
  - Form groups of 2 to 4 people for the project work.

### Week 03 (Nov 10): Oculo-motor control and types of eye movements
Presenter: Bene
  - FEF, PPC, superior colliculus
  - Saccades
  - Fixations
    - Smooth Pursuit
    - VOR, OK
  - vergence
  - rotation

**Homework:**
  - Read relevant chapter in Holmqvist et al.
 
### Week 04 (Nov 17): Eye-tracking technologies / types of eye-trackers
Presenter: Bene
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

**Homework:**
  - Read relevant chapter in Holmqvist et al.

### Week 05 (Nov 24): Designing experiments with OpenSesame 1
Presenter: Edwin Dalmaijer
  - Basics of OpenSesame without eye-tracking.  E.g. Posner cuing task.
  - Add eye-tracking (and mouse simulation) to the Posner task.
  - Anatomy of a simple scene-perception experiment, e.g. Yarbus-style.

**Homework:**
  - Install OpenSesame.
  - Work through introductory tutorial.
  - Implement a simple scene perception experiment similar to what was
    shown in the lecture but spelled out into a full experiment that
    you could actually run.  Could be modeled after some classic
    study, e.g. Yarbus (1967).  Test it with mouse-tracking.

### Week 06 (Dec 01): Designing experiments with OpenSesame 2
Presenter: Edwin Dalmaijer
  - Anatomy of a simple reading experiment.
  - Gaze-contingency: make the experiment respond to eye movements.

**Homework:**
  - Work through Visual World tutorial for OpenSesame.
  - Implement a simple reading experiment similar to what was
    shown in the lecture but spelled out into a full experiment that
    you could actually run.  Could be modeled after some classic
    study.  Test it with mouse-tracking.

### Week 07 (Dec 08): Acquisition of eye-tracking data and quality control 1
Presenter: Titus
  - Calibration methods
  - Drift correction
  - Glasses, contact lenses
  - Lighting
  - Chins rests
  - Remote tracking
  - Tower mount vs. desktop mount systems
  - Measures of accuracy / precision
  - Racial differences, model- vs. centroid pupil-tracking
  - Typical failure modes (example data).
  - Instructions (when you tell people not to blink, they sometimes blink more)

**Homework:**
  - Read relevant chapter in Holmqvist et al.
  - For a given data set:
    - perform drift correction
    - calculate accuracy
    - calculate precision
    - check how stable the sampling rate was, quantify variability somehow
    - label each sample with the AOI that it’s in (if any)

### Week 08 (Dec 15): Detection of eye movements events and post-processing
Presenter: Titus
  - Maybe broaden this up to blackbox algorithms as well? Cluster, HMMs, Deepnets
  - Criteria for removing data.
  - Manual corrections (common in some fields but questionable).
  - Automated correction of fixation locations:
    - Cohen, A. L. (2012). Software for the automatic correction of recorded eye fixation locations in reading experiments. Behavior Research Methods, 45(3), 679–683. http://dx.doi.org/10.3758/s13428-012-0280-3
    - Carr, J. W., Pescuma, V. N., Furlan, M., Ktori, M., & Crepaldi, D. (2021). Algorithms for the automated correction of vertical drift in eye-tracking data. Behavior Research Methods. http://dx.doi.org/10.3758/s13428-021-01554-0

**Homework:**
  - Read relevant chapter in Holmqvist et al.
  - Implement one of the following two and evaluate its performance using the provided reference data set:
    - a basic velocity-based saccade detection
    - a basic box-model fixation detection

### Week 09 (Dec 22): Conventional eye-tracking measures and analysis approaches in scene perception research
Presenter: Bene

**Homework:**
  - Read relevant chapter in Holmqvist et al.

### Week 10 (Jan 12): Conventional eye-tracking measures and analysis approaches in reading research and the visual world paradigm
Presenter: Titus
Reading:
  - Canonical ET measures and their interpretation.
  - Statistical issues
  - Predicting comprehension from canonical ET measures (Mézière et al.).
Visual world paradigm:
  - Looks to target over time plots
  - Binned analysis
  - Gamms
  - Survival analysis
  - Permutation tests
  - Stone and Lago paper.

**Homework:**
  - Read relevant chapter in Holmqvist et al.
  - Read:
    - Kliegl, R., & Laubrock, J. (2018). Eye-movement tracking during reading. In (Eds.), Research methods in psycholinguistics and the neurobiology of language: {A} practical guide (pp. 68–88). : Wiley Blackwell.
    - Clifton, C., Staub, A., & Rayner, K. (2007). Eye movements in reading words and sentences. In R. P. G. van Gompel (Eds.), Eye Movements: A Window on Mind and Brain (pp. 341–374). Amsterdam, Netherlands: Elsevier Science Ltd.
    - Vasishth, S., von der Malsburg, T., & Engelmann, F. (2013). What eye movements can tell us about sentence comprehension. Wiley Interdisciplinary Reviews: Cognitive Science, 4(2), 125–134. http://dx.doi.org/10.1002/wcs.1209
  - Provided a reference data set (fixations, perhaps Potsdam Sentence Corpus) write code that calculates:
    - First fixation durations
    - Gaze durations
    - First pass skipping probability
    - First pass regression probability
    - Total reading time
  - In the Potsdam Sentence Corpus, calculate proportion of:
    - progressive saccades to the next word,
    - progressive saccades that skip the next word,
    - regressions,
    - refixations.

### Week 11 (Jan 19): Scanpaths
Presenter: Titus
  - Scanpath theory
  - Yarbus
  - Frazier & Rayner (1982)
  - Overview of approaches 
    - Anderson, N. C., Anderson, F., Kingstone, A., & Bischof, W. F. (2014). A comparison of scanpath comparison methods. Behavior Research Methods, 1–16. http://dx.doi.org/10.3758/s13428-014-0550-3
    - HMMs
  - Malsburg & Vasishth (2011)

**Homework:**
  - Read relevant chapter in Holmqvist et al. (if any).
  - Given a python function for calculating the dissimilarity of two scanpaths, perform some simple scanpath analysis.

### Week 12 (Jan 26): Computational models of eye movements in scene viewing and reading
Presenter: Bene, Titus
  - SceneWalk
  - Deepgaze
  - Some reading model

**Homework:**
  - Read relevant chapter in Holmqvist et al.
  - Read (some or all of):
    - Engbert, R., Nuthmann, A., Richter, E. M., & Kliegl,
      R. (2005). SWIFT: A dynamical model of saccade generation during
      reading. Psychological Review, 112(4),
      777–813. http://dx.doi.org/10.1037/0033-295X.112.4.777
    - Engelmann, F., Vasishth, S., Engbert, R., & Kliegl, R. (2013). A
      framework for modeling the interaction of syntactic processing and
      eye movement control. Topics in Cognitive Science, 5(3),
      452–474. http://dx.doi.org/10.1111/tops.12026
    - Salvucci, D. D. (2001). An integrated model of eye movements and
      visual encoding. Cognitive Systems Research, 1(4),
      201–220. http://dx.doi.org/10.1016/s1389-0417(00)00015-2
    - Reichle, E. D., Rayner, K., & Pollatsek, A. (2003). The e-z reader
      model of eye-movement control in reading: Comparisons to other
      models. Behavioral Brain Science, 26(4), 445–476.

### Week 13 (Feb 02): Presentation of group projects
Presenter: Students

**Homework:** None.

### Week 14 (Feb 09): Presentation of group projects
Presenter: Students

**Homework:** None.

