local PARTE = workspace.PARTE

PARTE.Touched:Connect(function()
	
	
	
	while PARTE.BrickColor ~= BrickColor.new("Brigth green")do
		
		wait(0.1)
		
		PARTE.BrickColor = BrickColor.Random()
		
		if PARTE.BrickColor == BrickColor.new("Bright green") then
			
			print("Acabou")

			break
	end
	
	end
end)
