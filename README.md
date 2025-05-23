# Angular Trip Visualizer

An interactive Angular app to visualize trips between cities.  
Displays visual logic for continued, non-continued, and repeated trips using color, direction, and level indicators.

##  Features

- **First 3 letters** of Start and End points are used for display.
- **Trip types**:
  - **Continued Trip**: Straight line (→), Level 1 (e.g., Bangalore → Chennai, Chennai → Ooty).
  - **Non-Continued Trip**: Arrow (⬅️), Level 1 (e.g., Bangalore → Chennai, Ooty → Bangalore).
  - **Repeated Trip**: Same pickup & drop as previous — yellow card, Level 2 (e.g., Delhi → Mumbai, Delhi → Mumbai).
- Input validation — shows warning if either field is missing.
- Responsive layout with unlimited trips supported.
- Notes like “First Trip”, “Continued Trip”, etc., displayed alongside each trip.

##  Technologies Used

- Angular 15+
- TypeScript
- SCSS
- HTML5

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/YuvrajSingh05/Trip-Visualizer.git
   cd angular-trip-visualizer
   
Install dependencies:

bash
npm install
Run the app:

bash
ng serve

Navigate to http://localhost:4200 in your browser.

Usage
Enter Start Point and End Point — only the first 3 letters will be used.

Click Add Trip.

The trip will be evaluated and categorized as:

Level 1: Continued or Non-Continued

Level 2: Repeated

Visual feedback includes arrows, colors, and notes.

Example Scenarios

Input Order	Display	Level	Note
CHE → BAN	➝	1	First Trip
BAN → OTT	➝	1	Continued Trip
MUM → DEL	⬅️	1	Non-Continued Trip
DEL → MUM	➝ (Yellow)	2	Repeated Trip
