---
title: "EGG Lab Manual"
date: "Nov 2018"
author: "Nick Van Handel"

---

## Setting up a recording session

#### Based primarily on the Glottal Enterprises manual + Marc Garellek's AMP Tutorial


1. Turn the EGG on, and check that the batteries are charged
  * You can check each of the batteries by flipping the power switch to the left and the right
  * Both lights are green: 2-hour charge
  * Either light is red: 6-hour charge
  * The EGG MUST be turned off while charging
    * This prevents interference with the EGG signal

2. Connect the EGG to your laptop
  * Check that your computer recognizes the EGG
    * Mac: System Preferences -> Sound -> Input
    * Windows: **update this**
  
3. Connect the microphone
  * XLR port on the back panel
  * However, Marc Garellek recommends recording the audio separately (AMP 2018)
    * We should see we like audio recorded through the machine,
    since this does not require the additional step of syncing, which adds the possibility of
    extra complications (especially for experiments, but maybe not as bad for fieldwork?)

4. Position the electrodes
  * Plug the electrodes into the electrodes jack on the front panel
  * Cover the electrodes with a tiny layer of electrode gel (optional, but helps if the signal is weak)
    * The gel should not touch the insulating strip between the electrodes
  * Attach the electrodes to the velcro strap
    * The insulating strip should be horizontal (parallel with the strap)
    * The electrode with red wires should be on the left
  * Place the electrodes just below the Adam's apple; the electrodes should be facing one another to the extent possible
  * Have the subject hold /a/, and adjust the height of the electrodes until the "Electrode Placement/Laryngeal Movement" indicator
  on the front panel is centered on the green LEDs and relatively stable
    * **This is extremely important - the signal is noisy if the electrodes are too low or too high**
  * Secure the collar; it should be tight enough that the electrodes are always in contact with the skin
 
5. Open the recording software (Praat, Audacity)
  * Make sure to select the EGG as the input in the recording software (Praat, Audacity)
  * Stereo recording
  
6. Experiment with the output levels (optional)
  * Switches on front panel
  * Marc Garellek recommends EGG Output on Low, Audio Output on High
    * **Another thing we should play around with**

You are now ready to record!

## Wrapping up a recording session
1. Turn the EGG off

2. Clean off the electrodes with water

3. Wipe off the electrodes with disinfectant between subjects
  * **Do we have something for this?** 

## Analysis

### What measures are available?

#### Closed Quotient (CQ) and Open Quotient (OQ)

Two of the most common measures used in EGG research are the closed quotient (CQ) and open quotient (OQ).
These measures describe the proportion of a glottal period during which the vocal folds are closed
and open, respectively. It follows that CQ + OQ = 1.

Conceptually, the CQ and OQ are straightforward; however, there has been a lot of debate over how
to calculate these two measures [@henrich2004; @herbst2010; @herbst2014; @herbst2017]. The EGG + Threshold
method demarcates the closed and open portion of the period by determining when the EGG waveform
crosses a set percentage of the maximum amplitude [@henrich2004; @herbst2017]. The threshold method is problematic
as the analyst must make a choice of what threshold to use to determine that closure has taken place,
and this decision is somewhat arbitrary.

An alternative is to identify the closing and opening moments from the positive and negative peaks
in the derivative of the EGG signal (DEGG). This method is advantageous because there is usually one
clear positive and negative peak for each period in the DEGG signal, so the researcher does not need
to make a decision about the threshold to use. Moreover, DEGG-based measurements of OQ and CQ are more
closely correlated with measurements of glottal airflow [@henrich2004] and CQ based on videokymographic
endoscopy [@herbst2017]. However, use of peaks in the DEGG signal may be misleading, as
contacting and de-contacting should not be thought of as single moments in time [@herbst2014].

A downside to the DEGG signal is that there may be multiple opening peaks [@herbst2010]. In this case,
a hybrid method should be used: closure is determined from the positive peak in the DEGG signal, while
opening is based on a threshold. The typical threshold for the hybrid method is 3/7 [@kuang2012; @herbst2017].

CQ is extremely useful in the investigation of phonation types, since it provides an index of the degree
of glottal constriction. Tense / creaky / laryngealized registers tend to have higher CQs, while breathy
phonation has a relatively smaller CQ. Modal voice is less consistent, and may involve either high or low
OQ [@dicanio2009]. OQ is better correlated with H1-H2, a measure of glottal tension, than with H1-A3, a
measure of breathiness; as such, @dicanio2009 suggests that EGG is potentially limited for languages
with multiple phonation types, whose differences could go beyond what EGG shows. However, @keating2011
found that CQ reliably distinguishes phonation in several languages.

CQ may also be useful for investigating strengthening and hyperarticulation. @li2014 found that the CQ
of vowels following a segment in domain-initial position was negatively correlated with boundary strength;
however, the data are somewhat equivocal and this was not consistent across all of the segments tested,
so more research is needed before I would recommend using CQ for this purpose.

**figure out how to include images in markdown; would be useful here to compare EGG and DEGG**

#### Speed Quotient (SQ)

Speed Quotient (SQ) is the ratio of closure duration and opening duration [@kuang2012 and references therein].
This measure is a way of describing the symmetry of the glottal pulse, which may relate to phonation: creaky
voice should have a lower SQ, indicating a skewed pulse due to shorter closure duration, while breathy voice should
have an SQ closer to 1, reflecting similar closure and open durations. However, SQ is reported to not
vary with phonation as reliably as CQ [@kuang2012], and impressionistically, this measure is not used
nearly as much as the others discussed here.


#### Derivative-EGG Closure Peak Amplitude (DECPA) / Peak Increase in Contact (PIC)

DECPA / PIC is a measure of the amplitude at the positive (contacting) DEGG peak and is thought
to reflect the speed of the transition to the closure phase [@michaud2004; keating2011]. @keating2011
found that PIC can differentiate phonation contrasts in at least some languages and that it tends
to be higher for breathy phonation. Beyond phonation, @michaud2004 also found that DECPA correlates
with pragmatic emphasis, even in cases where F0 and intensity did not reliably indicate focus.

There are some potential limitation to the use of DECPA / PIC. Since DECPA is simply the amplitude
of the peak, the absolute value is meaningless and depends on the input level for the recording session.
This places limitations on comparisons across speakers and recording sessions. Although I don't believe
this has been discussed with respect to DECPA, the position of the larynx relative to the electrodes may
also shift during a recording session, which may affect the strength of the signal and raises further
questions about the reliability of DECPA.

#### Vertical Larynx Position

Vertical Larynx Position (VLP) is a measure of the relative height of the larynx estimated by comparing
the relative voltage from the upper and lower electrodes [@rothenberg1992]. VLP can be calibrated by
sliding the electrodes up and down the participant's neck and measuring the voltage output at
different heights [@elliot1997; @pabst1993; @rothenberg1992]. Alternatively, VLP can be taken
from the direct output voltage without conversion into a physical measure [@iwarsson1998].
In this case, comparisons should be made within subjects.

VLP can be useful for describing consonants; for instance, @elliot1997 found that a prolonged /b/
induces lowering more than other consonants. VLP could also be applied to hyper-articulation; we may
expect a greater level of larynx lowering in order to maintain voicing for a longer period of time. VLP
may also be useful in the description of sounds with a glottalic airstream mechanism. However, I have not
seen these applications of VLP discussed in the literature, and they may depend on how reliable and sensitive
the measure is.

VLP has several limitations. Since the measure relies on the relative contact of each electrode,
VLP can be influenced by factors other than laryngeal height, including tilt of the head and protrusion
of the chin [@iwarsson2001]. Despite these potential confounds, @laukkenan1999 found that VLP shows agreement
with videofluorographic measures of larynx height.

A more practical issue involves recording the output of the vertical larynx positioning meter
in tandem with the audio and EGG signals. We do not currently have a set up supporting
3-channel recording, and cannot use the measure at this time. Older Rothenberg EGGs had
a high-pass filter which could filter out frequencies below 0, 20, 30, or 40 Hz. Our machine
has a built-in high-pass filter that we cannot change. However, the low-frequency component of the signal
may correspond to larynx raising. Marc has offered to let us use UCSD's older EGG, which lets you
set the high pass filter, if we ever wanted to explore this option.


### Which measures should you use?

#### Interval-oriented analyses

If you are interested in interval-oriented analyses (e.g. phonation) then CQ and OQ are the most
widely used measures. Taking these measures from either the DEGG peaks or the hybrid method is more
common than using the threshold method on the EGG signal.

SQ may also be helpful, particularly if you are interested in quantifying the asymmetry of the glottal
pulse, but it is less consistent in distinguishing phonation types and so its use for linguistic analysis
is less clear.

DECPA / PIC is another measure to consider, but caution must be exercised given that there are no meaningful units.

#### Landmark-oriented analyses

The EGG signal can also be used to look at the opening and closing peaks in the DEGG in tandem with
audio to consider the relative timing of laryngeal gestures and consonant closure, although the literature
reviewed thus far has relatively little to say about this.

@dicanio2012 has looked at the relative timing of voicing and oral closure, which is particularly useful in fieldwork situations
when audio recordings may be noisy. For intervocalic stops, DiCanio tallied how often
devoicing preceded, followed, or was contemporaneous with closure. This can be accomplished by looking
for the moment where periodicity begins and ends in the EGG signal; presumably, the end of periodicity
corresponds to glottal spreading. A similar method could be useful for comparing different stop
productions and for investigating hyper-articulation.

According to Marc Garellek, identifying moments of glottal closure to assess oral-laryngeal timing
(e.g. with glottalized consonants in Mayan) may be more difficult, since the transition from modal voicing
to glottal constriction is continuous, and it is hard to pin down a moment corresponding to the initiation
of glottal constriction. Ryan has the idea of using thresholding - setting a convention for identifying the "onset"
of glottal constriction by taking a certain percentage (e.g. 20) of the participant's CQ range from the
constriction period. Marc is skeptical due to individual differences in baseline CQ value and
because differences in modal and creaky voice are small to begin with. Marc also suggested plotting
CQ values over time for each word (like an f0 plot) to see if there are any turning points that
could correspond to changes in constrictions, but he does not think we would see peaks / troughs so clearly.

For stimulus design, it is recommended to have targets in intervocalic position (e.g. [VXV], X = target
consonant).


## Data Processing

#### praatdet

[Praatdet](https://github.com/kirbyj/praatdet) is a set of Praat scripts created by James Kirby
at The University of Edinburgh. The scripts can process both stereo audio/EGG and mono EGG files. The scripts offer the choice of
calculating the Open Quotient either by relying solely on the dEGG signal or by using the
hybrid method which identifies the contact moment from local maxima in the dEGG signal and finds
the opening moment by applying the threshold method to the EGG signal. At this time, using the pure
threshold method for both contact and opening moments is not possible, but this is not a huge downside
since the dEGG method is preferred [@herbst2017]. The script also allows the user to visually inspect
the detected peaks, which makes it easy to see how the script has treated multiple opening peaks or
whether the script has spuriously identified peaks; this functionality is not available in alternatives
like EggWorks. One last benefit is that the output is R-friendly. At this time, I recommend we use
praatdet as the basis of our data processing / analysis pipeline.

**More information about how to use these scripts, and any adjustments we make to them,
will be added once we start our pilot**

#### NCSU Scripts

NCSU has an [informative page](https://phon.wordpress.ncsu.edu/lab-manual/electroglottograph/) on the basics of electroglottography
that includes Praat scripts for calculating dEGG and combining dEGG and EGG into a single recording.

While the information is useful, I have had some issues using the scripts to process creaky vowels.
A preliminary investigation suggested that there is an issue with the way in which the scripts
accomplish scaling. Should there turn out to be a problem with the praatdet scripts, it may be worth
trying to sort out this issue, but for now I recommend against using the NCSU scripts.

#### EggWorks

[EggWorks](http://www.appsobabble.com/functions/EGGWorks.aspx) is a free online program developed by UCLA.
The website is easy to use and offers a range of different measures (Speed Quotient, Closed Quotient), as
well as different ways of deriving them (e.g. thresholding, hybrid). The output is also easy to read
and R-friendly. That being said, there are some downsides. the program doesn't let you under the hood -
what you see is what you get, and there aren't any options for adapting their program to your needs. It
is also unclear how often the software is updated. For this reason, I would avoid EggWorks in favor of
using Praat scripts that we can adjust as needed.


Ignore amplitude (normalize)


## To-do
  * Certain things highlighted above
  * Analysis
    * Time normalization in R
    * Script to automate analysis of oral-laryngeal timing (a la @dicanio2012).
  * Decide whether we are happy with the audio signal from the EGG
    * Or record separately, and figure out syncing
    * Preferred output gain
  * Update manual with insights from our pilot study

## References