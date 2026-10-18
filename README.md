# tower-of-hanoi-visualizer
# Tower of Hanoi Repository README Markdown
## Interactive Tower of Hanoi Visualizer
An interactive, web-based algorithmic visualizer that demonstrates the step-by-step execution of the classic Tower of Hanoi recursive algorithm. Built entirely with vanilla HTML5, CSS3, and JavaScript, this project highlights clean UI/UX state machines and algorithmic event tracing.
## Features

* Dynamic Disk Control: Scale the problem difficulty in real-time by adjusting the simulation between 3 and 8 disks.
* Playback Telemetry: Play, pause, or manually step backward and forward through the execution call stack.
* Live State Tracing: View a synchronized logging terminal detailing every data node displacement.
* Adjustable Delays: Fine-tune animation speeds from 100ms to 2000ms on the fly.
* Adaptive UI: Fully responsive layouts optimized for varying screen footprints.

## Algorithmic Architecture
The core solver uses a classic divide-and-conquer recursive mechanism. For any given number of disks $n$, the system models state transitions across three pegs (A, B, and C) using the mathematical formulation:

   1. Sub-problem 1: Move $n-1$ disks from the source peg to the auxiliary peg.
   2. Base Move: Move the single remaining largest disk from the source peg to the target peg.
   3. Sub-problem 2: Move the $n-1$ disks from the auxiliary peg to the target peg.

## Complexity Breakdown

* Time Complexity: $O(2^n)$ — The exact number of sequential moves required is governed by the relation $T(n) = 2^n - 1$. For the default configuration of 5 disks, this triggers exactly 31 operations.
* Space Complexity: $O(n)$ — Memory overhead scales linearly with the maximum depth of the recursive execution call stack.

## Installation & Local Execution
Since this is a lightweight, zero-dependency client-side application, no installation or compilation pipelines are required.

   1. Clone the repository:
   
   git clone https://github.com/YelluMadhukar/tower-of-hanoi-visualizer.git
   
   2. Navigate into the directory:
   
   cd tower-of-hanoi-visualizer
   
   3. Launch the application:
   Open index.html directly in any modern web browser (Chrome, Firefox, Safari, Edge).

## License
This project is open-source and available under the MIT License.

