local PARTE = workspace.PARTE
local acabou = false

PARTE.Touched:Connect(function()
	if acabou then return end
	acabou = true
	PARTE.CanTouch = false

	while PARTE.BrickColor ~= BrickColor.new("Bright green") do
		wait(0.1)
		PARTE.BrickColor = BrickColor.Random()
	end

	PARTE.CanTouch = true
	print("Acabou")
end)
