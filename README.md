# CDC Wonder Cause Of Death Processing

![Notebook Runs](https://github.com/andyreagan/cdc-wonder-cause-of-death-processing/actions/workflows/notebook-test.yml/badge.svg)

Read from [CDC Wonder](https://wonder.cdc.gov/controller/datarequest/D158) data 
downloaded to `cod113-gender-5yr.txt`.
All of the .txt data files are from CDC,
all of the parquet are made by us.
Make a couple charts to examine cause of the death
and relative cause of death by age.
From the "Underlying Cause of Death, 2018-2023, Single Race Request" page.
See [data documentation from CDC](https://wonder.cdc.gov/wonder/help/ucd.html#Top15).
As-of 2025-02-06,
the CDC notes that

> CDC’s website is being modified to comply with President Trump’s Executive Orders

but our extracts were made before these modifications.

Our script groups the cause of death into high level categories.
Then we writes out a dataset that has cancer/cvd/self-harm deaths 
by age and gender, 
along with the relative percentage of cancer as a cause of death.

View the main notebook on 
[NBViewer](https://nbviewer.org/github/andyreagan/cdc-wonder-cause-of-death-processing/blob/main/cod113.ipynb)
for the Altair graphics to show up.
