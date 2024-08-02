# Comparing-Autoeroticisms
This is a repository for my never-completed study on Autogynephilia and Erotic Self-Focus in Women

# Data Description:

The data is split into two datasets, each corresponding to either the control group (Control_group_responses.csv), or the effect group (Adjustment_group_responses.csv). The effect in question is an adjustment to the wording of the items of the Anatomic subscale of the Generalized Autogynephilia Scale [citation]. Each subject was randonly assigned to either the control group or the effect group using a Google Apps Script which, upon clicking the link, would automatically use a random number generator to randomly render either the Google Form with the unadjusted items, or the Google Form with the adjusted items. 

The data is from an online convenience sample. The link to the Google Apps Script was shared on several sites such as Twitter, and Subreddits of various topics, tags on tumblr etc. A list of each exact platform/community where the link was posted, along with available details on the number of likes/impressions on the post will be made available in the [appendix, at the bottom]. We did not ask respondents to specify where they found the survey, so we can't be sure where responses come from.

All subjects were required to indicate that they were 18 years or older, and that they consented to what was outlined in the Informed Consent Block. [see in appendix, at the bottom]

# Measures:

Variable: (csv_column_label) (response type)

**Sex/Gender:** (sex_gender) (Multiple Choice)
Subjects were asked to select their sex/gender from a list of options, each specifying a gender identity and an indicator of assigned sex at birth. Additionally, subjects were allowed to select "other" and write in their own identity.

**Kinsey Scale:** (kinsey_scale) (7-Point Likert)
Subjects were asked to rate their sexual orientation from exclusively gynesexual to exclusively androsexual. Subjects were asked to leave this blank if they identify as asexual

**HRT:** (HRT) (binary response)
Subjects were asked whether or not they take cross-sex hormones for the purpose of gender/sex transition

**dimorphism:** (dimorphism) (7-point Likert)
Subjects were asked to rate their own subjective perception of their body as physically masculine or feminine

**sexual behavior:** (sexual_behavior) (Checklist)
Subjects were asked to specify what sex/gender (same list as Sex/Gender question) groups they have had sexual encounters with

**Erotic Self-Focus Questionnaire, Factor 1 - Arousal to Own Body/self:** (ESFQ_X; X = item number) (7-point Likert)
Subjets were administered a 21 question subscale of the Erotic Self-Focus Questionnaire reflecting the first factor of the full scale found by EFA (Evan Fertel, 2015).

**Generalized Autogynephilia Scale, Factor 1 - Anatomic Autogynephilia:** (AGP_X; X = item number) (5-point Likert)
Subjects were administered a 7 question subscale of the Generalized Autogynephilia scale, reflecting the first factor of the full scale found by EFA (Hsu Et al., 2015)

**Free Response:** (testimony) (qualitative, text)
Subjects were asked to describe how embodiment does or does not play a role in their sexuality

# Legend:

**Kinsey Scale:** 0 = gynesexual; 6 = androsexual; 3 = bisexual; missing data = Asexual

**dimorphism (self-rating of physical masculinity vs femininity):** 1 = highly masculine; 7 = highly feminine

# My Planned Confirmatory Analysis

**Key Variables:**

- Factor Scores on the ESFQ arousal to own body/self subscale (via Evan Fertel, 2021 EFA)
- Factor Scores on the adjusted and unadjusted GAS Anatomic AGP subscale (via Hsu et al., 2015 EFA)
- Sex/Gender

### Hypothesis 1:

We hypothesized that the items assessing anatomic autogynephilia lack divergent validity w/ measures of ESF to a notable extent, even if they are not exatly identical. 

**r** = Pearson Correlation Coefficient between GAS AGP subscale (factor scored), and ESFQ arousal to own body/self subscale (factor scored)

- **H_0: r** <= 0.50
- **H_a: r** > 0.50

Pre-Registration suggests we will take any **r** > 0.5 as confirmation. This is not to say **r** > 0.5 is evidence they measure the same construct entirely, just that there may be signal contamination, given that ESF validated as a characteristic construct in heterosexual cis women, should theoretically be entirely uassociated with AGP.  

#### Theoretical backing
It is clear to see from the content of the items in each scale, that there is conceptual overlap that could lead to shared variance. See for example "ESFQ_7 - To what extent do the following activities help get you in the mood for sex? Looking at myself in the mirror in my undergarments" compared to "AGP_2 - Picturing myself having a nude female body or certain features of the nude female form." or consider "ESFQ_14 - I get turned on by my own sense of masculinity/femininity." compared to "AGP_1 - The thought of being a woman.". It seems very likely that there would be a notable degree of *manifest* overlap between people who score high on AGP and people who score high on ESFQ. This may be indicative of poor construct validity on one side or the other if we consider the fact that the AGP scale is intended to measure a specific latent construct 'Autogynephilia' which is specified as an Erotic Target Location Inversion of a gynephilic sexual orientation. On the other hand, the ESFQ was inspired by and found to be characteristic of the sexualities of Heterosexual Cisgender Women. A demographic where no theoretical justification exists for the commonality of autogynephilia, indicating some other autoerotic construct exists that the ESFQ is sensitive to. And there doesn't seem to be any reason this construct should correlate with AGP. 

### Hypothesis 2:

We hypothesized, based on past data from Veale et al., that the adjustment to the Anatomic AGP subscale would increase cis women's scores on the scale.

**X_1** = Mean of Cis Women in Effect group; 
**X_2** = Mean of Cis Women in Control Group

**d** = **X_1** - **X_2**; Mean difference between Control Cis Women, and Effect Cis Women.

- **H_0: d** <= 0
- **H_a: d** > 0

t-test for independent samples, unequal variances

### Hypothesis 3:

We hypothesized that the effect of the adjustments on subjects responses would be greater for cis women than for trans women, and thus bring their score closer together relative to controls

**d_1** = Mean Difference between trans vs cis women in control group;
**d_2** = Mean Difference between trans vs cis women in Effect group 

- **H_0: d_2** >= **d_1**
- **H_a: d_2** < **d_1**

t-test for independent samples, unequal variances

#### Theoretical Backing
Veale et al. have previously made minor adjustments to the Core AGP Scale when administering the test to a sample inclusing cis women, out of concern that the wording of the original questions may seem strange to cis women, inducing measurement non-invariance. It is unclear whether there is any measurement non-invariance between groups on the original questions, however at face value it seems likley. These are questions about how it feels to imagine yourself in a specific embodiment. It seems like the more you are simply used to always being in that mode of embodiment by default, the stranger the question is. It's just your default. It's just you and always has been. Additionally, existing research suggests that it is very common for scales to fail tests of measurment invariance between gender and age groups. Theoretically, using research on Object of Desire Self-Consciousness (ODSC) we could imagine that seeing oneself specifically as "attractive or more attractive" plays a key role in autoerotic appeal in women. If this is the case then we might also think compare to a cis female group, a trans female group will be disproportionately male-bodied. For a male-bodies person who identifies as a woman, and has this aforementioned mode of autoeroticism, it may be the case that merely imagining oneself as a woman, also inherently makes them feel "more attractive" necessarily, while for the cis female group it may not have this automatic enhancement effect. As such it may be reasonable to hypothesize that, if this mode of autoeroticism is behind the scores of both cis and trans women, then there should be some mean-structure non-invariance between groups, that is reduced by an adjustment to the question that specifies imagining oneself as "attractive or more attractive" or in the case of my own adjustment "Particularly attractive and feminine" 

# Appendix

## Informed Consent Block
Thank you for taking an interest in our survey. First, we'd like you to read an informed consent form. 

This study is designed to add to the body of research on the sexualities of underrepresented gender and sexual identity groups. Particularly on the relation between multiple constructs related to self-focus during erotic fantasies/experiences, and sex/gender. You will be asked to answer questions about your feelings regarding the relation between your erotic experiences, and your relationship to your body, or your conceptualization of it.

No personal identifying information will be collected from you at any point in this survey. This includes your email, which may be associated with the google account you are accessing this survey on. Your data is entirely anonymous, and there is no way for us to find out who you are.

I have been informed that my participation in this research is voluntary. I have been informed that data collected for this study will be retained by the investigators and may be shared in a de-identified form with peer-review journals, Institutional Review Boards (IRBs), and even the general public for the purpose of open-science.

There are no known risks involved in completing the survey, and there are no tangible benefits. However, in completing the survey you may play a part in combating potentially harmful false narratives in the field of sexology, that disproportionately impact queer women. 

Options: "I Agree" ; "I Disagree"

## Sampling Sources

### Tumblr
Two sampling sessions were conducted through tumblr.

The Fist Session (12/11/23) made use of the paid "Blaze" feature. This resulted in 2500 impressions targeting US English speakers
Additionally, the following Hashtags were attatched:

#feminism
#transgender
#trans
#lgbtq
#psychology
#transsexual
#lgbtqia
#lesbian
#sapphic
#bisexual
#social justice
#transfem
#nonbinary
#lgbt
#queer
#gender
#smut
#fanfic
#fanfiction
#uquiz
#personality quiz
#fandom
#fan fic
#fan fiction

The Second Session (12/17) did not use the paid "Blaze" feature, and impressions were not recorded, nor likes. For this round, the following trending tags were attatched to maximize exposure:

#transmedicalism
#goodtimeswithscar
#pokemon
#hlvrai
#christmas
#one piece
#coraline
#mythology
#good omens

### Reddit

For a single session (12/18) the survey was posted to several subreddits. Some of these posts were immediately deleted:

r/AO3 - (deleted)
r/FanFiction - (deleted)
r/psychologyOfSex (12/18/2023)
r/Transmedical - (deleted)
r/Truscum - (deleted)
r/bisexual (12/18/2023)
r/destiny (12/18)

### Discord

At an unrecorded later date, the survey was posted in text channels from the following public discord servers:

Vaush's Praxis Emporium (A community for an american far left wing political streamer, known for trans positivity)

r/fanfiction (A community for users of the r/fanfiction subreddit, as well as other people interested in a community for fanfiction writers)

destiny.gg (A communuty for an american center left wing political streamer)

The Super Ego (A community for a psychology and center-left politics streamer)

DIRL (A community for a drama & lifestyle kick streamer)

Honey Bees (A Community for a fans of a lesbian ship between two characters in the animated roosterteeth show RWBY)

### Archive of our Own (AO3)

At an unrecorded later date, the survey was posted as a work under several highly popular fandom (Intellectual Property) categories on Archive of Our Own (a website for fanfiction)

Stranger Things (TV 2016)

Harry Potter - J. K. Rowling

原神 | Genshin Impact (Video Game)

文豪ストレイドッグス | Bungou Stray Dogs

Call of Duty (Video Games)

Our Flag Means Death (TV)

僕のヒーローアカデミア | Boku no Hero Academia | My Hero Academia (Anime & Manga)

Minecraft (Video Game)

Wednesday (TV 2022)

Stray Kids (Band)

The Sandman (TV 2022)

House of the Dragon (TV)

The Owl House (Cartoon)

Good Omens (TV)

Trigun Stampede (Anime 2023)

Original Work

The work remained listed for a few months, But unfortunately I was required to take it down, and I forgot to record how many hits it got before I took it down. oops. It seemed like a lot tho. There were certainly serveral comments

## Scales & Items

### Erotic Self-Focus Questionnaire, Arousal to own Body Subscale (ESFQ)

all of the following questions are from the Arousal to own Body subscale of the ESFQ from "It's not you, it's me: Measuring Erotic Self-Focus" by Evan Fertel, 2021

the scale was headed off with "For the following questions, respond with whether the statement is "Not at all" true or "Very much" true for yourself." 
all questions had a 7-point Likert response format ranging from "Not At All" to "Very Much"

ESFQ_1 - I find it exciting to walk around the house naked

ESFQ_2 - I find it exciting to walk around the house alone naked. 

ESFQ_3 - I feel sexy when I am naked. 

ESFQ_4 - To what extent do the following activities help get you in the mood for sex? Looking at myself in the mirror naked  

ESFQ_5 - I have been excited by the experience of catching a glimpse of my reflection in a mirror while naked or in a state of undress.

ESFQ_6 - I feel sexy when I wear a bathing suit.

ESFQ_7 - To what extent do the following activities help get you in the mood for sex? Looking at myself in the mirror in my undergarments  

ESFQ_8 - I experience a sexual energy when I walk a certain way (e.g., swinging my hips, strutting with confidence or swagger).   

ESFQ_9 - It is arousing to wear sexy underwear underneath my clothes, especially when I am the only one who knows I am wearing them.   

ESFQ_10 - I enjoy the feeling of being naked.  

ESFQ_11 - It is sexually exciting to go out without wearing underwear.  

ESFQ_12 - I have been excited by the experience of catching a glimpse of my reflection in a mirror or window in public.   

ESFQ_13 - I have found that feeling a strong sense of connectedness with my own body can be an erotic experience.  

ESFQ_14 - I get turned on by my own sense of masculinity/femininity.  

ESFQ_15 - I am aroused by the appearance of my own genitals in an aroused state (i.e., hard, engorged, wet).  

ESFQ_16 - During sex, how much of a turn on is it for me to think of, or imagine, how I look as I am having sex?   

ESFQ_17 - I have been aroused by the physical sensations of exercising/working out.

ESFQ_18 - During sex, how much of a turn on is it for me to think about how hard or wet I am?  

ESFQ_19 - The experience of dancing alone (i.e., without a partner) can feel erotic or arousing. 

ESFQ_20 - Would I want to have sex with me?  

ESFQ_21 - Outside of sexual activity, I enjoy my own physical touch (for example, sliding or rubbing my fingers against my own skin or massaging my own body).   

### Generalized Autogynephilia Scale, Anatomic Autogynephilia Subscale (AGP)

the following questions are from "the psychometric structure of items assesing autogynephilia" by Hsu et al (2015)

The scale was headed off with "How sexually arousing would you find each of the following activities?" 
all questions had a 5-point Likert response formate ranging from "Not at all arousing" to "Very Arousing"

AGP_1 - The thought of being a woman.  

AGP_2 - Picturing myself having a nude female body or certain features of the nude female form.

AGP_3 - Picturing myself with a woman’s breasts.

AGP_4 - Picturing myself with a woman’s buttocks.

AGP_5 - Picturing myself with a woman’s legs.

AGP_6 - Picturing myself with a vagina/vulva.

AGP_7 - Picturing myself with a woman’s face.

### The Adjusted Anatomic Autogynephelia Scale (AAGP)

The following questions are my own adjustment of the items from the Anatomic subscale of the Generalized Autogynephilia Scale by Hsu et al. (2015)
The adjustments are heavily inspired by the adjustment Veale et al (2014) made to the Core Autogynephilia Scale. The rationale behind the adjustment was to attempt to mitigate a theorized source of *hypothetically* expected measurement non-invariance

The scale was headed off with "How sexually arousing would you find each of the following activities?" 
all questions had a 5-point Likert response formate ranging from "Not at all arousing" to "Very Arousing"

AAGP_1 - The thought of being a particularly attractive and feminine woman.

AAGP_2 - Picturing myself having a particularly attractive and feminine nude female body or certain features of the nude female form.

AAGP_3 - Picturing myself with particularly attractive and feminine breasts.  

AAGP_4 - Picturing myself with a particularly attractive and feminine buttocks.

AAGP_5 - Picturing myself with particularly attractive and feminine legs.

AAGP_6 - Picturing myself with a particularly attractive and feminine vagina/vulva.

AAGP_7 - Picturing myself with a particularly attractive and feminine face.

### Free Response (testimony)

In addition to being required to complete the scales, subjects were optionally asked to write out a free response to the following question:

"Briefly describe how/why or to what extent your awareness/perception of your own body is relevant to your sexual fantasies, or the way you feel about actual sexual encounters."
