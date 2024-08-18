## Getting Started

Welcome to the VS Code Java world. Here is a guideline to help you get started to write Java code in Visual Studio Code.

## Folder Structure

The workspace contains two folders by default, where:

- `src`: the folder to maintain sources
- `lib`: the folder to maintain dependencies

Meanwhile, the compiled output files will be generated in the `bin` folder by default.

> If you want to customize the folder structure, open `.vscode/settings.json` and update the related settings there.

## Dependency Management

The `JAVA PROJECTS` view allows you to manage your dependencies. More details can be found [here](https://github.com/microsoft/vscode-java-dependency#manage-dependencies).

## Running the file & Considerations
Environment: Run the code on windows visual studio code.

Criteria to consider
1. Use either boolean or special characters like '*' to identify the tile in the grid that contains a mine.
2. Have a method that would display the values in the grid, after selecting a tile that is covered. If tile is revealed, print the char of the grid followed by " ". Else print "_" followed by " ".
3. Randomly place the mine in the game and check if that tile already contains a mine, if it does contain a mine, random again. Randomly put tiles in the grid until it matches the value specified by the user.
4. During the reveal phase, check if the tile is not outside the boundary of the grid. Count the mines present in the adjacent tiles, in all 8 directions, ensuring that the tile is still within the grid and that the grid contains a mine
5. If adjacent mines > 0; print the char of the mine count of that tile, detected for adjacent square. If the tile selected returns mine count of 0, run the reveal method again to simulate the same action of selecting an adjacent tile 
beside the tile revealed to be 0
6. Recursively run the program until either the mine has exploded or the game is won by the player.
