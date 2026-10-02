Tailwind CSS Grid — Classroom Practicals

This repository contains two practical examples I demonstrated in class at Tech Studio Academy to help my students understand CSS Grid using Tailwind CSS.
The demonstrations show how to create responsive grid layouts, change the number of columns at different screen sizes, and make individual boxes span multiple columns.

Technologies Used
- HTML5
- Tailwind CSS v4 through the browser CDN

PRACTICAL 1: RESPONSIVE GRID BOXES
This example contains six coloured boxes inside a white container on a light-green background. It demonstrates responsive columns, consistent box heights, spacing, and hover effects.
----------------------------------------
Screen width	  | Columns	 |   Rows  |
----------------------------------------
Below 640px	      |     1	 |   6     |
640px–1023px	  |     2	 |   3     |
1024px and above. |     3	 |   2     |
----------------------------------------

The grid layout uses:
class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4"
- grid creates a grid container.
- grid-cols-1 gives the grid one column by default.
- sm:grid-cols-2 changes it to two columns from 640px.
- lg:grid-cols-3 changes it to three columns from 1024px.
- gap-4 adds spacing between the boxes.

Each box uses h-48 to maintain the same height at every screen size. Different background colours and hover utilities provide visual feedback.


PRACTICAL 2: COLUMN SPAN
This example contains four boxes and demonstrates how a grid item can occupy more than one column using sm:col-span-2.
---------------------------------------------------------------------------------
Screen width	  |                Layout                                       |
---------------------------------------------------------------------------------
Below 640px	      | One column, with all four boxes stacked vertically          |
640px–1023px	  |  Two columns; Box One and Box Four each span both columns   |
1024px and above  |	Three columns; Box One and Box Four each span two columns   |
---------------------------------------------------------------------------------

At large screen sizes, the arrangement is:
----------------------------------------------------------------------------------------
Row	    Column 1	              |       Column 2	             |   Column 3          |
----------------------------------------------------------------------------------------
1	    Box One spans columns 1–2 |	Box One continued	         |  Box Two            |
2	    Box Three	              | Box Four spans columns 2–3	 |  Box Four continued |
----------------------------------------------------------------------------------------

The column-span utility is applied to Box One and Box Four:
class="sm:col-span-2"

It takes effect from the small breakpoint and continues to apply at larger screen sizes. The example also demonstrates responsive box heights, padding, and container background colours.


CONCEPTS COVERED
- Mobile-first responsive design
- Grid containers and column counts
- Column spanning
- Spacing between grid items
- Width and maximum-width utilities
- Fixed and responsive heights
- Responsive padding and background colours
- Flexbox for centring the grid container on the page
- Rounded corners, shadows, and hover effects
- Semantic HTML using section and article in the first practical


How to View the Examples
1. Clone or download this repository.
2. Open the project folder in Visual Studio Code.
3. Open either example's HTML file in your browser, or right-click the file and select Open with Live Server if the extension is installed.
4. Resize the browser window to observe the different layouts.
An internet connection is required to load Tailwind CSS through the browser CDN. No npm installation or build step is needed for these classroom examples.


Practice for Students
- Change the gap between the boxes.
- Adjust the box heights at different breakpoints.
- Try making another box span two columns and observe the placement.
- Add a four-column layout at the xl: breakpoint.
- Experiment with colours, shadows, and hover effects.


**Instructor** **Bukola Ruth Olafenwa**
**Full Stack Web Development Instructor — Tech Studio Academy**
