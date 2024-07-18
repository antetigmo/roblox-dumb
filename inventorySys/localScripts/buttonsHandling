local StarterGui = script.Parent
local userGui = StarterGui.userGui
local inventoryUi = StarterGui.inventoryUi

-- backpackButton 
local backpackButton = userGui.Main.backpackButton
local backpackButtonDebounce = false

-- inventoryUi
local inventoryMain = StarterGui.inventoryUi.Main
local closeButton = inventoryMain.closeButton


--local function closeAll()
	--for _, v do
		--if v == "Main" then
			--print(v)
		--end
--	end
--end

--closeAll()

function onCloseButton()
	inventoryMain.Visible = false
	backpackButtonDebounce = false
end

function onBackpackButton()
	if backpackButtonDebounce == false then
		backpackButtonDebounce = true
		inventoryMain.Visible = true
	elseif backpackButtonDebounce == true then
		backpackButtonDebounce = false
		inventoryMain.Visible = false
	end
end

closeButton.Activated:Connect(onCloseButton)
backpackButton.Activated:Connect(onBackpackButton)

