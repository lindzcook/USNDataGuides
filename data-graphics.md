# USN&WR Data and Graphics Style Guide

This style guide comprises the typographic and technical best practices used in the USN&WR newsroom.

Using rules consistently can make your job easier and can prevent readers from having to struggle with new interfaces on every project, but remember that overdependence on rules can hamper progress, and that "a foolish consistency is the hobgoblin of little minds." 

Finally, this is a living document. Please feel free to propose changes.

## Accuracy !!

The most important thing by far is to be accurate.

A full discussion on how to be sure you're accurate is beyond the scope of this document. Read "[Bulletproofing your data-based stories](data-bulletproofing.md)." Now.

## Asterisks !!

Asterisks and footnotes are artifacts of print, and lead to confusion on screen. Use [hovers](#hovers) instead.

## Axes

Always label axes except where the label would simply duplicate the headline or top matter.

## Bylines

Bylines are important measures of credit and responsibility. Just as every story has a byline, every news app and graphic should have a byline.

Bylines are in this format: "NAME for USN&WR"

If the chart is an image, bylines should appear on the actual image and on the credit line in the CMS, not simply below the image. For HTML embeds, bylines should be included in the HTML enhancement. Add the following HTML to the end of your enhancement: `<p>NAME for USN&WR</p>`. By adding credit in this manner, we ensure the byline remains with the content if it is reused.

## Charts

Use a bar chart to show discrete quantities.

Use a stacked bar chart to show the relative values of categories and subcategories of data.

Use a line chart (sometimes called a fever chart) to show continuous variables such as time series.

Use a scatterplot to show a correlation (or lack thereof) between two variables.

Bubble charts are acceptable where the accurate perception of fine differences between the circles is not important (see Maps). Circles in bubble charts should vary in area and not diameter or radius.

Avoid 3-D charts at all costs. Humans have enough problem perceiving area accurately. Asking them to perceive 3-D volume makes matters worse.

Use pie charts with caution. The information can likely be conveyed more clearly with a bar chart. [More on why.](http://www.excelcharts.com/blog/optimal-number-categories-pie-chart/)

Don't show interpolated or predicted data without saying you're doing so.

In annual trend data don't include partial years.

See also: [treemaps](#treemaps)

## Colors

Red-Green is the most common form of color blindness. Beware of using these colors to communicate data. To check if differences between colors can be perceived by color blind users, check [Color Oracle](http://colororacle.org/) or [Spectrum.] (https://chrome.google.com/webstore/detail/spectrum/ofclemegkcmilinpcimpjkfhjfgmhieb?hl=en)

When showing differences in rate of a single variable, stick to a single hue and vary value/lightness. For example, don't fade from blue to pink. The one exception is fading from red to green to show "bad" to "good" (and remember to check your reds and greens for color blindness accessibility). Beware of using numerical cut-offs for gradient-like colors, see [here](http://junkcharts.typepad.com/junk_charts/2014/08/people-are-happier-in-some-parts-of-the-country-as-labor-day-nears.html).

When use color to show category, use different colors instead of shades. 

## Color Breaks

Pick color breaks carefully. Your data may not be best represented with equal-interval breaks. See what patterns emerge using a variety of algorithms, such as quantiles, [Jenks natural breaks](http://en.wikipedia.org/wiki/Jenks_natural_breaks_optimization), [head/tail breaks](https://sites.google.com/site/thepowerofcartography/head-tail-breaks), standard deviation, or even arbitrary breaks that might make sense for your data. For example, if your data is average commute time to work, breaks of 10, 20, 30, 45 and 60+ minutes might make the most sense for readers, even if your data is not distributed normally among those breaks.

Make sure your color breaks don't mislead readers about the distribution of your data. For instance, if your values are mostly clustered between 1 and 10 but includes a few items above 1,000, make sure that the color that represents 1,000 is more than just one shade different than the color that represents 10. The Daily Beast uses a tool they made called [Histagram.me](http://www.histagram.me/) to examine the distribution of datasets.

If the pattern you see in your data only appears under a custom color break scale, rethink whether the pattern is actually in the data.

For color breaks in numerical data, see above.

## Corrections

News apps and graphics should follow your newsroom's standard corrections policy. Observe the following additions:

## Dashes

Stick with our policy for dashes in data descriptions.

## Data: Singular or Plural?

The world data is always plural. See stylebook entry: "data - always plural From AP: Data is a plural noun, it normally takes plural verbs and pronouns. AP's collective nouns entry includes examples of when data may take singular verbs and pronouns, but to avoid confusion and keep with USN standard practice, we stick with plural."

## Footnotes !!

Use [hovers](#hovers) instead. (See [asterisks](#asterisks))

## Geocoding

Geocoding is the process of matching address to latitude and longitude points. Use the geocoding guide for this, if you are geocoding large sets of data. For small sets, you can use [] or [] to find points in the city's center.

Always check geocoded data to make sure it isn't 1. in an ocean, 2. in China, 3. in the wrong state. 


## Headlines

Graphics should have a title. All text on graphics follow USN headline style.

## Hovers

!!

##Labels 

See Legends.

## Lead-in

(see [Top Matter](#topmatter)) !!

## Legends !! Transparency

Always include the information needed to understand the chart with the chart. That means transparency about what the data is, where it can from and its timeframe. 

In charts with only one element, include needed information on the axis or in the title. In charts with more than one element, use labels or a legend, depending on which is more clear. 

A legend must be visible on the reader's computer screen when the chart is visible. Legends should be in the same sequence as the charts they describe.

## Maps

Maps are best when showing data in which geography is an important variable. [Read "When Maps Shouldn't Be Maps" before making any maps](http://www.ericson.net/content/2011/10/when-maps-shouldnt-be-maps/).

All maps must be distinguishable from population maps. To accomplish this, the underlying data should control for population or other denominator. If you make a U.S. state choropleth map and the darkest states are New York, Texas and California, re-read this paragraph.

Avoid bubble maps, which represent the rate of a phenomenon at different locations using differently sized circles. This is for two reasons: First, people cannot accurately perceive differences in the area of circles. Second, bubble maps appear to show the geographic bounds of a phenomenon and not the rate of that phenomenon at the geographic center of the circle. This is another way of saying that they look too much like nuclear blast radius maps.

## Methodology !!link !!decimal points

Document any methodology and present it to readers clearly. Post a link to it prominently in the app or graphic. The methodology (or "nerd box") should detail the steps you took to clean the data and the exact analysis you ran on the data.

## Money

Use the appropriate currency symbols when showing currency. Avoid showing fractional currency like cents. In most cases, currency for multiple years should be adjusted to current year.

If you are comparing currency (such as costs, revenues, etc.) across multiple years, you should adjust for inflation. Don't ever refer to an amount of money being a "record" based on historical data that is not adjusted for inflation.

Always explain to readers whether and how you've adjusted currency figures. 

If you are using data from another source, always understand and make clear to readers if the data has been adjusted for inflation and what year's currency the data has been adjusted for.

## Numbers

The primary function of numbers in a news application or graphic is to help readers understand scale and order of magnitude, and compare against other numbers. Think of them more like words than like minutely precise coordinates (unless of course your numbers are literally coordinates).

Apply the following rules to numbers wherever they appear in your apps and graphics:

Except where special precision is required, round numbers and use whole numbers. Don't portray precision that doesn't really exist. This can be accomplished in Excel using the [ROUND function.](http://office.microsoft.com/en-us/excel-help/round-a-number-HP003056144.aspx)

When displaying numbers in a table, make them either right-aligned or decimal-aligned.

Except where special precision is required, abbreviate any number over 10,000 by truncating each number after the highest thousands place and appending a word or abbreviation indicating order of magnitude. Use one significant digit after the decimal point. For example:

    10,302,321 -> 10.3 million or 10.3M
    5,242,000,014 -> 5.2 billion or 5.2B
    901,212 -> 901.2 thousand or 901.2K or 0.9M

For numbers with more than three digits, always separate each thousands place with a comma.

Use AP style when using numbers in copy. That is, spell out numbers under 10 except in the following circumstances:

> Use figures for ages, sums of money, time of day, percentages, house numerals, years, days of the month, degrees of temperature, proportions, votes, scores, speeds, time of races, dimensions and serial numbers. ([via](https://websso.wwu.edu/down/index.shtml))

"Not available" and "not applicable" are abbreviated like this: N/A

##Reusing Graphics !!!

## States

Always seek to add clarity. 

In general, use USN headline style for all text on a graph, meaning the state abbreviation, separated by periods. For hovers, use the state's full name in sentence form. 

## Sources

Under every display of data, whether it's a map, chart, table or something else, show your data's sources. Our style is to combine the source with the credit line. For example, "Lindsey Cook for USN&WR, Source: FBI"

Link to the source or the best version of the source data whenever possible. If the data went through another party for cleaning or analysis, mention both in the source line. For example, "Source: FCC, Sunlight Foundation" for FCC comments data cleaned by the Sunlight Foundation.


## Top Matter

Put explanatory copy at the top of the first page of your app or graphic, under the byline. This copy goes by many names: "Lead-in," "top matter," etc. It should be very short -- aim for no more than four or five lines. Avoid re-telling a whole news story, but do make sure you accomplish three things:

1. Give the reader enough background to be able to understand the purpose of the app or graphic.
2. Let the reader know how to start using any interactivity.
3. Link to and briefly describe the related story, if any.

## Total

Only use "total" as an adjective when it's not clear what you're totaling. Never use the redundant "total amount" -- just use "total."

## Updates !!

Unlike an article, which tends to be a frozen description of a moment in time, news applications tend to be durable resources, and may need to be updated from time to time as new data becomes available.

When updating an app with new data, don't append a note explaining every change, as that note would be quite lengthy and very boring. Simply update the date in the byline to indicate when the data was last updated. If an app updates dynamically, the date in the byline should change dynamically as well.

Don't show both the original publication date and the most recent updated date in the byline. Your readers don't relish the archival history of our work quite like you might. Simply show the date of the latest update (after the word "updated," of course).

When the decision is reached to stop updating an app, put a prominent note on every page of the app that says when the app stopped being updated, and if possible, where to find more recent data.

