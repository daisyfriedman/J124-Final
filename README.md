# J124-Final

## Questions

### 1. Are the total benefits proportional to the total cost over time?

To test whether the benefits are proportional to the total cost, I wanted to create a ratio for easier comparison over time.

<img width="723" alt="Screen Shot 2022-08-04 at 9 16 44 AM" src="https://user-images.githubusercontent.com/109619721/183160903-268846d9-20b6-443c-b222-dc3da3e2cb4d.png">

This was a simple equation (seen above). The resulting column did shows how much of the total money spent goes into benefits (see highlighted column in image below). 

<img width="1139" alt="Screen Shot 2022-08-05 at 1 58 54 PM" src="https://user-images.githubusercontent.com/109619721/183166356-fdcaf2b6-f56c-4392-817c-fab462ebd3ac.png">

Because the numbers remain relatively constant (within hundreths of a decimal), I concluded that the benefits remained relatively proportional to the total cost.

### 2. Are the average benefits per person proportional to inflation prices (does the purchasing power remain constant)?

In order to compare the benefits to purchasing power, I had to download a dataset that shows these changes since the 1960s. I chose the Consumer Price Index because it best shows changes to prices relative to inflation.

<img width="1373" alt="Screen Shot 2022-08-04 at 9 18 35 AM" src="https://user-images.githubusercontent.com/109619721/183213295-0e7e0d48-e670-4fce-8a68-493aac3745e1.png">

After importing the data, I sorted it to only show statistics for the United States by using the filter option.

<img width="1440" alt="Screen Shot 2022-08-04 at 10 43 45 AM" src="https://user-images.githubusercontent.com/109619721/183215316-bb2630e4-57ef-4c5b-b9d3-4167037a883d.png">

After sorting the data, I copy and pasted the filtered values into another sheet.

<img width="947" alt="Screen Shot 2022-08-04 at 10 49 45 AM" src="https://user-images.githubusercontent.com/109619721/183215897-c1e3c718-f14d-4904-aa75-5f281a3d2011.png">

Then I used the 'transposed' option to paste the values with the years listed as columns.

<img width="1440" alt="Screen Shot 2022-08-04 at 10 44 42 AM" src="https://user-images.githubusercontent.com/109619721/183216134-cffe5aac-ce7a-4a8e-a4a2-41a05f38b827.png">

To combine this new dataset with the larger SNAP sheet, I used the VLOOKUP equation.

<img width="279" alt="Screen Shot 2022-08-04 at 9 13 23 AM" src="https://user-images.githubusercontent.com/109619721/183216762-ad7710d1-63ed-499d-8cdc-4bad26cd4270.png">

The data by itself was difficult to interpret, so the best way to compare the benefits to the purchasing price was a visual representation. I inputted the data of average benefit per person to the CPI on a line graph.

[<img width="878" alt="Screen Shot 2022-08-04 at 10 18 47 AM" src="https://user-images.githubusercontent.com/109619721/183217526-66adb0ba-e592-4cc1-b34f-6b657f66186d.png">](https://datawrapper.dwcdn.net/WVTIA/1/)

### 3. Were benefits affected by changes in the market (aka recessions)?

The process with which I completed this question is very similar to that of the previous one -- question 2. First, I found a dataset of changes to the USA's GDP since the 1960s. I chose GDP changes rather than a more linear chart of the GDP over time because the prior source has more easily-identifiable recession periods.

<img width="1440" alt="Screen Shot 2022-08-04 at 9 06 55 AM" src="https://user-images.githubusercontent.com/109619721/183310322-995d61cc-fbce-4324-ac71-db9563b72d88.png">

After downloading the data as a CSV, I imported it into my google sheet and copied, pasted and transposed it until it was in a simpler format (see analysis for question 2 for step-by-step process).

<img width="1440" alt="Screen Shot 2022-08-02 at 3 49 27 PM" src="https://user-images.githubusercontent.com/109619721/183310508-fb79248e-b0eb-4cbb-ab25-bbdd8e95900b.png">

From there, I used a VLOOKUP equation to match this data with the larger SNAP dataset.

<img width="279" alt="Screen Shot 2022-08-04 at 9 13 23 AM" src="https://user-images.githubusercontent.com/109619721/183310309-06a5f924-8593-474e-8a50-23a54c56e637.png">

From there, I felt the best way to comprehend any correlation between recession and benefits was to use a data visualization. I used Datawrapper to create a line chart with shaded columns to represent recession years. Other than just dips in the GDP changes, I used a list of recessions from CNBC to confirm the years.

<img width="1329" alt="Screen Shot 2022-08-07 at 1 44 17 PM" src="https://user-images.githubusercontent.com/109619721/183310346-f475a610-e0cc-4896-b202-b6a0c9d22c49.png">

[<img width="838" alt="Screen Shot 2022-08-05 at 1 40 34 PM" src="https://user-images.githubusercontent.com/109619721/183310264-e425d7b5-3925-4621-a2c1-1ec9c746b1c3.png">](https://datawrapper.dwcdn.net/WOm5a/1/)

From analyzing this chart, I concluded that there was little to no effect of the GDP on SNAP benefits in general, except for the Great Recession (2007 t0 2009), during which there was a sharp increase of the average benefit per person.

### 4. Which decade had the most SNAP participants (of the decades provided)?

First, I had to organize the data by decade. There are several ways to do this, so this is just one method.

I used the ROUNDDOWN to round down the years to the most recent decade.

<img width="220" alt="Screen Shot 2022-08-07 at 10 38 12 PM" src="https://user-images.githubusercontent.com/109619721/183349106-de9f395b-43af-4343-9174-34e00ff44d26.png">

The above funtion's syntax is ROUNDDOWN(value, places). Here is the breakdown for this example:
ROUNDDOWN(A4*0.1,0)*10
  * A is the column with contains the years. We are on row 4 in this example.
  * Multiplying the value by 0.1 turns the format from thousands to hundreds.
    * Ex: 1969 becomes 196.9
  * Having a 0 in  'places' rounds down the value to the whole number.
    * EX: 196.9 becomes 196
  * Multiplying the whole equation by 10 returns the numbers to four digits -- their decade.
    * Ex: 196 becomes 1960

From there, I made a pivot table to analyze the data.

<img width="322" alt="Screen Shot 2022-08-07 at 10 46 07 PM" src="https://user-images.githubusercontent.com/109619721/183351370-7fdf4a5f-873c-4ccb-b14c-6c119a8352cc.png">

I then formatted the pivot table to show the participation by decade.

<img width="460" alt="Screen Shot 2022-08-07 at 10 49 34 PM" src="https://user-images.githubusercontent.com/109619721/183351656-735a999c-b1fd-4c6d-abc2-10d13d63b34e.png">

Because the 1960s only have one year (1969), I filtered this decade out to only have the fully complete decades shown.

<img width="323" alt="Screen Shot 2022-08-07 at 10 42 46 PM" src="https://user-images.githubusercontent.com/109619721/183351920-d4c0451a-1b6d-41cf-acfc-860670465b58.png">

From there, I was able to analyze the data and conclude that the total participants grew every decade, making the 2010s the decade with the highest number of participants.

<img width="306" alt="Screen Shot 2022-08-07 at 10 49 43 PM" src="https://user-images.githubusercontent.com/109619721/183352206-74b2eddc-f5d7-4b6c-835e-69b966538436.png">

### 5. Which year had the highest total benefits? Highest other costs?

This is a relatively simple process. For this question, I simply sorted the total benefit column by descending value and scrolled over to the top year. Then I did the same for other costs.

<img width="462" alt="Screen Shot 2022-08-07 at 11 30 56 PM" src="https://user-images.githubusercontent.com/109619721/183354520-43043b81-9817-4a50-ba53-97d36ca10d4f.png">

I found that 2013 had the most total benefits but did not, in fact, have the highest cost for other variables. Instead, 2019 had the highest costs other than benefits.

<img width="593" alt="Screen Shot 2022-08-07 at 11 35 35 PM" src="https://user-images.githubusercontent.com/109619721/183354569-8acb77e5-e14b-4dd3-9da7-d2971d2c69da.png">

<img width="745" alt="Screen Shot 2022-08-07 at 11 35 17 PM" src="https://user-images.githubusercontent.com/109619721/183354584-14097d9a-7974-4729-93f2-bdfef63b45bd.png">

