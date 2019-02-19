---
title: 'EA Survey 2018 Series: Group Membership'
date: 2019-02-17T16:45:02.442Z
description: >-
  This post explores which EA groups EA Survey 2018 respondents were members of.
  We find reasonably large numbers of EAs are members of some groups (such as EA
  Facebook and Local Groups), but much smaller numbers are involved across many
  groups.
author: David Moss
originalPublicationURL: >-
  https://forum.effectivealtruism.org/posts/kqTTyz7BCt6ExrfF6/ea-survey-2018-series-group-membership
license:
  name: Creative Commons Attribution-ShareAlike 3.0
  url: 'https://creativecommons.org/licenses/by-sa/3.0/legalcode'
relatedArticles: []
---
## Summary

In this post we explore which EA groups EA Survey 2018 respondents were members of. We find reasonably large numbers of EAs are members of some groups (such as EA Facebook and Local Groups), but much smaller numbers are involved across many groups.

## Total membership of different groups

![Table "Total membership of different groups"](/img/total-membership.png)

**EA Facebook**

The main [EA Facebook](https://www.facebook.com/EffectiveAltruism/) group had the largest membership among our respondents, with slightly more than half being a member. This is unsurprising, given that the EA Facebook group has a very large, broad membership (>16,000, though only around 56.9% of these are active, based on data from the admins).

**EA Forum and LessWrong**

By contrast, [EA Forum](https://forum.effectivealtruism.org/) members were a much smaller group, comprised of just over 500 respondents or 20% of the total sample. This finding makes sense given that the Forum caters to relatively more in depth, niche and advanced content and discussion. As noted in our [previous post](https://forum.effectivealtruism.org/posts/hP6oEXurLrDXyEzcT/ea-survey-2018-series-cause-selections), the EA Forum is estimated to have only around 500 active members. A fairly similar number of EAs in our sample were members of LessWrong.

**Local Groups**

One surprise from this year’s data was the high number of EAs who reported being members of a Local EA group. This was 1018 individuals, the second largest grouping behind the EA Facebook group, and just short of 40% of EAs in our sample. This is a significant increase compared to reported local group membership in previous years of the EA Survey (\~25% in 2015, \~30% in 2017), although comparisons across different iterations of the EA Survey should be treated with extreme caution, given possible differences in sampling (for example, we might have systematically under-sampled local group members in earlier years or have disproportionately heavily sampled them in later years).

That said, it strikes us as plausible that there would be a real increase in the percentage of EAs being members of local groups, given that there has been a large increase in the total number of EA local groups in existence according to both Local Group Survey 2017 data and the central database of local groups (which both find a doubling in numbers of local groups since 2015).

![Graph "% of EAs Who Are Members of a Local Group"](/img/over-time.png)

_N.B. no EA Survey was run in 2016._

![Graph showing the number of EA groups over time](/img/existence.png)

_From Local Group Survey 2017 data._

This change is striking given that i) the EA community as a whole has often been perceived as a largely online community, ii) it has often been suspected that the EA Survey likely oversamples the online community and would undersample those who may be involved in EA offline, but are not active online. Each of these may still be true, and yet even if so, it seems there were still many more (around twice as many) EAs in our sample who reported being a member of a local group than the EA Forum and similar numbers were members of local groups than were members of the EA Facebook group.

**GWWC and TLYCS Pledge**

Around 32.4% of EAs in our sample had taken the Giving What We Can Pledge. We will be discussing the Giving What We Can Pledge further in a future post. Numbers of survey respondents who had taken the The Life You Can Save Pledge, which seems less prominent in the EA community, were predictably much lower.

## Relationships between membership of different groups

Most (>83%) respondents who were members of the EA Forum, were also members of the EA Facebook group. This means we cannot, strictly speaking, think of group membership within our sample in terms of a larger, broader group of EA Facebook members, containing a more narrow, population of EA Forum members, though there is broad overlap. In contrast, just over 61% of Forum members are members of local groups. Among local group members, 31% (320 people in total) are also members of the EA Forum (note that this is substantially higher than among those who are not members of local groups (12.8%)).

![Venn diagram of EA Facebook & EA Forum membership](/img/edited-venn.png)

EA Facebook and EA Local Groups were the two groups with the largest membership within our sample and while there was substantial overlap, many EAs who were members of EA Facebook were not members of a local group and vice versa.

![Venn diagram of EA Facebook & Local Group membership](/img/fb-local.png)

Despite there being similar numbers of EA Forum and LessWrong members in our sample, and despite the two forums sharing some similar areas of interest, membership of LessWrong and the EA Forum was surprisingly non-overlapping. Only about 31% of Forum members were also members of LessWrong and only 30% of LW members were also members of the EA Forum, with only 165 people in our whole sample being members of both. The majority of respondents (1694, 65%) were members of neither.

## Membership clusters

We also performed a cluster analysis to investigate clusters within group membership in our data more inductively, rather than assuming a priori that certain groupings were related or informative combinations.

To determine the best number of clusters we used [the NBcust package](https://CRAN.R-project.org/package=NbClust) in R which provides 30 clustering indices and proposes the best scheme by varying all combinations of number of clusters, distance measures, and clustering methods. We used euclidean distance for the dissimilarity matrix, and completed the final clustering by cutting the classification tree generated by agglomerative hierarchical clustering with complete linkage to create the desired number of groups.

Our analysis suggested that the data could be best understood in terms of 7 clusters of respondents, displayed below. The table shows, for example, that among members of group 1, 0% of people are members of the EA Forum, Facebook, LessWrong, The Life You Can Save a local group, while 19% are members of Giving What We Can. By contrast, in group 5, 100% of members are part of EA Facebook and LessWrong and a local EA group and 50% are members of the EA Forum.

![Table of the clustering data](/img/cluster-table.png)

!["Size of Clusters" bar chart](/img/cluster-bar.png)

![legend table for the clustering](/img/cluster2.png)

How exactly to interpret these clusters in the data is not exactly intuitive or straightforward. Nevertheless, we think it highlights a few groupings of interest. For example, it identifies a cluster (1) of 709 people (27.7% of respondents) who do not report being members of any of the EA groups listed other than a minority having taken the GWWC pledge. Clusters 2 (16.2%) and 3 (18.54%), conversely, represent clusters that are largely involved in EA Facebook, local groups (and, for group 2, GWWC), but not the EA Forum or LessWrong. Cluster 4 are all local group members, but not members of most other groups. Cluster 5 (6.21%) and cluster 7 (11.98%) conversely, represent two distinct clusters that are highly engaged across a selection of groups.

Notably these clusters correspond fairly intuitively with differences that we previously noted in the [cause selection](https://forum.effectivealtruism.org/posts/hP6oEXurLrDXyEzcT/ea-survey-2018-series-cause-selections) post. Clusters 1-4 each have a plurality of respondents selecting Global Poverty as the top cause, whereas 5 and 7 (who have higher membership across a variety of highly involved groups), along with cluster 6, which is primarily LW members who are otherwise not engaged with EA groups, have a plurality of respondents selecting AI as the top cause. Similarly, cluster 1 the cluster with the lowest level of engagement, has the highest support for Climate Change as a cause.

## Gender Differences in Group Membership

One more sensitive finding was the relationship between gender and membership of different EA groups. Across virtually every category of group membership, a lower percentage of women were members relative to the sample as a whole. The one exception is The Life You Can Save Pledge, which appears to have a slightly higher percentage of women.

![Gender table](/img/gender.png)

A different way to look at this is the % of women and men, in our sample, who were members of the different groups. Note that the number of respondents for the categories “Other” and “Prefer not to answer” were not included in the analysis below as the very small number of responses would limit statistical analysis.

![Group differences table](/img/group-differences.png)

Of course, it is impossible to infer much about the cause of these differences from these results, nevertheless, it seems worth noting as potentially relevant to ongoing discussions about demographic differences within EA.

## Conclusion

Overall, these analyses suggest that a fairly large proportion of EAs, in our sample at least, are not members of many EA groups. While moderately large portions of our sample were involved either in the EA Facebook group (\~50%), a local group (\~40%) or the EA Forum (~20%), relatively small numbers of individuals were involved in a wide variety of different groups. This seems to accord with a common view that, among EAs, a relatively small subset are highly involved, at least in terms of group membership alongside others with differing levels of involvement.

We will be exploring possible predictors of individuals being more likely to be highly involved in EA groups in a [follow-up post](https://forum.effectivealtruism.org/posts/S4WmbHJr32WcmwFD7/ea-survey-series-2018-where-people-first-hear-about-ea-and).

\[1] Note that the percentage female for GWWC pledges as a whole (which includes members who are not necessarily effective altruists) is estimated to be roughly 30%- higher than within the effective altruist sample, though far from gender parity.

**Credits**

This post was written and with analysis by David Moss, Neil Dullaghan and Kim Cuddington.

Thanks to Julia Wise for comment and to Peter Hurford for review and editing.

_The annual EA Survey is a project of Rethink Charity with analysis and commentary from researchers at Rethink Priorities._

**Supporting Documents**

Articles in the 2018 EA Survey Series:

* [I - Community Demographics & Characteristics](http://effective-altruism.com/ea/1th/ea_survey_2018_series_community_demographics/)
* [II - Distribution & Analysis Methodology](https://forum.effectivealtruism.org/posts/iSjttL9PPq9eiqrc3/ea-survey-2018-series-distribution-and-analysis-methodology)
* [III - How do people get involved in EA?](https://forum.effectivealtruism.org/posts/uPFx462NAamBo5Eqq/ea-survey-series-2018-how-do-people-get-involved-in-ea)
* [IV - Subscribers and Identifiers](https://forum.effectivealtruism.org/posts/K2u4rvy38YmSnhQ5X/ea-survey-series-2018-subscribers-and-identifiers)
* [V - Donation Data](https://forum.effectivealtruism.org/posts/SnE9FpArs2uXJsRtB/ea-survey-2018-series-donation-data)
* [VI - Cause Selection](https://forum.effectivealtruism.org/posts/hP6oEXurLrDXyEzcT/ea-survey-2018-series-cause-selections)
* [VIII- Where People First Hear About EA and Influences on Involvement](https://forum.effectivealtruism.org/posts/S4WmbHJr32WcmwFD7/ea-survey-series-2018-where-people-first-hear-about-ea-and)

Prior EA Surveys conducted by Rethink Charity:

* [The 2017 Survey of Effective Altruists](https://forum.effectivealtruism.org/posts/TuzkYANf7tmQDF2Hk/ea-survey-2017-series-distribution-and-analysis-methodology)
* [The 2015 Survey of Effective Altruists: Results and Analysis](https://forum.effectivealtruism.org/posts/EqgF5amS96TahanzK/the-2015-survey-of-effective-altruists-results-and-analysis)
* [The 2014 Survey of Effective Altruists: Results and Analysis](https://forum.effectivealtruism.org/posts/z5swaf6342AbG93Mp/the-2014-survey-of-effective-altruists-results-and-analysis)