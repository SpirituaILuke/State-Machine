# State-Machine

A simple state machine for managing character states in Roblox.

## Methods

### `StateMachine:Initiate(Character)`
Initializes a state machine for the given character.

### `StateMachine:Remove(Character)`
Removes the state machine for the given character.

### `StateMachine:ReturnData(Character, Path)`
Returns the state data at the specified path for the character.

### `StateMachine:PushState(Character, Path, NewValue, ExtraInfo)`
Updates the state of a character at the specified path with a new value and additional data.

### `StateMachine:CheckState(Character, Path)`
Checks the current state of a character at the specified path.

### `StateMachine:AppendState(Character, StateData)`
Appends a new state to the character's state machine.

## Examples

### Basic Example

```lua
local StateMachine = require(Path)

-- Initialize the state machine for the character
StateMachine:Initiate(Player.Character)

-- Append a new state for jumping
StateMachine:AppendState(Player.Character, { Name = "Jumping", Type = "Boolean" })

-- Push a new value to the "Jumping" state
StateMachine:PushState(Player.Character, "Jumping", true)

-- Check if the character is jumping
local IsJumping = StateMachine:CheckState(Player.Character, "Jumping")
