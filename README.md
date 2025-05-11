CreateScriptButton("Drift!", [[
--[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
if game:GetService("Players").LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid").RigType == Enum.HumanoidRigType.R6 then

	local char = game:GetService("Players").LocalPlayer.Character
	local hum = char:FindFirstChildWhichIsA("Humanoid")
	hum.WalkSpeed = 60
	hum.JumpPower = 20
	char.Animate.walk.WalkAnim.AnimationId = "rbxassetid://129342287"
	char.Animate.run.RunAnim.AnimationId = "rbxassetid://129342287"
	char.Animate.fall.FallAnim.AnimationId = "rbxassetid://129342287"
	char.Animate.idle.Animation1.AnimationId = "rbxassetid://129342287"
	char.Animate.idle.Animation2.AnimationId = "rbxassetid://129342287"
	char.Animate.jump.JumpAnim.AnimationId = "rbxassetid://129342287"
	for _, part in pairs(char:GetDescendants()) do
		if part:IsA("Part") then
			part.CustomPhysicalProperties = PhysicalProperties.new(0.04, 0, 0)
		end
	end
	hum.HipHeight = -1.03

elseif game:GetService("Players").LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid").RigType == Enum.HumanoidRigType.R15 then

	local char = game:GetService("Players").LocalPlayer.Character
	local hum = char:FindFirstChildWhichIsA("Humanoid")
	hum.WalkSpeed = 60
	hum.JumpPower = 20
	char.Animate.walk.WalkAnim.AnimationId = "rbxassetid://3360694441"
	char.Animate.run.RunAnim.AnimationId = "rbxassetid://3360694441"
	char.Animate.fall.FallAnim.AnimationId = "rbxassetid://3360694441"
	char.Animate.idle.Animation1.AnimationId = "rbxassetid://3360694441"
	char.Animate.idle.Animation2.AnimationId = "rbxassetid://3360694441"
	char.Animate.jump.JumpAnim.AnimationId = "rbxassetid://3360694441"
	for _, part in pairs(char:GetDescendants()) do
		if part:IsA("MeshPart") then
			part.CustomPhysicalProperties = PhysicalProperties.new(0.04, 0, 0)
		end
	end
	hum.HipHeight = 0.56

end
]])
