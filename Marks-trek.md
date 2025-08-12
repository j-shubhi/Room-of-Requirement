# Marks Tracker

**Google Sheet:** [Open Marks Tracker Sheet](https://docs.google.com/spreadsheets/d/17A50Qm1LKryI9OanMO0Htojxf1xi2TAlH6yrtdu2z-g/edit?usp=sharing)

> Template based on Google Sheet layout (6 courses, columns: MO, MM, Actual Contribution, Weightage)

## How to use

- **MM** = Maximum Marks
- **MO** = Marks Obtained
- **Actual Contribution** = usually percentage score for that assessment
- **Weightage** = percent contribution of assessment to course total
- **Weighted Score** = `Actual Contribution × (Weightage / 100)`

---

## Per-Course Template

**Course:** COURSE NAME  
**Total Weightage (check):** `=SUM(E3:E100)` — should equal `100`

| Assessment | MM | MO | Actual Contribution (%) | Weightage (%) | Weighted Score (%) |
|------------|---:|---:|------------------------:|--------------:|-------------------:|
| Assessment 1 |  |  | `=IF(B4=0,0,C4/B4*100)` |  | `=D4*(E4/100)` |
| Assessment 2 |  |  | `=IF(B5=0,0,C5/B5*100)` |  | `=D5*(E5/100)` |
| Assessment 3 |  |  | `=IF(B6=0,0,C6/B6*100)` |  | `=D6*(E6/100)` |
| ...          |  |  |                         |  |               |
| **Course Total (%)** |  |  |  | **=SUM(E4:E100)** | **=SUM(F4:F100)** |

---

## Example for Course 1

| Assessment | MM  | MO  | Actual Contribution (%)         | Weightage (%) | Weighted Score (%) |
|------------|----:|----:|--------------------------------:|--------------:|-------------------:|
| Quiz 1     | 20  | 18  | `=IF(B4=0,0,C4/B4*100)`          | 10            | `=D4*(E4/100)`     |
| Mid        | 100 | 72  | `=IF(B5=0,0,C5/B5*100)`          | 40            | `=D5*(E5/100)`     |
| Assign     | 30  | 28  | `=IF(B6=0,0,C6/B6*100)`          | 20            | `=D6*(E6/100)`     |
| Final      | 100 | 65  | `=IF(B7=0,0,C7/B7*100)`          | 30            | `=D7*(E7/100)`     |
| **Total**  |     |     |                                 | **=SUM(E4:E7)** | **=SUM(F4:F7)**   |

---

## Overall Summary (All Courses)

| Course | Course Total (%) |
|--------|-----------------:|
| Course 1 |                 |
| Course 2 |                 |
| Course 3 |                 |
| Course 4 |                 |
| Course 5 |                 |
| Course 6 |                 |
| **Overall % (avg)** | `=AVERAGE(B2:B7)` |


