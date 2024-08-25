# State-Machine
This is a simple state machine for managing character states in roblox. 

@ Methods

--  StateMachine:Initiate(Character) 
--    Initializes a state machine for the given character.
-- 
--  StateMachine:Remove(Character) 
--    Removes the state machine for the given character.
-- 
--  StateMachine:ReturnData(Character, Path) 
--    Returns the state data at the specified path for the character.
-- 
--  StateMachine:PushState(Character, Path, NewValue, ExtraInfo) 
--    Updates the state of a character at the specified path with a new value and additional data.
-- 
--  StateMachine:CheckState(Character, Path) 
--    Checks the current state of a character at the specified path.
--
--  StateMachine:AppendState(Character, StateData) 
--    Appends a new state to the character's state machine.

@ Usage example.

-- local StateMachine = require(Path)
-- StateMachine:Initiate(Player.Character)
-- StateMachine:AppendState(Player.Character, { Name = "Jumping", Type = "Boolean" })
-- StateMachine:PushState(Player.Character, "Jumping", true)
-- local IsJumping = StateMachine:CheckState(Player.Character, "Jumping")

