Analysis of Child Detention at the US-Mexico Border
================
Vikas Maturi

-   [Summary](#summary)
    -   [Context](#context)
    -   [Key questions](#key-questions)
    -   [Prior reporting](#prior-reporting)
    -   [Next steps](#next-steps)
        -   [Questions](#questions)
    -   [Data](#data)
-   [Libraries, parameters, and data
    import](#libraries-parameters-and-data-import)
-   [Analysis 1: Length of detention](#analysis-1-length-of-detention)
    -   [Q1: What were the lengths of the longest stays of children in
        immigration
        detention?](#q1-what-were-the-lengths-of-the-longest-stays-of-children-in-immigration-detention)
        -   [A large percentage of children are kept past the legal
            limit - some vastly
            longer](#a-large-percentage-of-children-are-kept-past-the-legal-limit---some-vastly-longer)
    -   [Q2: How does time in detention vary by
        site?](#q2-how-does-time-in-detention-vary-by-site)
        -   [Detentions in San Diego consistently far exceed the legal
            limit](#detentions-in-san-diego-consistently-far-exceed-the-legal-limit)
        -   [Detentions between ports of entry also consistently far
            exceed the legal
            limit](#detentions-between-ports-of-entry-also-consistently-far-exceed-the-legal-limit)
    -   [Q3: How old were the children detained for long periods of
        time?](#q3-how-old-were-the-children-detained-for-long-periods-of-time)
        -   [Over 100 children under the age of 5 were detained for more
            than 30
            days](#over-100-children-under-the-age-of-5-were-detained-for-more-than-30-days)
    -   [Q4: What was the average length of detainment, by
        age](#q4-what-was-the-average-length-of-detainment-by-age)
        -   [Age group is not clearly correlated with detention
            time](#age-group-is-not-clearly-correlated-with-detention-time)
-   [Analysis 2: Detentions across nationality and age
    group](#analysis-2-detentions-across-nationality-and-age-group)
    -   [Q1: What are the countries of citizenship with the most
        children
        detained?](#q1-what-are-the-countries-of-citizenship-with-the-most-children-detained)
        -   [The highest levels of child migration are from Guatemala,
            Honduras, El Salvador, and
            Mexico](#the-highest-levels-of-child-migration-are-from-guatemala-honduras-el-salvador-and-mexico)
    -   [Q2: What are the most common non-Central American citizenships
        for detained children to
        hold?](#q2-what-are-the-most-common-non-central-american-citizenships-for-detained-children-to-hold)
        -   [The highest levels of child migration from
            non-Central/South American countries are from older
            Indians](#the-highest-levels-of-child-migration-from-non-centralsouth-american-countries-are-from-older-indians)

## Summary

#### Context

This analysis explores data on child detention during the Trump
administration (January 2017 to January 2020). Children are detained
after they cross the US-Mexico border. Many detained children travel
alone (unaccompanied), while others are detained with their family unit.
The Trump administration???s family separation policy took children away
from their parents during a substantial portion of their detention.
Detentions are carried out by US Customs and Border Protection agents.
Once detained, children are held in CBP facilities. These facilities are
not meant for long-term detention, but for short-term stays. The law
states that unaccompanied minor children can not be detained for more
than 72 hours. After 72 hours, unaccompanied children must be
transferred from immigration detention to the Office of Refugee
Resettlement (a part of the Department of Health and Human Services),
where they reside in ORR shelters. For children detained with their
families, A 2015 court order, based on a document called the Flores
settlement, prevents the government from keeping migrant children in
detention for more than 20 days. \[1\]

The Marshall Project???s reporting on this topic found that children were
consistently detained for far longer than 72 hours, particularly during
peaks of border crossings. Reports indicate that children separated from
their families under the Trump administration???s family separation policy
were treated similarly to unaccompanied minors. \[1\]

#### Key questions

We explore:

-   The longest times that children were held in immigration detention
-   The number of children were held in immigration detention at the
    US-Mexico border beyond the 72-hour legal limit, across detention
    sites and age groups
-   A few other topics, including differences in the citizenship and age
    group of children detained

**We find:**

-   A large percentage of children (33%) are kept in immigration
    detention past the legal limit (72 hours, or 3 days)
-   19 children were kept in immigration detention for over 6 months
    (over 50x the legal limit), and 3 children for over 1 year (over
    100x the legal limit)
-   Over 100 children under the age of 5 were kept in immigration
    detention for longer than 1 month

#### Prior reporting

This analysis extends the fantastic work of the [The Marshall
Project](https://www.themarshallproject.org/2020/10/30/500-000-kids-30-million-hours-trump-s-vast-expansion-of-child-detention),
profiled in their piece [500,000 Kids, 30 Million Hours: Trump???s Vast
Expansion of Child
Detention](https://www.themarshallproject.org/2020/10/30/500-000-kids-30-million-hours-trump-s-vast-expansion-of-child-detention).

1.  [What We Know: Family Separation And ???Zero Tolerance??? At The Border
    (NPR)](https://www.npr.org/2018/06/19/621065383/what-we-know-family-separation-and-zero-tolerance-at-the-border)
2.  [500,000 Kids, 30 Million Hours: Trump???s Vast Expansion of Child
    Detention](https://www.themarshallproject.org/2020/10/30/500-000-kids-30-million-hours-trump-s-vast-expansion-of-child-detention).
3.  [What it was like working with migrant children inside the San Diego
    Convention
    Center](https://www.sandiegouniontribune.com/news/immigration/story/2021-08-08/migrant-children-san-diego-convention-center)
4.  [More Migrants From India Try To Get Into U.S. From
    Mexico](https://www.npr.org/2020/05/18/857727126/more-migrants-from-india-try-to-get-into-u-s-from-mexico)

#### Next steps

##### Questions

For the Marshall Project:

1.  Do we have more recent data (e.g., 2020 to present) that has been
    cleaned and summarized in the same way
2.  For the data entries where hours_in_custody was added, many of them
    are among the largest hours_in_custody of any children. Why is this
    the case?
3.  Do the child detentions in this dataset include or exclude children
    that were NOT separated from their parents?
4.  Have the primary questions that are the focus of this analysis
    already been considered / analyzed / investigated?

#### Data

The Marshall Project made the data used for this reporting available
[here](https://observablehq.com/@themarshallproject/cbp-child-detentions-2017-to-2020),
which we leveraged in our analysis.

The data is a combination of two sources:

-   CBP Office of Field Operations (OFO) child detentions: Detentions of
    children at ports of entry by the U.S. Customs and Border Protection
    Border Patrol between mid-January of 2017 and late January of 2020.
-   CBP Border Patrol (BP) child detentions: Detentions of children
    between ports of entry by the U.S. Customs and Border Protection
    Office of Field Operations between mid-January of 2017 and mid-June
    of 2020.

The file includes these fields:

-   date_in: Custody book-in time and date
-   date_out: Custody book-out time and date
-   app_date: Apprehension date (OFO dataset)
-   hours_in_custody: Time in custody in hours
-   age_group: Age group of child (grouped by Marshall Project
    reporters)
-   gender: Child gender
-   citizenship: Child country of citizenship
-   border: Border (BP dataset)
-   field_office: Field office name (OFO dataset)
-   source: Data source; ???OFO??? or ???BP???.

*Summary of the data sources is from the Marshall Project*

## Libraries, parameters, and data import

Read in the raw data

``` r
# load library for pipes
library(magrittr)

# data files
file_child_detention_data <- "https://raw.githubusercontent.com/themarshallproject/cbp-migrantchildren-detention-data/main/data/cbp_foia_response-oct_2020.csv"

# read in raw data; specify column types
data_raw <- 
  readr::read_csv(
    file = file_child_detention_data, 
    col_types = list(
      readr::col_datetime(format = ""),
      readr::col_datetime(format = ""),
      readr::col_character(),
      readr::col_double(),
      readr::col_character(),
      readr::col_character(),
      readr::col_character(),
      readr::col_character(),
      readr::col_character(),
      readr::col_character(),
      readr::col_character()
    )
  )

# Display a few rows of the raw data
data_raw %>% 
  head(5) %>% 
  knitr::kable()
```

| date_in             | date_out            | app_date | hours_in_custody | age_group   | gender | citizenship | border | sector     | field_office | source |
|:--------------------|:--------------------|:---------|-----------------:|:------------|:-------|:------------|:-------|:-----------|:-------------|:-------|
| 2017-01-20 00:10:00 | 2017-01-20 10:08:00 | NA       |          9.95000 | 6-8 years   | Female | EL SALVADOR | SBO    | (b)(7)(E ) | NA           | BP     |
| 2017-01-20 00:15:00 | 2017-01-24 17:30:00 | NA       |        113.23333 | 3-5 years   | Female | GUATEMALA   | SBO    | (b)(7)(E ) | NA           | BP     |
| 2017-01-20 00:22:00 | 2017-01-24 17:47:00 | NA       |        113.41667 | 3-5 years   | Female | BRAZIL      | SBO    | (b)(7)(E ) | NA           | BP     |
| 2017-01-20 00:30:00 | 2017-01-21 06:35:00 | NA       |         30.08333 | 12-14 years | Male   | EL SALVADOR | SBO    | (b)(7)(E ) | NA           | BP     |
| 2017-01-20 00:30:00 | 2017-01-21 13:03:00 | NA       |         36.53333 | 3-5 years   | Male   | HONDURAS    | SBO    | (b)(7)(E ) | NA           | BP     |

Clean the data

``` r
# According to the metadata provided by The Marshall Project, when the CBP detains a child (rather than ORR), it is by definition between a port of entry

data_clean <-
  data_raw %>% 
  # Add in "between port of entry" field office
  dplyr::mutate(
    field_office = dplyr::case_when(
      is.na(field_office) ~ "between_ports_of_entry",
      !is.na(field_office) ~ field_office,
      TRUE ~ field_office
    )
  ) %>% 
  # filter out entries where we do not have recorded date_in or date_out data
  dplyr::filter(!is.na(date_out), !is.na(date_in)) %>% 
  # add hours in custody where not recorded (but both date_out and date_in data are available)
  dplyr::mutate(
    manually_added_hours = dplyr::if_else(is.na(hours_in_custody), 1, 0), 
    hours_in_custody = dplyr::case_when(
      !is.na(hours_in_custody) ~ hours_in_custody, 
      is.na(hours_in_custody) ~ round(as.numeric(difftime(date_out, date_in, units = "hours")), 4),
      TRUE ~ NaN
    ),
    # make age_group a factor for reliable plotting order
    age_group = factor(age_group, levels = c("Under 1 year", "1-2 years", "3-5 years", "6-8 years", "9-11 years", "12-14 years", "15-18 years"), ordered = TRUE)
  ) %>% 
  # fill in data for hours_in_custody when the date_in and date_out information are available
  dplyr::filter(hours_in_custody > 0)
```

## Analysis 1: Length of detention

#### Q1: What were the lengths of the longest stays of children in immigration detention?

``` r
# calculate days in detention, select relevant columns
detention_length <- 
  data_clean %>% 
  dplyr::arrange(dplyr::desc(hours_in_custody)) %>% 
  dplyr::mutate(days_in_custody = hours_in_custody / 24) %>% 
  dplyr::select(date_in, date_out, hours_in_custody, days_in_custody, manually_added_hours, dplyr::everything())

# count the number of children detained for more than 72 hours (beyond the legal limit)
num_over_72_hours <-
  detention_length %>% 
  dplyr::filter(days_in_custody > 3) %>% 
  dplyr::count()

# calculate the total number of children in the dataset
total_num_children <- 
  data_clean %>% 
  dplyr::count() %>% 
  dplyr::pull() %>% 
  purrr::pluck(1)

# calculate the total number of children that were detained for at least x days (for all x > 3)
num_over_x_days <-
  detention_length %>% 
  dplyr::filter(days_in_custody > 3) %>% 
  dplyr::mutate(round_days_in_custody = round(days_in_custody, 0)) %>% 
  dplyr::count(round_days_in_custody) %>%  
  dplyr::rename(num_of_children = n) %>% 
  dplyr::arrange(dplyr::desc(round_days_in_custody)) %>% 
  dplyr::mutate(
    num_of_children_higher_days = cumsum(num_of_children), 
    prop_children_higher_days = round(num_of_children_higher_days / total_num_children, 6)
  )
```

``` r
# display the table for the most days
num_over_x_days %>% 
  head(20) %>% 
  knitr::kable()
```

| round_days_in_custody | num_of_children | num_of_children_higher_days | prop_children_higher_days |
|----------------------:|----------------:|----------------------------:|--------------------------:|
|                   586 |               1 |                           1 |                   2.0e-06 |
|                   558 |               1 |                           2 |                   3.0e-06 |
|                   371 |               1 |                           3 |                   5.0e-06 |
|                   258 |               1 |                           4 |                   7.0e-06 |
|                   247 |               1 |                           5 |                   9.0e-06 |
|                   240 |               2 |                           7 |                   1.2e-05 |
|                   224 |               1 |                           8 |                   1.4e-05 |
|                   211 |               1 |                           9 |                   1.5e-05 |
|                   205 |               1 |                          10 |                   1.7e-05 |
|                   204 |               1 |                          11 |                   1.9e-05 |
|                   191 |               1 |                          12 |                   2.1e-05 |
|                   190 |               3 |                          15 |                   2.6e-05 |
|                   189 |               2 |                          17 |                   2.9e-05 |
|                   180 |               2 |                          19 |                   3.3e-05 |
|                   179 |               6 |                          25 |                   4.3e-05 |
|                   173 |               2 |                          27 |                   4.6e-05 |
|                   171 |               1 |                          28 |                   4.8e-05 |
|                   168 |               1 |                          29 |                   5.0e-05 |
|                   145 |               1 |                          30 |                   5.2e-05 |
|                   140 |               5 |                          35 |                   6.0e-05 |

Number (and percentage) of all children detained that were kept in
detention for at least x days

``` r
# display the table for the days just over the legal limit
num_over_x_days %>% 
  dplyr::arrange(round_days_in_custody) %>% 
  head(10) %>% 
  dplyr::arrange(dplyr::desc(round_days_in_custody)) %>% 
  knitr::kable()
```

| round_days_in_custody | num_of_children | num_of_children_higher_days | prop_children_higher_days |
|----------------------:|----------------:|----------------------------:|--------------------------:|
|                    12 |             845 |                        4383 |                  0.007526 |
|                    11 |            1249 |                        5632 |                  0.009670 |
|                    10 |            2197 |                        7829 |                  0.013442 |
|                     9 |            3944 |                       11773 |                  0.020214 |
|                     8 |            5928 |                       17701 |                  0.030392 |
|                     7 |           10659 |                       28360 |                  0.048694 |
|                     6 |           19441 |                       47801 |                  0.082074 |
|                     5 |           35985 |                       83786 |                  0.143860 |
|                     4 |           69374 |                      153160 |                  0.262974 |
|                     3 |           40762 |                      193922 |                  0.332962 |

Number (and percentage) of all children detained that were kept in
detention for at least x days

##### A large percentage of children are kept past the legal limit - some vastly longer

The understood legal limit is 3 days (72 hours). We find here that:

-   193,922 children (33% of all children) were detained for longer than
    72 hours
-   47,801 children (8% of all children) detained for 6 days - 2x longer
    than the legal limit
-   11,773 children (1.9% of all children) detained for 9 days - 3x
    longer than legal limit
-   1,429 children detained longer than 18 days (6x longer than legal
    limit)
-   353 children longer than 1 month (30 days)
-   61 children longer than 3 months (> 90 days)
-   56 children longer than 100 days
-   19 children for more than 6 months (>180 days)
-   3 children for more than 1 year

Data, if accurate, indicate that many children spent longer than the
legal limit - some vastly longer than allowed.

Example full data of children kept \> 225 days in custody

``` r
detention_length %>% 
  dplyr::arrange(dplyr::desc(hours_in_custody)) %>% 
  dplyr::filter(days_in_custody > 225) %>% 
  knitr::kable()
```

| date_in             | date_out            | hours_in_custody | days_in_custody | manually_added_hours | app_date | age_group   | gender | citizenship | border | sector     | field_office           | source |
|:--------------------|:--------------------|-----------------:|----------------:|---------------------:|:---------|:------------|:-------|:------------|:-------|:-----------|:-----------------------|:-------|
| 2017-02-24 17:15:00 | 2018-10-03 10:19:00 |        14057.067 |        585.7111 |                    1 | NA       | 6-8 years   | Female | EL SALVADOR | SBO    | (b)(7)(E ) | between_ports_of_entry | BP     |
| 2017-03-24 20:20:00 | 2018-10-03 10:20:00 |        13382.000 |        557.5833 |                    1 | NA       | 15-18 years | Male   | MEXICO      | SBO    | (b)(7)(E ) | between_ports_of_entry | BP     |
| 2017-11-15 19:35:00 | 2018-11-22 00:00:00 |         8908.417 |        371.1840 |                    1 | NA       | 15-18 years | Male   | EL SALVADOR | CBO    | (b)(7)(E ) | between_ports_of_entry | BP     |
| 2019-05-16 13:20:00 | 2020-01-29 15:45:00 |         6194.417 |        258.1007 |                    1 | NA       | 6-8 years   | Female | EL SALVADOR | SBO    | (b)(7)(E ) | between_ports_of_entry | BP     |
| 2017-02-15 00:00:00 | 2017-10-20 08:26:00 |         5936.433 |        247.3514 |                    1 | NA       | 15-18 years | Male   | MEXICO      | SBO    | (b)(7)(E ) | between_ports_of_entry | BP     |
| 2018-06-05 15:04:00 | 2019-01-31 13:02:00 |         5757.967 |        239.9153 |                    1 | NA       | 6-8 years   | Male   | GUATEMALA   | SBO    | (b)(7)(E ) | between_ports_of_entry | BP     |
| 2018-06-05 15:04:00 | 2019-01-31 13:02:00 |         5757.967 |        239.9153 |                    1 | NA       | 15-18 years | Male   | GUATEMALA   | SBO    | (b)(7)(E ) | between_ports_of_entry | BP     |

Flag: Children with the longest times in detention had their
hours_in_custody manually added into the data (the calculation of their
hours was not done in the default dataset from the Marshall Project). We
should understand why that is the case.

#### Q2: How does time in detention vary by site?

``` r
# create a table with hour blocks for visualization
field_over_time <-
  data_clean %>% 
  dplyr::mutate(
    semester_raw = dplyr::if_else(lubridate::semester(date_in, with_year = FALSE) == 1, "Jan-June", "Jul-Dec"),
    year = as.character(lubridate::year(date_in)),
    hours_custody_group = round(hours_in_custody / 8, 0),
    hours_custody_group = dplyr::case_when(
      hours_custody_group == 0 ~ "0 to 8 hours",
      hours_custody_group == 1 ~ "8 to 16 hours",
      hours_custody_group == 2 ~ "16 to 24 hours",
      hours_custody_group == 3 ~ "24 to 32 hours", 
      hours_custody_group == 4 ~ "32 to 40 hours",
      hours_custody_group == 5 ~ "40 to 48 hours", 
      hours_custody_group == 6 ~ "48 to 56 hours", 
      hours_custody_group == 7 ~ "56 to 64 hours", 
      hours_custody_group == 8 ~ "64 to 72 hours", 
      hours_custody_group == 9 ~ "72 to 80 hours",
      hours_custody_group == 10 ~ "80 to 88 hours", 
      hours_custody_group == 11 ~ "88 to 96 hours", 
      hours_custody_group == 12 ~ "96 to 104 hours", 
      hours_custody_group == 13 ~ "104 to 112 hours", 
      hours_custody_group == 14 ~ "112 to 120 hours",
      hours_custody_group == 15 ~ "120 to 128 hours", 
      hours_custody_group == 16 ~ "128 to 136 hours", 
      hours_custody_group == 17 ~ "136 to 144 hours", 
      hours_custody_group > 17 ~ "144 hours or more",
      TRUE ~ NA_character_
    ),
    hours_custody_group = factor(
      hours_custody_group, 
      levels = c("0 to 8 hours", "8 to 16 hours", "16 to 24 hours", "24 to 32 hours", "32 to 40 hours", "40 to 48 hours", "48 to 56 hours", "56 to 64 hours", "64 to 72 hours", "72 to 80 hours", "80 to 88 hours", "88 to 96 hours", "96 to 104 hours", "104 to 112 hours", "112 to 120 hours", "120 to 128 hours", "128 to 136 hours", "136 to 144 hours", "144 hours or more"), 
      ordered = TRUE)
  ) %>% 
  tidyr::unite("semester", semester_raw, year, sep = " ") %>% 
  dplyr::mutate(semester = factor(semester, ordered = TRUE, levels = c("Jan-June 2017", "Jul-Dec 2017", "Jan-June 2018", "Jul-Dec 2018", "Jan-June 2019", "Jul-Dec 2019", "Jan-June 2020"))) %>% 
  dplyr::count(hours_custody_group, semester, field_office) %>% 
  dplyr::mutate(
    legal_limit = ifelse(hours_custody_group %in% c("0 to 8 hours", "8 to 16 hours", "16 to 24 hours", "24 to 32 hours", "32 to 40 hours", "40 to 48 hours", "48 to 56 hours", "56 to 64 hours", "64 to 72 hours"), "Under 72 hours", "Over 72 hours"),
    legal_limit = factor(legal_limit, ordered = TRUE, levels = c("Under 72 hours", "Over 72 hours"))
  )
```

##### Detentions in San Diego consistently far exceed the legal limit

``` r
# ggplot theme load
ggthemr::ggthemr(palette = 'dust', layout = "clean")

# plot hours in custody based on the immigration detention center children entered at
field_over_time %>% 
  dplyr::filter(!field_office == "between_ports_of_entry") %>% 
  ggplot2::ggplot(ggplot2::aes(x = hours_custody_group, y = n, fill = legal_limit, group = legal_limit)) +
  ggplot2::geom_col() + 
  ggplot2::facet_grid(field_office~semester) +
  ggplot2::scale_fill_manual(values = c("rosybrown2", "tomato1")) +
  ggplot2::scale_x_discrete(breaks = c("0 to 8 hours", "72 to 80 hours", "144 hours or more"), labels = c("0", "72 hrs", "144+")) +
  ggplot2::scale_y_continuous(breaks = c(1000, 2000), labels = c("1000", "2000"), limits = c(0, 2000)) +
  ggplot2::theme(
    axis.text.x = ggplot2::element_text(angle = 45, hjust = 1), 
    legend.position = "bottom", 
    panel.grid.major.y = ggplot2::element_line(size = .5)
  ) +
  ggplot2::labs(
    title = "Time in immigration detention by field office and semester", 
    subtitle = "The San Diego field office detained children for far longer than the 72 hour limit, even as they detained fewer children than Laredo", 
    y = "Number of children in custody", 
    x = "Hours detained",
    fill = "Legal limit"
  )
```

![](detentions_files/figure-gfm/unnamed-chunk-8-1.png)<!-- -->

Of detentions happening at border patrol sites, those happening in San
Diego are far more likely to result in detention lengths far longer than
legally allowed. Conversely, Laredo has similar number of detentions,
but far more childre are detained for less than 72 hours.

##### Detentions between ports of entry also consistently far exceed the legal limit

``` r
# ggplot theme load
ggthemr::ggthemr(palette = 'dust', layout = "clean")

# plot hours in custody based on the the semester of entry, for those entering between ports of entry
field_over_time %>% 
  dplyr::filter(field_office == "between_ports_of_entry") %>% 
  ggplot2::ggplot(ggplot2::aes(x = hours_custody_group, y = n, fill = legal_limit, group = legal_limit)) +
  ggplot2::geom_col() + 
  ggplot2::facet_grid(~semester) +
  ggplot2::scale_fill_manual(values = c("rosybrown2", "tomato1")) +
  ggplot2::scale_x_discrete(breaks = c("0 to 8 hours", "72 to 80 hours", "144 hours or more"), labels = c("0", "72 hrs", "144+")) +
  #ggplot2::scale_y_continuous(breaks = c(1000, 2000), labels = c("1000", "2000")) +
  ggplot2::theme(
    axis.text.x = ggplot2::element_text(angle = 45, hjust = 1), 
    legend.position = "bottom", 
    panel.grid.major.y = ggplot2::element_line(size = .5)
  ) +
  ggplot2::labs(
    title = "Time in immigration detention by semester", 
    subtitle = "Vastly more children are detained between ports of entry, and a substantial number are held for longer than the 72 hour limit", 
    y = "Number of children in custody", 
    x = "Hours detained",
    fill = "Legal limit"
  )
```

![](detentions_files/figure-gfm/unnamed-chunk-9-1.png)<!-- -->

For those children detained between port of entry, we find that many -
particularly at the peak of detentions in the first six months of 2019 -
were detained more than 72 hours.

#### Q3: How old were the children detained for long periods of time?

``` r
# calculate distribution of age group for children held for one month (30 days) or longer)
one_month <-
  detention_length %>% 
  dplyr::filter(days_in_custody > 30) %>% 
  dplyr::count(age_group)
```

##### Over 100 children under the age of 5 were detained for more than 30 days

``` r
# ggplot theme load
ggthemr::ggthemr(palette = 'dust', layout = "clean")

one_month %>% 
  ggplot2::ggplot(ggplot2::aes(x = age_group, y = n)) +
  ggplot2::geom_col() +
  ggplot2::theme(
    axis.text.x = ggplot2::element_text(angle = 45, hjust = 1)
  ) + 
  ggplot2::labs(
    title = "Distribution of age group for children detained for more than one month", 
    subtitle = "Over 100 children under the age of 5 were detained for more than 30 days", 
    y = "Number of children detained for more than one month", 
    x = "Age group"
  )
```

![](detentions_files/figure-gfm/unnamed-chunk-11-1.png)<!-- -->

Over 100 children 5 and under were detained for 30+ days

#### Q4: What was the average length of detainment, by age

``` r
detainment_by_age <-
  detention_length %>% 
  dplyr::mutate(
    gender = dplyr::case_when(
      gender %in% c("F - FEMALE", "Female") ~ "Female", 
      gender %in% c("M - MALE", "Male") ~ "Male", 
      TRUE ~ "Unknown"
    )
  ) %>% 
  dplyr::group_by(age_group, gender) %>% 
  dplyr::summarise(
    mean_hours_in_custody = mean(hours_in_custody, na.rm = TRUE),
    n = dplyr::n()
  ) %>% 
  dplyr::filter(!is.na(age_group), !gender == "Unknown")
```

    ## `summarise()` has grouped output by 'age_group'. You can override using the `.groups` argument.

##### Age group is not clearly correlated with detention time

``` r
# ggplot theme load
ggthemr::ggthemr(palette = 'dust', layout = "clean")

detainment_by_age %>% 
  ggplot2::ggplot(ggplot2::aes(x = age_group, y = mean_hours_in_custody, group = gender, fill = gender)) +
  ggplot2::geom_col(position = "dodge") +
  ggplot2::theme_light() +
  ggplot2::theme(
    axis.text.x = ggplot2::element_text(angle = 45, hjust = 1)
  ) + 
  ggplot2::labs(
    title = "Average hours in custody by age group", 
    subtitle = "Age group is not clearly correlated with detention time", 
    y = "Average hours in custody", 
    x = "Age group", 
    fill = "Gender"
  )
```

![](detentions_files/figure-gfm/unnamed-chunk-13-1.png)<!-- -->

Hours in custody does not seem to vary widely by gender and age, though
15-18 year old males tend to be released fastest.

## Analysis 2: Detentions across nationality and age group

#### Q1: What are the countries of citizenship with the most children detained?

``` r
top_cross_nationality <-
  data_clean %>% 
  dplyr::count(citizenship) %>% 
  dplyr::arrange(dplyr::desc(n)) %>% 
  dplyr::filter(n > 3000) %>% 
  dplyr::pull(citizenship)

nationality_crossing <-
  data_clean %>% 
  dplyr::count(citizenship, age_group) %>% 
  dplyr::filter(citizenship %in% top_cross_nationality, !is.na(age_group))
```

##### The highest levels of child migration are from Guatemala, Honduras, El Salvador, and Mexico

``` r
# ggplot theme load
ggthemr::ggthemr(palette = 'dust', layout = "clean")

nationality_crossing %>% 
  ggplot2::ggplot(ggplot2::aes(x = age_group, y = n)) +
  ggplot2::geom_col() +
  ggplot2::facet_wrap(~citizenship) +
  ggplot2::theme(
    axis.text.x = ggplot2::element_text(angle = 45, hjust = 1)
  ) +
  ggplot2::labs(
    title = "Child detention by country of citizenship and age group",
    subtitle = "The highest levels of child migration are from Guatemala, Honduras, El Salvador, and Mexico", 
    y = "Number of children detained", 
    x = "Age group"
  )
```

![](detentions_files/figure-gfm/unnamed-chunk-15-1.png)<!-- -->

Many of those detained are older minors (particularly from Guatemala),
though a substantial proportion are young.

#### Q2: What are the most common non-Central American citizenships for detained children to hold?

``` r
middle_cross_nationality <-
  data_clean %>% 
  dplyr::count(citizenship) %>% 
  dplyr::arrange(dplyr::desc(n)) %>% 
  dplyr::filter(n < 3000, n > 500) %>% 
  dplyr::pull(citizenship)

other_continents <-
  data_clean %>% 
  dplyr::count(citizenship, age_group, border) %>% 
  dplyr::filter(citizenship %in% middle_cross_nationality, !is.na(age_group))
```

##### The highest levels of child migration from non-Central/South American countries are from older Indians

``` r
# ggplot theme load
ggthemr::ggthemr(palette = 'dust', layout = "clean")


other_continents %>% 
  ggplot2::ggplot(ggplot2::aes(x = age_group, y = n, group = border, fill = border)) +
  ggplot2::geom_col() +
  ggplot2::facet_wrap(~citizenship) +
  ggplot2::theme(
    axis.text.x = ggplot2::element_text(angle = 45, hjust = 1)
  ) +
  ggplot2::labs(
    title = "Child detention by country of citizenship and age group",
    subtitle = "The highest levels of child migration from non-Central/South American countries \nare from older Indians", 
    y = "Number of children detained", 
    x = "Age group"
  )
```

![](detentions_files/figure-gfm/unnamed-chunk-17-1.png)<!-- -->
