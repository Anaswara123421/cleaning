# Excel Conditional Formatting Demo

A small Excel workbook that shows how **Conditional Formatting** works, using a student marks sheet as the example. Cells change their look automatically (colours, icons, data bars) based on the values inside them.

## What's in this repo

| File | Description |
| --- | --- |
| `conditional_formatting.xlsx` | The workbook with the sample data and all formatting rules applied |
| `README.md` | This file |

## The data

The sheet (`Sheet1`) holds marks for 10 students in six subjects.

| Column | Contents |
| --- | --- |
| A | Student name |
| B to G | Marks in English, Maths, Social, Science, Hindi and Statistics |
| H | Grand Total |
| I | Date |

Students: Roy, Seeba, Sherin, Amal, Ajith, Aparna, Merlin, Gayathri, Susmitha, Roshan.

## Conditional formatting rules used

| # | Range | Rule type | What it does |
| --- | --- | --- | --- |
| 1 | `H2:H12` | Icon Set (3 Arrows) | Shows an arrow icon for each Grand Total: low, middle or high (split at the 33rd and 67th percentile) |
| 2 | `G3:G12` | Data Bars | Draws a gold bar in each Statistics cell. A longer bar means a higher mark |
| 3 | `B3:E12` | Duplicate Values | Highlights any repeated marks in English, Maths, Social and Science |
| 4 | `I1:I1048576` | Date Occurring: This Week | Highlights dates that fall in the current week |
| 5 | `I3` | Date Occurring: Tomorrow | Highlights the date if it is tomorrow |
| 6 | `H13` | Cell Value: Between 400 and 500 | Highlights the cell when its value is from 400 to 500 |

### Colour legend (cells F15 to F17)

The sheet includes a small legend describing the grand total ranges:

- `>450`
- `between 400 to 500`
- `<400`

## How to use

1. Download or clone this repository.
2. Open `conditional_formatting.xlsx` in Microsoft Excel (2010 or later recommended).
3. To view or edit the rules, go to **Home > Conditional Formatting > Manage Rules**, and set *Show formatting rules for* to **This Worksheet**.

To clear the rules, select the cells and choose **Home > Conditional Formatting > Clear Rules**.

## Try it yourself

- Change a mark in columns B to G and watch the Grand Total icon and the data bar update.
- Type the same mark in two cells within `B3:E12` to see the duplicate highlight.
- Change the dates in column I to today's date to see the "this week" and "tomorrow" rules react.

## What you'll learn

- Applying **Icon Sets**, **Data Bars** and **Highlight Cells** rules
- Using **date-based** rules (This Week, Tomorrow)
- Finding **duplicate values** quickly
- Managing and editing multiple rules on one sheet

## Notes

- Date rules depend on today's date, so highlights change as time passes. The sample dates are in late September 2026.
- Data bars and some icon features may look slightly different in LibreOffice or Google Sheets than in Excel.

## Contributing

Suggestions and improvements are welcome. Open an issue or submit a pull request.

## License

Free to use for learning and practice. Add a license of your choice (for example MIT) if you want to share it more widely.
