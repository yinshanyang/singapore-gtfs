# Singapore GTFS (Updated 2018-04-28)

Pardon my language, but getting a version of the public transport schedule in Singapore in GTFS format is almost impossible. This is a composed version of the data based on scheduling data available online gathered through scripts and some manual data entry.

It might be dirty in places.

## Notes

### Weekdays only

At the moment, only weekday schedules are covered. The reason behind this is that my needs only required this amount of schedule information. The effort to cover Saturday and Sunday didn’t justify the returns.

So much as possible, the peak and off-peak hours and frequencies are represented.

### Frequencies are Averages

Frequencies are taken as the average of the range provided from information online.

### Bus Schedules

`stop_times` are generated through looking at the delta between first/last bus arrival timings. There are some instances where the deltas are still negative and an educated guess based on distance travelled is used to calculate the delta.

### LRT Schedules

The LRT schedules are manually put together, and due to the lack of updated information, or simply the complexity of the lines (looking at you Bukit Panjang LRT), some assumptions were made to simplify the data entry without causing too much impact on the resulting schedule.
