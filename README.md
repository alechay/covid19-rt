# covid19-rt
Calculation of Rt values from COVID-19 daily case counts

We require statistical consultation and support for a public health study analyzing data for several Public Health Units in the province of Ontario.

The first analysis will be:

1. Calculate weekly Rt values from the daily COVID-19 case counts from the attached Excel file (i.e. between March 1 and now) for Ontario, Waterloo, York, Toronto, and Peel region.

The second analysis will be:

2. Segmented regressions to identify changes in slope/breakpoints in the behavior of Rt over time (and shifts in COVID-19 transmission trends) in each of the Public Health Units and Ontario as a whole. Please see the example attached.

Regressions will be based on zero to eight breaking points, using slope changes/discrete regression segments with at least five data points per segment. Calculate the best-model’s intercepts and slopes, using separate intercepts at each different segment, allowing for separate identification of increases or decreases in Rt, and sudden “jumps” or “plunges” in daily values.

Colour code similar to the example attached the periods of increasing restrictions (dark red for lockdown, light red for increasing restrictions, green for decreasing restrictions)

3. Correlation analysis between Rt and global mobility index (at lockdown, 7 days after, and 14 days after), as in the example graph I will attach. Data set is the same as before.

See below for more details from the methods:

"We calculated correlation between global mobility score (and each of the 6 types) and Rt for each public health unit (PHU) via ordinary least square regression, accounting for time lag:

COVs,t=αS+βiMobi, s,t−n+γt+εs,t (n = 0,1,…,t − 1),
(4)

COV is Rt on date t. Mobi denotes each type i (i=1, 2…6) of mobility; and Mobi, s,t−n is the mobility index in PHU s on the date (t − n). n equals 0, 7, and 14. βi is the standardised coefficient for each type of mobility; ε is the standardised error; αS denotes the fixed place effect of state s and γt denotes the fixed date effect for a transmission period after date t.
