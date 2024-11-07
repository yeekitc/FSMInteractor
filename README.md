# FSM-Based UI Components (https://github.com/yeekitc/FSMInteractor.git)
A TypeScript implementation of interactive UI components using Finite State Machines (FSM), featuring standard UI elements and a custom interaction framework.

## Features
- **FSM-Driven Architecture**: Core finite state machine implementation powering all interactive components with clean state transitions and event handling
- **Standard UI Components**: Implementations of checkbox, radio buttons, rotary dial, and standard button
- **Event Management**: Robust event specification and handling system with filtering and propagation
- **Region Management**: Screen area definition and tracking with efficient damage/redraw mechanisms
- **Custom Interactive Component**

## How to Use
Since the renderer requires running over HTTP(S), set up a local web server to serve the project files. The Live Server extension on VS Code is an option. Then navigate to Debug and Run panel in VSCode to start the server, which will launch a Chrome browser window automatically.

## Project Structure
- **`src/`**: 
  - **`Action.ts`**: Defines actions triggered during FSM transitions
  - **`Check.ts`**: Handles validation and checking functionality
  - **`Err.ts`**: Error handling and management
  - **`EventSpec.ts`**: Handles user event specifications and management
  - **`FSM.ts`**: Core finite state machine implementation
  - **`FSMInteractor.ts`**: Base class for all interactive components
  - **`Region.ts`**: Screen region management for interactors
  - **`Root.ts`**: Tree management for FSMInteractor objects
  - **`State.ts`**: State management and definitions
  - **`test_cases.ts`**: Test implementations of various interactive components
  - **`Transition.ts`**: State transition logic for FSMs

## FSM Architecture
Each component is defined by:
- **States**: Distinct configurations (e.g., Button states: idle, hover, pressed)
- **Events**: User actions or system triggers that cause state changes
- **Transitions**: Rules for moving between states
- **Actions**: Behaviors executed during state transitions

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.