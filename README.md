local PARTE = workspace.PARTE

PARTE.Touched:Connect(function()
	while PARTE.BrickColor ~= BrickColor.new("Bright green") do
		task.wait(0.5)
		PARTE.BrickColor = BrickColor.Random()

		if PARTE.BrickColor == BrickColor.new("Bright green") then
			print("Acabou")
			break
		end
	end
end)
