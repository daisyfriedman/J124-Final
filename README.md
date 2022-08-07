# J124-Final

## Questions

### 1. Are the total benefits proportional to the total cost over time?

##### To test whether the benefits are proportional to the total cost, I wanted to create a ratio for easier comparison over time.

<img width="723" alt="Screen Shot 2022-08-04 at 9 16 44 AM" src="https://user-images.githubusercontent.com/109619721/183160903-268846d9-20b6-443c-b222-dc3da3e2cb4d.png">

##### This was a simple equation (seen above). The resulting column did shows how much of the total money spent goes into benefits (see highlighted column in image below). 

<img width="1139" alt="Screen Shot 2022-08-05 at 1 58 54 PM" src="https://user-images.githubusercontent.com/109619721/183166356-fdcaf2b6-f56c-4392-817c-fab462ebd3ac.png">

##### Because the numbers remain relatively constant (within hundreths of a decimal), I concluded that the benefits remained relatively proportional to the total cost.

### 2. Are the average benefits per person proportional to inflation prices (does the purchasing power remain constant)?

##### In order to compare the benefits to purchasing power, I had to download a dataset that shows these changes since the 1960s. I chose the Consumer Price Index because it best shows changes to prices relative to inflation.

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

<img width="878" alt="Screen Shot 2022-08-04 at 10 18 47 AM" src="https://user-images.githubusercontent.com/109619721/183217526-66adb0ba-e592-4cc1-b34f-6b657f66186d.png">
https://datawrapper.dwcdn.net/WVTIA/1/

### 3. Were benefits affected by changes in the market (aka recessions)?

The process with which I completed this question is very similar to that of the previous one -- question 2. First, I found a dataset of changes to the USA's GDP since the 1960s. I chose GDP changes rather than a more linear chart of the GDP over time because the prior source has more easily-identifiable recession periods.

<img width="1440" alt="Screen Shot 2022-08-04 at 9 06 55 AM" src="https://user-images.githubusercontent.com/109619721/183310322-995d61cc-fbce-4324-ac71-db9563b72d88.png">

After downloading the data as a CSV, I imported it into my google sheet and copied, pasted and transposed it until it was in a simpler format (see analysis for question 2 for step-by-step process).

<img width="1440" alt="Screen Shot 2022-08-02 at 3 49 27 PM" src="https://user-images.githubusercontent.com/109619721/183310508-fb79248e-b0eb-4cbb-ab25-bbdd8e95900b.png">

From there, I used a VLOOKUP equation to match this data with the larger SNAP dataset.

<img width="279" alt="Screen Shot 2022-08-04 at 9 13 23 AM" src="https://user-images.githubusercontent.com/109619721/183310309-06a5f924-8593-474e-8a50-23a54c56e637.png">

From there, I felt the best way to comprehend any correlation between recession and benefits was to use a data visualization. I used Datawrapper to create a line chart with shaded columns to represent recession years. Other than just dips in the GDP changes, I used a list of recessions from CNBC to confirm the years.

<img width="1329" alt="Screen Shot 2022-08-07 at 1 44 17 PM" src="https://user-images.githubusercontent.com/109619721/183310346-f475a610-e0cc-4896-b202-b6a0c9d22c49.png">

<img width="838" alt="Screen Shot 2022-08-05 at 1 40 34 PM" src="https://user-images.githubusercontent.com/109619721/183310264-e425d7b5-3925-4621-a2c1-1ec9c746b1c3.png">
https://datawrapper.dwcdn.net/WOm5a/1/

From analyzing this chart, I concluded that there was little to no effect of the GDP on SNAP benefits in general, except for the Great Recession (2007 t0 2009), during which there was a sharp increase of the average benefit per person.
