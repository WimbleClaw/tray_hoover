# Hoover

Navigates a imaginary robotic hoover (much like a Roomba) through an equally imaginary room.

## Meeting Requirements

- Placing the hoover on a patch of dirt ("hoovering") removes the patch of dirt so that patch is then clean for the remainder of the program run.
- Driving into a wall has no effect (the robot skids in place).
- Takes the room dimensions, the locations of the dirt patches, the hoover location and the driving instructions as input and to then output the final hoover position (X, Y) and the number of patches of dirt the robot cleaned up.
- The program runs in the command line
- Is written in JS
- The bottom left corner is the point of origin for our coordinate system, so as the room contains all coordinates its bottom left corner is defined by X: 0 and Y: 0.

## Getting Started

To run the program type

```
node index.js
```

## Input

To update the input, you will have to update the input.txt file and change the test code accordingly. As the bottom left corner is defined by X: 0 and Y: 0 all the coordinates must be less than the grid size.

Example input:

```
5 5
1 2
1 0
2 2
2 3
NNESEESWNWW
```

- the first line holds the room dimensions (X Y), separated by a single space (all coordinates will be presented in this format)
- the second line holds the hoover position
- subsequent lines contain the zero or more positions of patches of dirt (one per line)
- the next line then always contains the driving instructions (at least one)

## Running the tests

First run

```
$ npm install
```

then

```
$ npm test
```

If all tests haven't run enter

```
a
```

## Layout

The code is split into separate files for separation of concerns. As classes would not have added to the program I have not used a class based system.

## Built With

- [Node.js](https://nodejs.org/en/) - JavaScript runtime for building fast network applications.
- [Jest](https://jestjs.io/) - Frontend testing library

## Author

**Aisha D'Souza**
