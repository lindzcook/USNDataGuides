# USN&WR Graphics Style Guide

This style guide comprises the typographic and technical best practices used for the USN&WR newsroom.

Using rules consistently make your job easier and prevent readers from having to struggle with new interfaces on every project, but remember that overdependence on rules can hamper progress, and that "a foolish consistency is the hobgoblin of little minds." 

Finally, This is a living document. Please feel free to propose changes.

## Asterisks

Use asterisks only when it is necessary to communicate a difference in a few data points versus the whole graphic. For example, a map where the lat and long needed to be approximated on three points. 

For more data explanation, avoid asterisks and use lead-in text or methodology.

## Axes

Make clear what data you are showing by labeling.

Avoid repetition in the headline, axes labels and legends.

## Bylines

Bylines are important measures of credit and responsibility. Just as every story has a byline, every graphic should have a byline.

Bylines are in this format: "NAME for USN&WR"

If the chart is an image, bylines should appear on the actual image and on the credit line in the CMS, not simply below the image. For HTML embeds, bylines should be included in the HTML enhancement. Add the following HTML to the end of your enhancement: `<p>NAME for USN&WR</p>`. 

By adding credit in this manner, we ensure bylines remain with the content if it is reused.

## Charts

For guidance on which charts and tools to use, refer to the "Which Chart" guide.

## Colors

Red-Green is the most common form of color blindness. Beware of using these colors to communicate data. To check if differences between colors can be perceived by colorblind users, check [Color Oracle](http://colororacle.org/) or [Spectrum.](https://chrome.google.com/webstore/detail/spectrum/ofclemegkcmilinpcimpjkfhjfgmhieb?hl=en)

When showing differences in rate of a single variable, stick to a single hue and vary value/lightness. For example, don't fade from blue to pink. The one exception is fading from red to green to show "bad" to "good" (and remember to check your reds and greens for color blindness accessibility). 

Beware of using numerical cut-offs for gradient-like colors, see [here](http://junkcharts.typepad.com/junk_charts/2014/08/people-are-happier-in-some-parts-of-the-country-as-labor-day-nears.html).

When using color to show category, use different colors instead of shades on maps.

Using shades of the same color for bar graphs can be less distracting for the reader than using high contrast colors. 

## Color Breaks

Pick color breaks carefully. Your data may not be best represented with equal-interval breaks. See what patterns emerge using a variety of algorithms, such as quantiles, [Jenks natural breaks](http://en.wikipedia.org/wiki/Jenks_natural_breaks_optimization), [head/tail breaks](https://sites.google.com/site/thepowerofcartography/head-tail-breaks), standard deviation, or even arbitrary breaks that might make sense for your data. For example, if your data is average commute time to work, breaks of 10, 20, 30, 45 and 60+ minutes might make the most sense for readers, even if your data is not distributed normally among those breaks.

Make sure your color breaks don't mislead readers about the distribution of your data. For instance, if your values are mostly clustered between 1 and 10 but includes a few items above 1,000, make sure that the color that represents 1,000 is more than just one shade different than the color that represents 10. The Daily Beast uses a tool they made called [Histagram.me](http://www.histagram.me/) to examine the distribution of datasets.

If the pattern you see in your data only appears under a custom color break scale, rethink whether the pattern is actually in the data.

For color breaks in numerical data, see [above](#colors).

## Corrections

Graphics follow the newsroom's standard corrections policy.

## Dashes

Stick with our policy for dashes in data descriptions.

## Data: Singular or Plural?

The word "data" is always plural. See USN stylebook entry: 

> "data - always plural From AP: Data is a plural noun, it normally takes plural verbs and pronouns. AP's collective nouns entry includes examples of when data may take singular verbs and pronouns, but to avoid confusion and keep with USN standard practice, we stick with plural."

## Footnotes

Don't use footnotes. For information necessary for [transparency,](#transparency) but not for understanding of the graphic, use [methodology.](#methodology) 

For information necessary for understanding the graphic, see [lead-in](#lead-in), [asterisks](#asterisks), [hovers](#hovers).

## Geocoding

Geocoding is the process of matching address to latitude and longitude points. Use the geocoding guide for this, if you are geocoding large sets of data. 

For small sets, you can use [Google Maps.](https://www.google.com/maps/preview) The latitude and longitude are in the URL when you look up a point. 

Always check geocoded data to make sure it isn't 1. in an ocean, 2. in China, 3. in the wrong state. 

## Headlines

Graphics should have a title. All text on graphics should follow USN headline style.

Avoid repetition in axes labels, legends and the title.

## Hovers

In general, use hovers to communicate information not evident by glancing at the graph. For example, a line graph of the U.S. joblessness rate doesn't need hovers to communicate the rate and the year. That's what the graph is for. 

Practically though, some free tools we use require hovers, making it unavoidable. In those cases, convert numbers to understandable formats using rounding and labels (is this a dollar amount or a percent, for example). 

For maps, include the state name on hovers. People forget where all the states are. In general, avoid the default hover options and convert hovers to sentence form. 

##  Labels (Axes)

See [axes](#axes).

##  Labels (Data)

See [legends](#legends).

## Lead-in

Put explanatory copy in the article/blog post before the graphic. It should be very short -- aim for no more than four or five lines. Avoid re-telling a whole news story, but do make sure you accomplish three things:

1. Give the reader enough background to be able to understand the purpose of the app or graphic.
2. Let the reader know how to start using any interactivity.
3. Link to and briefly describe the related story, if any.

## Legends

Always include the information needed to understand the chart with the chart. That means transparency about what the data is, where it came from and its timeframe. 

In charts with only one element, include needed information on the axis or in the title. In charts with more than one element, use labels (by the lines or bars) or a legend, depending on which is more clear, but never both. For a line chart, use a legend when space is tight and the lines intersect at many points, making it unclear from a label. Otherwise, use labels.

A legend must be visible on the reader's computer screen when the chart is visible. Legends should be in the same sequence as the charts they describe.

Avoid repetition in axes labels, legends and titles.

## Maps

Maps are best when showing data in which geography is an important variable. [Read "When Maps Shouldn't Be Maps" before making any maps](http://www.ericson.net/content/2011/10/when-maps-shouldnt-be-maps/).

All maps must be distinguishable from population maps. To accomplish this, the underlying data should control for population or other denominator. If you make a U.S. state choropleth map and the darkest states are New York, Texas and California, re-read this paragraph.

Avoid bubble maps, which represent the rate of a phenomenon at different locations using differently sized circles. This is for two reasons: First, people cannot accurately perceive differences in the area of circles. Second, bubble maps appear to show the geographic bounds of a phenomenon and not the rate of that phenomenon at the geographic center of the circle. This is another way of saying that they look too much like nuclear blast radius maps.

## Mean Versus Median

The mean is the average of the data. The median if the middle value in a distribution of the data. 

In general, use median if extreme outliers are present (like income level) and use mean otherwise. 

## Methodology 

Document any methodology and present it to readers clearly. Post a link to it prominently in the app or graphic. The methodology (or "nerd box") should detail the steps you took to clean the data and the exact analysis you ran on the data.

## Money

Use the appropriate currency symbols when showing currency. Avoid showing fractional currency like cents. In most cases, currency for multiple years should be adjusted to current year.

If you are comparing currency (such as costs, revenues, etc.) across multiple years, you should adjust for inflation. Don't ever refer to an amount of money being a "record" based on historical data that is not adjusted for inflation.

Always explain to readers whether and how you've adjusted currency figures. 

If you are using data from another source, always understand and make clear to readers if the data has been adjusted for inflation and what year's currency the data has been adjusted for.

## Numbers

The primary function of numbers in a graphic is to help readers understand scale and order of magnitude, and compare against other numbers. Think of them more like words than like minutely precise coordinates (unless of course your numbers are literally coordinates).

Apply the following rules to numbers wherever they appear in graphics:

Except where special precision is required, round numbers and use whole numbers. Don't portray precision that doesn't really exist. This can be accomplished in Excel using the [ROUND function.](http://office.microsoft.com/en-us/excel-help/round-a-number-HP003056144.aspx) Always round as your last step.

When displaying numbers in a table, make them either right-aligned or decimal-aligned.

Except where special precision is required, abbreviate any number over 10,000 by truncating each number after the highest thousands place and appending a word or abbreviation indicating order of magnitude. Use one significant digit after the decimal point. For example:

    10,302,321 -> 10.3 million or 10.3M
    5,242,000,014 -> 5.2 billion or 5.2B
    901,212 -> 901.2 thousand or 901.2K or 0.9M

For numbers with more than three digits, always separate each thousands place with a comma.

Use AP style when using numbers in copy. That is, spell out numbers under 10 except in the following circumstances:

> Use figures for ages, sums of money, time of day, percentages, house numerals, years, days of the month, degrees of temperature, proportions, votes, scores, speeds, time of races, dimensions and serial numbers. ([via](https://websso.wwu.edu/down/index.shtml))

"Not available" and "not applicable" are abbreviated like this: N/A

##Percent Change/ Percentage Change

Percent change expresses the change in values as a percentage change from the original value. 

Wrong:

In the USN newsroom, 50 percent of reporters liked math in 2010 and 60 percent of reporters liked math in 2012. This is a 10 percent increase in people who like math. 

Right: 

In the USN newsroom, 12 reporters liked math in 2010 and 16 reporters liked math in 2012. This is a 33 percent increase in math lovers. 

To calculate percentage change, use the formula: 

`(New number - old number)/ old number * 100`

Or use this handy [calculator.](http://www.skillsyouneed.com/num/percent-change.html)

##  Reuse

When a reporter or producer uses a graphic that has already been created, they need to verify that the data is the most recent available. 

Check the Google Doc for our data dictionary. A list of available graphics is on sheet two. Each graphic includes the date when it needs to be updated. Contact the creator to make sure.

If a graphic you created has staying power, add it to the sheet so that it can be reused.

## Rounding

See [numbers](#numbers).

## States

Always seek to add clarity. 

In general, use USN headline style for all text on a graph, meaning the state abbreviation, separated by periods. For hovers, use the state's full name in sentence form. 

## Sources

Under every display of data, whether it's a map, chart, table or something else, show your data's sources. Our style is to combine the source with the credit line. For example, "Lindsey Cook for USN&WR, Source: FBI"

Link to the source or the best version of the source data whenever possible. If the data went through another party for cleaning or analysis, mention both in the source line. For example, "Source: FCC, Sunlight Foundation" for FCC comments data cleaned by the Sunlight Foundation.

## Title 

See [headline](#headline).

## Total

Only use "total" as an adjective when it's not clear what you're totaling. Never use the redundant "total amount" -- just use "total."

##  Transparency

We communicate how we obtain information for our stories, and we must do the same for our data. Be transparent about how the numbers were calculated and why they were calculated in that way. See [methodology](#methodology). 

## Updates

Unlike an article, which tends to be a frozen description of a moment in time, graphics tend to be durable resources, and may need to be updated from time to time as new data becomes available.

When updating an app with new data, don't append a note explaining every change, as that note would be quite lengthy and very boring. Simply update the date in the byline to indicate when the data was last updated. If an app updates dynamically, the date in the byline should change dynamically as well.

Don't show both the original publication date and the most recent updated date in the byline. Your readers don't relish the archival history of our work quite like you might. Simply show the date of the latest update (after the word "updated," of course).

When the decision is reached to stop updating an app, put a prominent note on every page of the app that says when the app stopped being updated, and if possible, where to find more recent data.

See [reuse](#reuse). 

