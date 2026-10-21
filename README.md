# 🎓 StudentHub – Student Dashboard

**Created by O.Divyareddy**

🔗 **Live demo:** https://divyareddy0734-ops.github.io/student-/
A responsive student dashboard for a B.Tech CSE (AI & ML) student. It shows courses, assignments, attendance, a weekly timetable, results and the student profile on one page. It is built with plain HTML, CSS and JavaScript, so there is nothing to install.

## Features

- **Dashboard overview:** a welcome banner and summary cards for enrolled courses, attendance, pending assignments and grade.
- **My Courses:** subject cards with progress bars.
- **Upcoming Tasks:** the next deadlines, with a "View All Tasks" button.
- **Assignments:** tick an assignment to move it from Pending to Completed. Untick it to move it back. The pending count on the dashboard updates automatically.
- **Weekly Timetable:**
  - Mon–Fri grid with 7 periods a day, a short break and lunch.
  - Colour-coded class types: theory, lab (3 periods), project work, placement training, mentor hour and self study.
  - Today's column is highlighted, the current class is outlined, and a "Next class" box is shown.
  - Weekly summary of theory, lab, project and placement periods.
  - Click any class to edit its name, room, faculty and type. Changes are saved in the browser (`localStorage`), and a Reset button restores the sample week.
- **Internal assessments:** a table with each subject's faculty, next assessment, date and internal marks.
- **Attendance by Subject:** attendance bars for each subject, with the 75% minimum shown.
- **My Profile:** department, university, roll number, CGPA, education and contact.
- **Responsive design:** works on desktop, tablet and mobile.

## Tech stack

| Part | Used |
| --- | --- |
| Structure | HTML5 |
| Styling | CSS3 (grid, flexbox, animations) |
| Logic | Vanilla JavaScript |
| Font | Poppins (Google Fonts) |

## Project structure

```
studenthub/
├── index.html    # the whole dashboard (HTML, CSS and JS in one file)
└── README.md
```

## How to run

1. Download or clone the project.
2. Rename `student-dashboard-btech.html` to `index.html` if you like.
3. Open `index.html` in any modern browser (Chrome, Edge, Firefox or Safari).

That's all. It works offline too, apart from the Poppins font, which falls back to the system font.

### Host it online (optional)

Upload `index.html` to a repository and turn on **GitHub Pages** (Settings → Pages), or drag the file into Netlify Drop.

## Customising

| To change | Where to look in `index.html` |
| --- | --- |
| Name, roll number, CGPA, email | The `My Profile` section (`id="profile"`) and the welcome banner |
| Courses and progress | The `My Courses` panel |
| Attendance percentages | The `Attendance by Subject` section (`id="attendance"`) |
| Assignments | The `assignments` array in the script |
| Timetable | The `defaults` object in the timetable script, or click a class on the page |
| Internal assessments | The `rows` array in the timetable script |
| Colours | The CSS at the top of the file |

## Notes

- The timetable, faculty names, rooms, marks and attendance numbers are sample data. Replace them with your own.
- Timetable edits are stored only in your own browser. Clearing browser data resets them.

## Author

**O.Divyareddy**
B.Tech CSE (AI & ML), Mohan Babu University (2023 – 2027)
