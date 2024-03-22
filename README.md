# Darwin World Project

### Main Part Structure of the Project
In the directory src/main/java/agh/dg, you can find the main project files.
We distinguish among them:
- the *DarwinWorldApp* class, which prepares the application for display.
- the *ExtendedThread* class, which contains the implementation of extending the Thread class, used in thread management for pausing and closing the simulation.
- the *Main* class, which launches the program.
- the *Simulation* class, which contains the implementation of the animal world simulation.
- the *Statistics* class, which stores statistical data displayed in the simulation.

Additionally, there are packages:
*enums*, which contains enumerations used in the application
- the *GameCommunicat* class contains messages used when displaying statistics.
- the *MoveDirection* class contains possible movement directions for animals.

*exceptions*, which contains custom exception classes used
- the *InvalidGameParamsException* class contains the implementation of an exception for providing invalid game parameters.

*helpers*, which contains helper classes for file handling and data conversion
- the *CsvFileHandler* class contains support for saving data to a .csv file.
- the *GameStatic* class contains conversion of an animal to color and statistical data to String.

*models*, which contains the implementation of the simulation world and its elements
- the *abstracts* package, containing abstract classes within models
  - the abstract *Animal* class contains the implementation of common features of both animal variants, inheriting from WorldElement.
  - the abstract *World* class contains the implementation of common features of both map variants.
  - the abstract *WorldElement* class contains the implementation of common features of map elements.
- the *BasicAnimal* class contains the implementation of the standard version of the animal, inheriting from Animal.
- the *CrazyAnimal* class contains the implementation of the animal variant with ```a touch of madness```, inheriting from Animal.
- the *CreepingJungle* class contains the implementation of the map variant ```creeping jungle```, inheriting from World.
- the *Plant* class contains the implementation of a plant on the map, inheriting from WorldElement.
- the *RegularWorld* class contains the implementation of the standard version of the map, inheriting from World.
- the *Vector2d* class contains the implementation of a position on a plane.
- the *WorldElementBox* class contains a graphical representation of a map element.

*observers*, which contains classes implementing the observer pattern.
- the *MapChangeListener* interface, which presents a schema for reacting to map changes.

*presenters*, which contains presenter classes
- the abstract *BasePresenter* class, containing the implementation of common features of presenters.
- the *GamePresenter* class, describing the presenter of the simulation window, inheriting from BasePresenter.
- the *MenuPresenter* class, describing the presenter of the main program panel - the menu.

*records*, which contains records used within the project
- the *Boundary* record contains Vector2d positions describing the map dimensions.
- the *WorldConfig* record contains simulation parameters selected in the menu.

In the directory src/main/resources, there are project resources - .csv files, styles, .fxml files.
- the *configs* folder contains example simulation configurations
  - the *crazy_animal_config.csv* file contains an example configuration for the ```a touch of madness``` variant.
  - the *creeping_jungle_and_crazy_animal_config.csv* file contains an example configuration for both applied variants ```creeping jungle``` and ```a touch of madness```.
  - the *creeping_jungle_config.csv* file contains an example configuration for the ```creeping jungle``` variant.
- the *statistics* folder, to which .csv files with statistics are saved (if such an option is selected)
  - the *.gitignore* file indicates that we do not want to save statistics files to the repository.
- the *styles* folder, which contains the .css style descriptions
  - the *game.css* file contains style descriptions for the simulation window.
  - the *menu.css* file contains style descriptions for the main panel - the program menu.
- the *images* folder, which contains images displayed in the application
  - the *icon.png* file, which is the favicon of the application.
- the *game.fxml* file contains the description of the view for the simulation window.
- the *menu.fxml* file contains the description of the view for the menu.

In the directory src/test/java/agh/dg, there are tests for selected classes that are important for the program's operation.
- the *enums* package contains tests for enumeration types
  - the *MoveDirectionTest* class contains tests for the *MoveDirection* class.
- the *models* package
  Cell In[1], line 3
    readme_content = """
                     ^
SyntaxError: incomplete input

Error analyzing
Always expand output?
python
Copy code
# Correcting the mistake - properly defining the content and saving it to README.md file

readme_content = """
# Darwin World Project

### Main Part Structure of the Project
In the directory src/main/java/agh/dg, you can find the main project files.
We distinguish among them:
- the *DarwinWorldApp* class, which prepares the application for display.
- the *ExtendedThread* class, which contains the implementation of extending the Thread class, used in thread management for pausing and closing the simulation.
- the *Main* class, which launches the program.
- the *Simulation* class, which contains the implementation of the animal world simulation.
- the *Statistics* class, which stores statistical data displayed in the simulation.

Additionally, there are packages:
*enums*, which contains enumerations used in the application
- the *GameCommunicat* class contains messages used when displaying statistics.
- the *MoveDirection* class contains possible movement directions for animals.

*exceptions*, which contains custom exception classes used
- the *InvalidGameParamsException* class contains the implementation of an exception for providing invalid game parameters.

*helpers*, which contains helper classes for file handling and data conversion
- the *CsvFileHandler* class contains support for saving data to a .csv file.
- the *GameStatic* class contains conversion of an animal to color and statistical data to String.

*models*, which contains the implementation of the simulation world and its elements
- the *abstracts* package, containing abstract classes within models
  - the abstract *Animal* class contains the implementation of common features of both animal variants, inheriting from WorldElement.
  - the abstract *World* class contains the implementation of common features of both map variants.
  - the abstract *WorldElement* class contains the implementation of common features of map elements.
- the *BasicAnimal* class contains the implementation of the standard version of the animal, inheriting from Animal.
- the *CrazyAnimal* class contains the implementation of the animal variant with `a touch of madness`, inheriting from Animal.
- the *CreepingJungle* class contains the implementation of the map variant `creeping jungle`, inheriting from World.
- the *Plant* class contains the implementation of a plant on the map, inheriting from WorldElement.
- the *RegularWorld* class contains the implementation of the standard version of the map, inheriting from World.
- the *Vector2d* class contains the implementation of a position on a plane.
- the *WorldElementBox* class contains a graphical representation of a map element.

*observers*, which contains classes implementing the observer pattern.
- the *MapChangeListener* interface, which presents a schema for reacting to map changes.

*presenters*, which contains presenter classes
- the abstract *BasePresenter* class, containing the implementation of common features of presenters.
- the *GamePresenter* class, describing the presenter of the simulation window, inheriting from BasePresenter.
- the *MenuPresenter* class, describing the presenter of the main program panel - the menu.

*records*, which contains records used within the project
- the *Boundary* record contains Vector2d positions describing the map dimensions.
- the *WorldConfig* record contains simulation parameters selected in the menu.

In the directory src/main/resources, there are project resources - .csv files, styles, .fxml files.
- the *configs* folder contains example simulation configurations
  - the *crazy_animal_config.csv* file contains an example configuration for the `a touch of madness` variant.
  - the *creeping_jungle_and_crazy_animal_config.csv* file contains an example configuration for both applied variants `creeping jungle` and `a touch of madness`.
  - the *creeping_jungle_config.csv* file contains an example configuration for the `creeping jungle` variant.
- the *statistics* folder, to which .csv files with statistics are saved (if such an option is selected)
  - the *.gitignore* file indicates that we do not want to save statistics files to the repository.
- the *styles* folder, which contains the .css style descriptions
  - the *game.css* file contains style descriptions for the simulation window.
  - the *menu.css* file contains style descriptions for the main panel - the program menu.
- the *images* folder, which contains images displayed in the application
  - the *icon.png* file, which is the favicon of the application.
- the *game.fxml* file contains the description of the view for the simulation window.
- the *menu.fxml* file contains the description of the view for the menu.

In the `src/test/java/agh/dg` directory, there are tests for selected classes that are crucial for the program's operation.
- The *enums* package contains tests for enumeration types
  - The *MoveDirectionTest* class contains tests for the *MoveDirection* class.
- The *models* package contains tests for classes that form the application model
  - The *BasicAnimalTest* class contains tests for the BasicAnimal class.
  - The *CrazyAnimalTest* class contains tests for the CrazyAnimal class.
  - The *CreepingJungleTest* class contains tests for the CreepingJungle class.
  - The *RegularWorldTest* class contains tests for the RegularWorld class.
  - The *Vector2dTest* class contains tests for the Vector2d class.
- The *SimulationTest* class tests the code of methods from the Simulation class (though it does not run the simulation itself).
- The *StatisticsTest* class tests the correctness of handling statistical data.
